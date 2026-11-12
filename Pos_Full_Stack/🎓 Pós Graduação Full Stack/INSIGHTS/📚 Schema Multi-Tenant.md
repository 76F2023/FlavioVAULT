# 📚 Schema Multi-Tenant

> Arquitetura utilizada principalmente em aplicações SaaS para permitir que vários clientes utilizem a mesma aplicação com isolamento de dados.

---

# Conceitos Fundamentais

|Termo|Definição|
|---|---|
|**Tenant**|Cliente, empresa ou organização que utiliza o sistema.|
|**Multi-Tenant**|Arquitetura onde vários tenants compartilham a mesma aplicação.|
|**Isolamento de Dados**|Garantia de que um cliente não terá acesso aos dados de outro cliente.|
|**SaaS**|Software como Serviço (Software as a Service).|

---

# Exemplo Prático

Imagine um SaaS de Gestão de Vendas com três empresas utilizando a mesma aplicação:

|Empresa|Tenant ID|
|---|---|
|Empresa A|100|
|Empresa B|200|
|Empresa C|300|

---

## Estrutura da Tabela

SQL

clientes

---------

id

tenant_id

nome

email

### Dados Armazenados

|id|tenant_id|nome|
|---|---|---|
|1|100|João|
|2|100|Maria|
|3|200|Pedro|

### Resultado

|Usuário Logado|Dados Visíveis|
|---|---|
|Tenant 100|João, Maria|
|Tenant 200|Pedro|
|Tenant 300|Apenas seus próprios dados|

---

# Modelos de Multi-Tenancy

## 1. Banco Compartilhado + Schema Compartilhado

Todos os clientes utilizam as mesmas tabelas.

### Estrutura

Plain Text

Banco

├── usuarios

├── vendas

└── produtos

### Exemplo

SQL

SELECT *

FROM clientes

WHERE tenant_id = 100;

### Características

|Aspecto|Avaliação|
|---|---|
|Custo|⭐ Muito baixo|
|Complexidade|⭐ Baixa|
|Escalabilidade|⭐⭐⭐⭐⭐ Alta|
|Isolamento|⭐⭐ Médio|
|Manutenção|⭐⭐⭐⭐⭐ Fácil|

### Vantagens

|Vantagem|
|---|
|Menor custo operacional|
|Mais fácil de desenvolver|
|Escala facilmente|
|Menor consumo de recursos|

### Desvantagens

|Desvantagem|
|---|
|Exige filtros por tenant em todas as consultas|
|Maior risco de vazamento de dados por erro de programação|
|Customizações por cliente são mais difíceis|

---

## 2. Banco Compartilhado + Schema por Tenant

Cada cliente possui seu próprio schema.

### Estrutura

Plain Text

Banco

├── empresa_a

│ ├── usuarios

│ └── vendas

│

├── empresa_b

│ ├── usuarios

│ └── vendas

│

└── empresa_c

├── usuarios

└── vendas

### Exemplo no PostgreSQL

Plain Text

empresa_a.clientes

empresa_b.clientes

empresa_c.clientes

### Características

|Aspecto|Avaliação|
|---|---|
|Custo|⭐⭐ Médio|
|Complexidade|⭐⭐⭐ Média|
|Escalabilidade|⭐⭐⭐⭐ Boa|
|Isolamento|⭐⭐⭐⭐ Alto|
|Manutenção|⭐⭐⭐ Média|

### Vantagens

|Vantagem|
|---|
|Melhor isolamento|
|Facilita customizações|
|Menor risco de vazamento de dados|
|Organização por cliente|

### Desvantagens

|Desvantagem|
|---|
|Administração mais complexa|
|Migrações podem ser mais trabalhosas|
|Crescimento do número de schemas|

---

## 3. Banco por Tenant

Cada cliente possui seu próprio banco de dados.

### Estrutura

Plain Text

Banco_Empresa_A

Banco_Empresa_B

Banco_Empresa_C

### Características

|Aspecto|Avaliação|
|---|---|
|Custo|⭐⭐⭐⭐⭐ Alto|
|Complexidade|⭐⭐⭐⭐⭐ Alta|
|Escalabilidade|⭐⭐⭐ Média|
|Isolamento|⭐⭐⭐⭐⭐ Máximo|
|Manutenção|⭐⭐ Difícil|

### Vantagens

|Vantagem|
|---|
|Isolamento total|
|Backups independentes|
|Melhor segurança|
|Facilita requisitos corporativos|

### Desvantagens

|Desvantagem|
|---|
|Alto custo|
|Infraestrutura mais complexa|
|Operação mais difícil|

---

# Comparação Geral

|Critério|Banco Compartilhado|Schema por Tenant|Banco por Tenant|
|---|---|---|---|
|Custo|Baixo|Médio|Alto|
|Isolamento|Baixo|Médio/Alto|Máximo|
|Escalabilidade|Alta|Alta|Média|
|Complexidade|Baixa|Média|Alta|
|Customização|Baixa|Média|Alta|
|Backup Individual|Não|Parcial|Sim|
|Segurança|Média|Boa|Excelente|

---

# O Que Geralmente é Chamado de "Schema Multi-Tenant"?

Na prática, quando desenvolvedores falam:

> "Estamos usando Schema Multi-Tenant"

geralmente estão se referindo à seguinte arquitetura:

Plain Text

PostgreSQL

│

├── public

├── cliente_1

├── cliente_2

├── cliente_3

└── cliente_n

Cada tenant possui um schema próprio dentro do mesmo banco de dados.

---

# Quando Utilizar Cada Modelo?

|Cenário|Recomendação|
|---|---|
|MVP SaaS|Banco Compartilhado + Tenant ID|
|Até centenas de clientes|Banco Compartilhado + Tenant ID|
|Clientes corporativos|Schema por Tenant|
|Clientes Enterprise|Banco por Tenant|
|Necessidade máxima de segurança|Banco por Tenant|
|Necessidade de menor custo|Banco Compartilhado|

---

# Arquitetura Recomendada para um Novo SaaS

Plain Text

Fase 1 → Tenant ID nas tabelas

↓

Fase 2 → Schema por Tenant

↓

Fase 3 → Banco dedicado para clientes Enterprise

Essa abordagem permite começar simples, com baixo custo e alta velocidade de desenvolvimento, evoluindo conforme o crescimento da base de clientes.

---

# Resumo Rápido

|Modelo|Melhor Para|
|---|---|
|Banco Compartilhado (`tenant_id`)|MVPs e SaaS iniciantes|
|Schema por Tenant|SaaS em crescimento|
|Banco por Tenant|Grandes clientes corporativos|

> **Regra prática:** 90% dos SaaS começam utilizando um único banco compartilhado com uma coluna `tenant_id`. Conforme surgem requisitos de segurança, customização e clientes maiores, evoluem para schemas dedicados ou bancos exclusivos.