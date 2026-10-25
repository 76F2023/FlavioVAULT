# 📅 Cronograma de Projeto: Prazos e Definição de Atividades ao Longo do Tempo

> **Fonte:** [Cronograma de Projeto - Prazos e Definição de atividades ao longo do tempo](https://www.youtube.com/watch?v=2BQXnur4jww "null")
> 
> **Canal:** Thiago Jabur

## 📌 1. Conceito e Importância do Cronograma

O **cronograma** é a ferramenta essencial de planejamento e controle que mapeia a execução do projeto ao longo do tempo. Ele converte o escopo definido em uma linha temporal concreta, permitindo monitorar o progresso e garantir a entrega nos prazos estipulados.

- **Objetivo Principal:** Prever o tempo necessário para conclusão do projeto e coordenar os recursos ao longo das fases.
    
- **Benefícios:**
    
    - Alinhamento de expectativas com _stakeholders_.
        
    - Facilidade de identificação de gargalos antes que ocorram.
        
    - Base para medir o avanço físico e financeiro.
        

## 🛠️ 2. Passos para Elaboração do Cronograma

Para construir um cronograma eficiente, é necessário seguir uma sequência estruturada de gerenciamento de tempo:

```
graph TD
    A[1. Definir Atividades / EAP] --> B[2. Sequenciar Atividades]
    B --> C[3. Estimar Recursos e Duração]
    C --> D[4. Desenvolver o Cronograma]
    D --> E[5. Controlar e Acompanhar]
```

### Step 1: Definição de Atividades (EAP / WBS)

- Desmembramento das entregas em pacotes de trabalho e tarefas menores (_Work Breakdown Structure_).
    
- Garante que nenhuma etapa crítica seja esquecida.
    

### Step 2: Sequenciamento de Atividades

- Identificação das dependências e relações lógicas entre as tarefas:
    
    - **Término para Início (TI):** A tarefa B só começa quando A terminar.
        
    - **Início para Início (II):** A tarefa B pode começar junto com A.
        
    - **Término para Término (TT):** A tarefa B só termina quando A terminar.
        

### Step 3: Estimativa de Duração e Recursos

- Atribuição da quantidade de tempo e recursos (humanos, materiais e financeiros) para cada atividade.
    
- Utilização de técnicas como estimativa por analogia, paramétrica ou de três pontos (PERT).
    

### Step 4: Desenvolvimento e Ajustes

- Consolidação das atividades, prazos e dependências em uma ferramenta de visualização (ex.: **Gráfico de Gantt**).
    
- Definição da **Linha de Base (Baseline)** do projeto.
    

## ⚡ 3. Elementos Fundamentais do Gerenciamento de Prazos

- **Caminho Crítico (CPM - Critical Path Method):** A sequência de atividades interdependentes que determina a duração total mínima do projeto. Tarefas no caminho crítico têm folga zero.
    
- **Folga (Float/Slack):** O tempo que uma atividade pode ser atrasada sem impactar a data final do projeto.
    
- **Compressão de Cronograma (se necessário):**
    
    - _Fast-tracking:_ Executar tarefas em paralelo que originalmente seriam em sequência.
        
    - _Crashing:_ Adicionar mais recursos para reduzir o tempo de execução.
-------------------------------------------------------------------

# 🔗 Cronograma de Projeto - Parte 2: Sequenciamento de Atividades e Estimativas

> **Fonte:** [Cronograma de Projeto - Parte 2 - Sequenciamento de atividades - Estimativas](http://www.youtube.com/watch?v=DEVX4cGVdDY "null")
> 
> **Canal:** Thiago Jabur
> 
> **Nota Relacionada:** [[cronograma_projeto_obsidian|Cronograma de Projeto - Parte 1]]

## 🔗 1. Sequenciamento de Atividades

O **sequenciamento de atividades** é o processo de identificação e documentação das relações de dependência entre as tarefas do projeto. Ele define a ordem lógica de execução para otimizar tempo e recursos.

### Tipos de Dependências Lógicas

|                          |             |                                                                                 |                                                                         |
| ------------------------ | ----------- | ------------------------------------------------------------------------------- | ----------------------------------------------------------------------- |
| **Tipo de Relação**      | **Sigla**   | **Descrição**                                                                   | **Exemplo**                                                             |
| **Término para Início**  | **TI** (FS) | A atividade _B_ só pode iniciar após o término da atividade _A_. _(Mais comum)_ | A pintura da parede só começa após a secagem do reboco.                 |
| **Início para Início**   | **II** (SS) | A atividade _B_ só pode iniciar após o início da atividade _A_.                 | A pavimentação da pista só inicia após o início do nivelamento do solo. |
| **Término para Término** | **TT** (FF) | A atividade _B_ só pode terminar após o término da atividade _A_.               | A documentação técnica só termina quando o desenvolvimento terminar.    |
| **Início para Término**  | **IT** (SF) | A atividade _B_ só pode terminar após o início da atividade _A_. _(Raro)_       | O plantão da equipe antiga só termina quando a nova equipe iniciar.     |

### Antecipações e Esperas (Leads & Lags)

- **Antecipação (**_**Lead**_**):** Adiantamento do início de uma atividade sucessora antes que a antecessora seja concluída (ex.: iniciar os testes de software 2 dias antes do fim do desenvolvimento).
    
- **Espera (**_**Lag**_**):** Tempo de retardo obrigatório entre a conclusão de uma atividade e o início da próxima (ex.: aguardar 3 dias de cura do concreto antes de subir a estrutura).
    

## ⏱️ 2. Estimativa de Duração de Atividades

Estimar a duração consiste em avaliar o número de períodos de trabalho necessários para concluir cada tarefa com os recursos previstos.

### Técnicas de Estimativa

```
graph LR
    A[Técnicas de Estimativa] --> B[Opinião de Especialistas]
    A --> C[Estimativa por Analogia]
    A --> D[Estimativa Paramétrica]
    A --> E
```

