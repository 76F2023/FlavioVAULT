# 🚀 Google Antigravity 2.0: Guia de Desenvolvimento Orientado a Agentes

O **Google Antigravity 2.0** é um ambiente de desenvolvimento orientado a agentes de Inteligência Artificial. Diferente de um chatbot tradicional que apenas escreve código isolado, o Antigravity gerencia agentes capazes de entender o contexto global de um projeto, planejar soluções, executar comandos no terminal, automatizar navegadores e validar os resultados de ponta a ponta.

---

## 🧭 Mudança de Mentalidade: Do Prompting à Delegação

* **Desenvolvimento com IA Tradicional:** Você pede uma função, copia o código, cola no editor, encontra um erro, joga o erro na IA e repete o ciclo operacional.
* **Desenvolvimento com Antigravity:** Você passa um **Objetivo Verificável** (ex: criar uma tela, integrar com a API, validar os campos e testar no navegador). O agente investiga o projeto, altera múltiplos arquivos, roda testes e entrega as evidências.
* **Fórmula de Comunicação Eficiente:** `Contexto ➡️ Objetivo ➡️ Restrições ➡️ Critérios de Aceitação`.

---

## 💻 Tabela de Comandos Especiais (Slash Commands)

Use estes comandos diretamente no chat do Antigravity para ditar o modo de operação do agente:

| Comando | Função Principal | Quando Utilizar |
| :--- | :--- | :--- |
| `/plan` | Força o agente a analisar o escopo e criar uma estratégia de arquitetura antes de mexer no código. | Funcionalidades grandes, migrações e refatorações complexas. |
| `/grill-me` | Faz o agente questionar seus requisitos e apontar lacunas (ex: esquecimento de fluxos de reembolso ou falha de pagamento). | No início de um projeto, quando os requisitos ainda estão nebulosos. |
| `/goal` | Define uma condição de conclusão para a IA trabalhar de forma 100% autônoma até o objetivo ser atingido. | Tarefas muito longas onde você não quer ficar digitando "continue". |
| `/browser` | Aciona o Browser Agent para abrir o navegador, interagir com a aplicação, testar fluxos e validar responsividade. | Validar se telas, botões e gráficos estão funcionando visualmente. |
| `/btw` | Permite fazer uma pergunta paralela em um chat separado sem interromper ou poluir o fluxo da tarefa principal. | Descobrir em qual arquivo uma interface está definida enquanto a IA coda. |
| `/learn` | Registra correções e aprendizados da conversa atual para gerar novas regras (`rules`) ou habilidades (`skills`) persistentes. | Quando a IA comete um erro e você a ensina o padrão correto para que não repita no futuro. |
| `/schedule`| Configura rotinas, análises recorrentes ou execuções agendadas para o agente fazer sozinho. | Automações diárias de repositórios, checagem de branches ou relatórios periódicos. |

---

## 🛠️ Conceitos-Chave da Ferramenta

### 1. Projects (Contexto Controlado)
Os projetos definem o escopo de atuação do agente. Em vez de liberar acesso ao computador inteiro, você aponta para pastas ou repositórios específicos (é possível incluir múltiplos repositórios, integrando Front-end e Back-end).

### 2. Terminal Integrado & Ciclo de Validação
O agente interage com o terminal de forma nativa. Ele pode rodar comandos como `npm install`, `npm test` e `npm run build`. Caso um erro aconteça no terminal, o próprio agente analisa a saída e se autocorrige.

### 3. Artifacts (Artefatos)
Resultados estruturados gerados pelo agente para fins de revisão humana. Podem incluir planos de implementação, diagramas, diffs de código, mídias e gravações de testes feitos no navegador. **Autonomia não elimina a supervisão**.

### 4. Rules & Skills
* **Rules (Regras):** Instruções persistentes globais ou por Workspace (ex: "Sempre use TypeScript", "Nunca use Any").
* **Skills (Habilidades):** Processos complexos e reutilizáveis ensinados por você (ex: uma skill de auditoria de SEO ou uma rotina específica de Deploy).

### 5. MCP (Model Context Protocol)
Protocolo padronizado que conecta os agentes a ferramentas e infraestruturas externas ao seu computador local, como bancos de dados PostgreSQL, APIs corporativas e a plataforma do GitHub.

### 6. Segurança e Git Worktrees
* **Worktrees (Módulo Isolado):** Permite que o agente trabalhe em cópias isoladas do repositório. Excelente para experimentos arriscados, permitindo que você revise o Diff antes de consolidar as alterações.
* **Strict Mode:** Configuração para restringir ações destrutivas (como `rm`, `drop database`, `git reset` ou alterações em produção) exigindo sempre a aprovação expressa do usuário.

### 7. Orquestração de Múltiplos Agentes
Permite abrir conversas com múltiplos agentes especializados trabalhando em paralelo (ex: um focado em Back-end, um em Front-end, um em Segurança e outro em Testes) atuando de forma coordenada sob sua gerência.

---

## 📈 Trilha de Aprendizado Recomendada
Não tente dominar tudo no primeiro dia. Siga esta ordem de evolução técnica:
1. **Fundamentos:** Domine o Agente, o uso do Terminal, o Git e o Browser.
2. **Planejamento:** Aprenda a delegar usando `/plan` e criar bons critérios de aceitação.
3. **Padronização:** Comece a criar suas próprias `Rules` e `Skills`.
4. **Automação e Escala:** Implemente rotinas com `/schedule`, conexões via MCP e múltiplos agentes.
-----------------------------------------------------------------------
# 📑 Template: Prompt Estruturado para Antigravity

> [!info] Instruções de Uso
> Use este template sempre que for delegar uma tarefa média ou grande para o agente técnico. Preencha os campos entre colchetes `[ ]` e cole o bloco inteiro no chat da ferramenta.

---

## 📌 Contexto
Estou trabalhando no projeto local de **[Nome do Sistema/Contexto Geral]**. A estrutura atual utiliza as seguintes tecnologias: **[Tecnologias principais, ex: React, Next.js, FastAPI, Prisma, etc.]**. 
O código atual do fluxo de **[Módulo afetado, ex: Autenticação, Relatórios, Checkout]** está localizado no diretório `[caminho/do/diretorio/ou/arquivo.ext]`.

## 🎯 Objetivo
Quero adicionar/modificar a seguinte funcionalidade:
* **[Descreva o objetivo principal de forma direta e sem ambiguidade]**
* **[Adicione sub-tarefas essenciais se houver]**

## 🛑 Restrições
Para a execução desta tarefa, você **NÃO** deve:
* Alterar o mecanismo existente de **[Mecanismo que deve ser preservado, ex: Autenticação, banco de dados]**.
* Adicionar novas dependências externas sem antes me consultar.
* Usar o tipo `any` ou deixar de tipar os novos retornos (se aplicável ao projeto).
* **[Adicione outras restrições arquiteturais específicas da sua empresa/projeto]**.

## ✅ Critérios de Aceitação (Condições de Conclusão)
A tarefa só será considerada concluída quando você validar e garantir que:
1. O plano inicial gerado por você faça sentido arquitetural.
2. O código compile e passe pelo processo de build sem nenhum aviso ou erro no terminal.
3. Todos os testes unitários/integração existentes e novos estejam passando com sucesso.
4. O fluxo principal da interface funcione perfeitamente ao ser testado no ambiente local através do navegador.

---

## ⚡ Comandos de Inicialização (Workflow recomendado)

Abaixo estão os comandos iniciais que usaremos para validar este escopo. 

1. Primeiro, execute o comando abaixo para encontrar possíveis lacunas nos meus requisitos de negócios:
`/grill-me`

2. Após respondermos as perguntas do passo anterior, analise a arquitetura do projeto e monte a estratégia de implementação através de um artefato:
`/plan`

3. Quando validarmos o plano, execute o trabalho de forma autônoma até cumprir todos os critérios de aceitação listados acima:
`/goal`
