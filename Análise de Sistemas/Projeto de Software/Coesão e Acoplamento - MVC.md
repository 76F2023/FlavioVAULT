# Projeto de Software - Coesão e Acoplamento - MVC

## Visão Geral

A qualidade de um projeto de software depende diretamente da forma como seus componentes são organizados e relacionados.

Dois conceitos fundamentais para avaliar a qualidade de uma arquitetura são:

- Coesão
- Acoplamento

Além disso, o padrão arquitetural **MVC (Model-View-Controller)** é apresentado como uma forma prática de melhorar a organização do sistema.

---

# Coesão

## Definição

Coesão representa o grau de relacionamento entre as responsabilidades de um módulo.

Uma classe ou componente coeso possui funções relacionadas a um único propósito.

### Alta Coesão

Características:

- Responsabilidade bem definida.
- Código mais fácil de entender.
- Maior reutilização.
- Menor impacto de mudanças.

Exemplo:

```text
ClienteService
├── cadastrarCliente()
├── atualizarCliente()
├── removerCliente()
└── buscarCliente()
```

Todas as operações estão relacionadas ao domínio "Cliente".

---

### Baixa Coesão

Características:

- Muitas responsabilidades misturadas.
- Dificuldade de manutenção.
- Maior chance de erros.

Exemplo:

```text
SistemaUtil

├── cadastrarCliente()
├── gerarPDF()
├── enviarEmail()
├── calcularFolha()
└── conectarBanco()
```

A classe acumula responsabilidades sem relação direta.

---

# Acoplamento

## Definição

Acoplamento mede o nível de dependência entre módulos.

Quanto mais um componente depende de outro, maior o acoplamento.

---

## Alto Acoplamento

Problemas:

- Mudanças propagam erros.
- Código difícil de testar.
- Baixa flexibilidade.
- Menor reutilização.

Exemplo:

```java
Pedido pedido = new Pedido();
BancoMySQL banco = new BancoMySQL();
banco.salvar(pedido);
```

O código depende diretamente de uma implementação específica.

---

## Baixo Acoplamento

Benefícios:

- Flexibilidade.
- Facilidade para manutenção.
- Melhor testabilidade.
- Maior reutilização.

Exemplo:

```java
Repositorio repositorio;
repositorio.salvar(pedido);
```

O sistema depende de abstrações.

---

# Relação Entre Coesão e Acoplamento

Objetivo de um bom projeto:

✅ Alta Coesão

✅ Baixo Acoplamento

Essa combinação produz sistemas:

- Mais organizados.
- Mais fáceis de evoluir.
- Menos suscetíveis a falhas.

---

# MVC (Model-View-Controller)

## Objetivo

Separar responsabilidades dentro do software.

MVC divide o sistema em três camadas principais:

```text
Usuário
   ↓
 View
   ↓
Controller
   ↓
 Model
   ↓
Banco de Dados
```

---

# Model

Representa:

- Dados.
- Regras de negócio.
- Persistência.

Responsabilidades:

- Validar regras.
- Manipular entidades.
- Interagir com banco de dados.

Exemplo:

```java
Cliente
Pedido
Produto
```

---

# View

Responsável pela interface.

Funções:

- Exibir informações.
- Receber entradas do usuário.

Exemplos:

- Página HTML
- Formulário
- Tela Mobile

A View não deve conter regras de negócio.

---

# Controller

Responsável pela coordenação.

Funções:

- Receber requisições.
- Acionar Models.
- Retornar resultados para a View.

Exemplo:

```text
Usuário clica em "Salvar"

↓

Controller recebe ação

↓

Model grava dados

↓

View exibe confirmação
```

---

# Fluxo MVC

```text
1. Usuário interage com a View

2. Controller recebe a ação

3. Controller chama o Model

4. Model processa regras de negócio

5. Model retorna resultado

6. Controller envia resposta

7. View apresenta ao usuário
```

---

# Benefícios do MVC

## Organização

Cada componente possui uma responsabilidade específica.

## Manutenção

Alterações na interface não afetam regras de negócio.

## Reutilização

O mesmo Model pode servir várias interfaces.

## Escalabilidade

Facilidade para crescimento do sistema.

## Testabilidade

As camadas podem ser testadas separadamente.

---

# Problemas Comuns

## Controller Gigante

Quando todas as regras ficam no Controller.

Consequências:

- Baixa coesão.
- Difícil manutenção.

---

## View Inteligente

Quando a interface contém regras de negócio.

Consequências:

- Violação do MVC.
- Aumento do acoplamento.

---

## Model Anêmico

Quando o Model contém apenas dados.

Consequências:

- Regras acabam espalhadas pelo sistema.

---

# Resumo para Prova

### Coesão

- Mede a relação entre responsabilidades internas.
- Quanto maior, melhor.

### Acoplamento

- Mede dependência entre módulos.
- Quanto menor, melhor.

### Regra de Ouro

> Projetar sistemas com ALTA COESÃO e BAIXO ACOPLAMENTO.

### MVC

Model:

- Dados e regras de negócio.

View:

- Interface com o usuário.

Controller:

- Coordena a comunicação entre View e Model.

### Benefícios do MVC

- Organização.
- Manutenção.
- Reuso.
- Escalabilidade.
- Testabilidade.

### Resumo em uma frase

> **Um bom projeto de software busca alta coesão e baixo acoplamento, e o padrão MVC ajuda a alcançar esse objetivo separando claramente dados, interface e controle da aplicação.** [[youtube.com]](https://www.youtube.com/watch?v=nGVy_JisFRY), [[devmedia.com.br]](https://www.devmedia.com.br/entendendo-coesao-e-acoplamento/18538)