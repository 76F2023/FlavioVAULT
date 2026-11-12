tipo: aula curso: Pós-Graduação em Desenvolvimento de Software Full Stack disciplina: data: 2026-11-04 fontes:

- "[[Desenvolvimento de Software Centrado no Usuário]]"
- "[[Descoberta de Sistemas]]"
- "[[Engenharia de Requisitos]]"
- "[[Especificação e DDR]]"
- "[[Tipos de Requisitos]]"
- "[[Levantamento de Requisitos]]" tags:
- aula
- estudo
- ddr
- requisitos

---

# DDR na Prática

## Resumo

O DDR (Documento de Definição de Requisitos) é o artefato central que consolida todos os resultados da descoberta e da engenharia de requisitos. Esta aula, dividida em cinco blocos práticos, mostra como construir um DDR de verdade: quando começar, quem escreve cada seção, como redigir requisitos funcionais e não funcionais mensuráveis, como montar a matriz de rastreabilidade com critérios de aceite testáveis e como manter o documento vivo ao longo do projeto. O foco é transformar a teoria da especificação em um documento operacional que a equipe de desenvolvimento consiga usar no dia a dia, e que sirva de base para testes, homologação e aprovação.

---

## Conceitos principais

- DDR como documento vivo: não é um artefato que se escreve uma única vez no início e se abandona — ele evolui com o projeto, sempre versionado e rastreado. Quem tenta "congelar" o DDR no primeiro rascunho condena o projeto a trabalhar com uma especificação desatualizada.
- Identificador de requisito: cada requisito recebe um código único e imutável (ex.: `RF-001`, `RNF-003`, `RN-007`). O código é a âncora da rastreabilidade: nunca se renumera requisito após publicação — cria-se versão nova do mesmo código ou se marca como obsoleto.
- Fonte de origem: todo requisito precisa declarar de onde veio (entrevista, observação, desk research, persona, JTBD, Matriz CSD, regra de negócio da organização). Sem origem, o requisito é indetectável quanto à validade quando algo mudar.
- Critério de aceite escrito antes do desenvolvimento: a prática de escrever o aceite junto com o requisito — e não depois — força o time a pensar no que significa "pronto" antes de codificar, e transforma o DDR em base de teste.
- Nível de requisito: usuário × sistema. O requisito de usuário descreve a necessidade de negócio em linguagem acessível; o requisito de sistema detalha o comportamento técnico mensurável. O DDR separa os dois, mas os conecta pela rastreabilidade.

---

## Conteúdo da aula

### BLOCO 1 — Preparação: quando e como começar o DDR

#### Quando começar a escrever

O erro mais comum é começar o DDR "do zero" depois de encerrar a descoberta, como se fosse uma redação final. Na prática, o DDR nasce durante o levantamento:

- A cada entrevista, os achados já são registrados com um rascunho de requisito candidato.
- A Observação gera requisitos implícitos — tarefas reais que o usuário executa e que viram requisitos funcionais reais.
- A Desk research alimenta regras de negócio e requisitos não funcionais (prazos legais, conformidade, padrões de mercado).
- A Matriz CSD aponta o que ainda é Suposição — e suposição não pode virar requisito sem virar hipótese validada ou ser assumida como risco explicitamente.

Regra prática: não detalhe tudo antes de priorizar. Primeiro priorize (MoSCoW, RICE) e depois detalhe o que realmente vai ser construído no horizonte próximo. Detalhar um requisito "Would" que nunca será implementado é retrabalho garantido.

#### Quem escreve cada seção

O DDR não é responsabilidade de uma única pessoa. Na prática:

|Seção|Responsável principal|Contribuintes|
|---|---|---|
|Introdução e visão geral|PO / analista de negócio|PM, stakeholders|
|Stakeholders e usuários|PO / UX|Pesquisa, suporte|
|Requisitos funcionais|Analista de requisitos|PO, devs, UX|
|Requisitos não funcionais|Arquiteto / tech lead|Devs, infra, segurança|
|Regras de negócio|Especialista do domínio|PO, jurídico/compliance|
|Rastreabilidade|Analista de requisitos|Todo o time|
|Critérios de aceite|PO + QA + dev|UX|
|Glossário|Analista + UX|Especialista do domínio|

#### Checklist de entrada (pré-condições para o DDR)

Antes de começar a escrever de fato, verifique se você tem em mãos:

- [ ]  Personas e JTBD definidos (quem e qual "trabalho")
- [ ]  Achados de entrevistas e observação consolidados
- [ ]  Matriz CSD com suposições sinalizadas
- [ ]  Requisitos priorizados (pelo menos no nível Must/Should)
- [ ]  Escopo do horizonte (o que entra agora, o que fica para depois)
- [ ]  Glossário mínimo com termos do domínio

Se faltar algum desses itens, o DDR nascerá com buracos que vão gerar retrabalho nas próximas etapas.

---

### BLOCO 2 — Escrevendo requisitos funcionais na prática

#### Formato padronizado de um requisito funcional

Cada requisito funcional deve seguir uma estrutura fixa no documento:

|Campo|Descrição|Exemplo|
|---|---|---|
|ID|Código único|`RF-014`|
|Título|Nome curto e descritivo|"Filtrar pedidos por status"|
|Ator|Quem executa a ação|Usuário autenticado com perfil de atendente|
|Ação|Verbo de ação específico|filtrar|
|Objeto|Sobre o que recai a ação|lista de pedidos|
|Condição/Critério|Quando e sob quais regras|por status aberto, com atualização automática|
|Prioridade|MoSCoW / RICE|Must|
|Fonte|Origem do requisito|Entrevista com atendentes (Ver [[Entrevistas]])|
|Aceite|ID do critério de aceite vinculado|`CA-014`|

#### A fórmula de escrita (regra de ouro)

> Ator + ação + objeto + condição/critério mensurável.

- ❌ Ruim: "O sistema deve ser bom para filtrar pedidos."
- ✅ Bom: "O atendente autenticado deve filtrar a lista de pedidos por status, exibindo apenas os pedidos do status selecionado em até 2 segundos."

Perceba que a versão boa usa verbo específico, ator identificado e critério mensurável (`em até 2 segundos`).

#### Um requisito por frase

Nunca escreva dois requisitos na mesma frase com "e". Exemplo:

- ❌ Ruim: "O usuário deve poder exportar o relatório em PDF e enviar por e-mail."
- ✅ Bom: `RF-031` "O usuário deve exportar o relatório em PDF." / `RF-032` "O usuário deve enviar o relatório exportado por e-mail."

Separar força cada requisito a ser testado, priorizado e rastreado individualmente.

#### Exemplo prático de bloco no DDR

> ### RF-014 — Filtrar pedidos por status
> 
> - Ator: atendente autenticado
> - Descrição: o atendente deve filtrar a lista de pedidos por status (aberto, em separação, enviado, cancelado), exibindo apenas os pedidos do status selecionado.
> - Prioridade: Must
> - Fonte: Entrevista com atendentes (S04) e Observação da rotina de atendimento
> - Critério de aceite: `CA-014`
> - Rastreabilidade: [[Levantamento de Requisitos]] · [[Tipos de Requisitos]]

---

### BLOCO 3 — Requisitos não funcionais e regras de negócio

#### Requisitos não funcionais (RNF)

A regra é a mesma dos funcionais: mensurabilidade. Cada RNF precisa ser verificável objetivamente. A pior palavra num RNF é um adjetivo solto: "rápido", "seguro", "intuitivo", "robusto".

Conversão de adjetivo para medida:

|Adjetivo vago|Critério mensurável|Tipo de RNF|
|---|---|---|
|"rápido"|tempo de resposta ≤ 2s para 10.000 registros|Desempenho|
|"seguro"|criptografia TLS 1.3 em trânsito; AES-256 em repouso|Segurança|
|"disponível"|99,9% uptime mensal (máx. 43,8 min de indisponibilidade)|Disponibilidade|
|"intuitivo"|tarefa concluída por 80% dos usuários sem ajuda, em ≤ 3 min|Usabilidade|
|"funciona no celular"|responsivo para viewports de 320px a 1440px; toques com área mínima de 44×44px|Compatibilidade|

Cada um desses vira um `RNF-XXX` com ID, fonte (geralmente desk research, benchmark, SLA da organização) e critério de verificação.

#### Regras de negócio (RN)

Regras de negócio não são requisitos do sistema — são restrições impostas pela organização, independentemente de tecnologia. Mas o DDR precisa registrá-las porque elas condicionam os requisitos.

- Exemplo: `RN-003` "Pedidos acima de R$ 10.000 exigem aprovação de um supervisor."
- Essa regra não descreve uma tela, mas gera requisitos funcionais: campo de aprovação, fluxo de encaminhamento, notificação ao supervisor.

Prática recomendada: liste as regras de negócio uma única vez, num capítulo próprio, e aponte para elas a partir dos requisitos que elas condicionam. Assim, se a regra mudar, a análise de impacto identifica rapidamente todo requisito afetado (conexão direta com [[Gerenciamento e Mudanças]]).

---

### BLOCO 4 — Rastreabilidade e critérios de aceite na prática

#### Matriz de rastreabilidade

A matriz é a espinha dorsal do DDR. Sem ela, o documento é uma coleção de frases bonitas. Na prática, monte uma tabela que responda a três perguntas para cada requisito:

1. De onde veio? (fonte/rastreabilidade vertical)
2. Para onde vai? (casos de uso, histórias, casos de teste)
3. O que o cobre? (critérios de aceite)

Exemplo de matriz:

|ID|Requisito|Fonte|Prioridade|Critério de aceite|Caso de teste|Status|
|---|---|---|---|---|---|---|
|RF-014|Filtrar pedidos por status|Entrevista S04|Must|CA-014|CT-014|Aprovado|
|RF-031|Exportar relatório em PDF|Desk research|Should|CA-031|CT-031|Em análise|
|RNF-002|Resposta ≤ 2s|Benchmark|Must|CA-002|CT-002|Aprovado|
|RN-003|Aprovação p/ pedidos > R$10k|Compliance|Must|CA-018|CT-018|Aprovado|

Regra de ouro da rastreabilidade: nenhum requisito pode existir no DDR sem fonte e sem critério de aceite. Se aparecer um requisito "órfão" (sem fonte), ele volta para validação.

#### Critérios de aceite no formato Dado/Quando/Então

O formato mais usado na prática é o Gherkin (estilo BDD), porque ele já nasce testável:

> CA-014 — Filtrar pedidos por status
> 
> - Dado que estou autenticado como atendente e existe uma lista com pedidos de status variados
> - Quando seleciono o filtro "aberto"
> - Então a lista exibe somente pedidos com status "aberto"
> - E a atualização ocorre em até 2 segundos
> 
> Caso negativo:
> 
> - Dado que não há pedidos com o status selecionado
> - Quando aplico o filtro
> - Então o sistema exibe a mensagem "Nenhum pedido encontrado" com um botão para limpar o filtro

Perceba que cada critério tem caso feliz e caso de exceção. Requisito sem exceção descrita é requisito incompleto.

#### Vinculando aceite a teste

Cada critério de aceite deve apontar para um caso de teste (CT) explícito. Se não é possível escrever o caso de teste, o critério está ambíguo demais e precisa ser reescrito. Essa é uma técnica de auto-validação do DDR: o analista que não consegue imaginar como testar o requisito ainda não entendeu o requisito.

---

### BLOCO 5 — Revisão, validação e manutenção do DDR

#### Ciclo de revisão do DDR

O DDR passa por três camadas de revisão antes de ser aprovado:

1. Revisão técnica (time): devs, arquitetos e QA leem e marcam ambiguidades, lacunas e inconsistências. Pergunta-guia: "Dá para implementar e testar exatamente como está escrito?"
2. Revisão com stakeholders: o dono do negócio confirma que o documento reflete as necessidades reais — e não uma interpretação do analista. Pergunta-guia: "É isso mesmo que você precisa?"
3. Revisão com usuários (quando viável): protótipos e cenários validam se o entendimento se sustenta fora do papel. Pergunta-guia: "Faz sentido para quem usa no dia a dia?"

Só depois dessas três camadas o requisito ganha o status Aprovado.

#### Manutenção e mudança

Requisitos mudam. O DDR precisa absorver isso sem virar um caos. As regras práticas:

- Versionamento: cada alteração gera uma nova versão com histórico do que mudou, quem pediu e por quê.
- Análise de impacto: antes de aprovar uma mudança, identifique todos os requisitos, critérios e testes afetados (via matriz de rastreabilidade).
- Baseline: marque versões estáveis como linha de base. Mudanças a partir dali exigem aprovação formal.
- Status do requisito: mantenha o ciclo de vida explícito: _Proposto → Em análise → Aprovado → Implementado → Verificado → Obsoleto_.

Isso conecta o DDR diretamente ao fluxo completo de [[Gerenciamento e Mudanças]] e à tríade de [[Verificação, Validação e Aprovação]].

#### Ferramentas práticas

O professor reforça que a ferramenta importa menos que a disciplina. Algumas opções comuns:

|Ferramenta|Uso típico|Observação|
|---|---|---|
|Wiki corporativa (Confluence, Notion, Obsidian)|Documento formal + colaboração|Histórico de versão e comentários|
|Rastreador (Jira, Trello, Linear)|Vinculo requisito → história → teste|A rastreabilidade vira prática diária|
|Planilha compartilhada|Matriz de rastreabilidade em projetos simples|Simples, mas perde controle de versão|
|Ferramenta dedicada (Icescrum, Craft, Doors)|DDR completo com rastreabilidade rígida|Para projetos maiores/regulados|

---

## Conexões com as leituras

- [[Engenharia de Requisitos]] — o DDR é a etapa de especificação do fluxo (elicitacão → análise → especificação → validação → gerenciamento). Tudo que acontece antes alimenta o documento; tudo que acontece depois depende dele.
- [[Especificação e DDR]] — esta nota aprofunda a estrutura teórica; aqui o foco é o como fazer no dia a dia, com exemplos e checklists.
- [[Tipos de Requisitos]] — a classificação (funcional, não funcional, regra de negócio) define como cada bloco do DDR é redigido e identificado (`RF-`, `RNF-`, `RN-`).
- [[Levantamento de Requisitos]] — as técnicas de elicitação são as fontes da matriz de rastreabilidade. Sem levantar bem, não há o que especificar bem.
- [[Gerenciamento e Mudanças]] — o DDR é o objeto central do controle de mudanças: versionamento, baseline e análise de impacto existem para proteger o documento.
- [[Verificação, Validação e Aprovação]] — o DDR fornece os requisitos e critérios que são verificados (o documento está correto?), validados (o documento captura a necessidade?) e aprovados (o documento é a referência oficial?).

---

## Exemplos e aplicações

### Estudo de caso — "Sistema de pedidos da lanchonete"

Cenário simplificado para fixar o passo a passo:

Descoberta (antes do DDR):

- Entrevistas com atendentes revelaram que o maior gargalo é o tempo para localizar pedidos antigos.
- Observação mostrou que atendentes usam atalhos manuais (caderno) porque o sistema atual não filtra por status.
- Desk research indicou que concorrentes respondem à consulta em média 1,5s.

DDR (especificação):

1. RF-014 — Filtrar pedidos por status (Must, fonte: entrevista S04 + observação)
2. RF-015 — Buscar pedido por número e CPF (Must, fonte: entrevista S02)
3. RNF-002 — Consulta de pedidos com resposta ≤ 2s para 10.000 registros (Must, fonte: benchmark)
4. RN-003 — Pedidos > R$ 200 exigem confirmação do cliente por telefone (Must, fonte: política da empresa)

Critérios de aceite:

- CA-014 (Dado/Quando/Então para o filtro)
- CA-015 (busca por número/CPF com caso negativo)
- CA-002 (teste de carga com 10.000 registros)
- CA-018 (fluxo de aprovação do pedido > R$ 200)

Rastreabilidade:

|ID|Fonte|Prioridade|Aceite|Teste|
|---|---|---|---|---|
|RF-014|Entrevista S04|Must|CA-014|CT-014|
|RF-015|Entrevista S02|Must|CA-015|CT-015|
|RNF-002|Benchmark|Must|CA-002|CT-002|
|RN-003|Política interna|Must|CA-018|CT-018|

Validação: protótipo do filtro testado com 3 atendentes — 100% concluíram a tarefa em < 1 minuto, confirmando o entendimento do RF-014.

---

### Checklist prático — "O DDR está pronto?"

Antes de considerar o DDR aprovado, verifique:

- [ ]  Todo requisito tem ID único, fonte e prioridade
- [ ]  Nenhum requisito mistura duas ideias em uma frase
- [ ]  RNFs usam medidas, não adjetivos vagos
- [ ]  Toda regra de negócio está rastreada aos requisitos que ela condiciona
- [ ]  Todo requisito tem critério de aceite escrito (Dado/Quando/Então, com exceção)
- [ ]  Todo critério de aceite tem caso de teste vinculado
- [ ]  A matriz de rastreabilidade está completa e sem "órfãos"
- [ ]  Glossário cobre os termos do domínio usados no documento
- [ ]  O documento tem versão, data e responsáveis identificados
- [ ]  Passou pelas três camadas de revisão (técnica, stakeholders, usuários)

---

## Dúvidas para revisar

- [ ]  Qual a diferença prática entre fonte de requisito e rastreabilidade — são a mesma coisa ou coisas distintas?
- [ ]  Quando um requisito muda, reutilizo o mesmo ID com nova versão ou crio um ID novo? Por que isso importa?
- [ ]  Um critério de aceite pode existir sem caso de teste? Em que situação?
- [ ]  Requisito "Would" (MoSCoW) deve ganhar aceite e rastreabilidade desde o início ou só quando for priorizado para implementação?
- [ ]  Na matriz de rastreabilidade, o que fazer quando o teste falha — o requisito muda, o teste muda ou o entendimento muda?
- [ ]  Qual a diferença entre aprovação de requisito (no DDR) e aprovação de sistema (homologação)? Elas podem acontecer em momentos diferentes?

---

## Aprendizados

- O DDR não se escreve "do zero" no fim — nasce durante o levantamento e amadurece com a análise.
- ID de requisito é âncora: nunca renumere, apenas versione.
- Requisito sem fonte é suposição; requisito sem aceite é intenção; requisito sem teste é opinião.
- RNF vago é armadilha: "rápido" não é testável, "≤ 2s para 10.000 registros" é.
- Critérios de aceite antes do desenvolvimento transformam o DDR em contrato testável, não em papel decorativo.
- A matriz de rastreabilidade é o coração do DDR — ela conecta descoberta, especificação, implementação e teste.
- Revisar em três camadas (técnica, stakeholders, usuários) reduz drasticamente o retrabalho.
- Ferramentas ajudam, mas disciplina de rastreabilidade e versionamento é o que sustenta o documento no longo prazo.

---

## Próximos passos

- [ ]  Praticar: escrever 5 RFs completos (ID, ator, ação, objeto, critério, fonte, aceite) para um sistema simples
- [ ]  Converter 3 adjetivos vagos em RNFs mensuráveis
- [ ]  Montar uma matriz de rastreabilidade para esses requisitos
- [ ]  Escrever critérios de aceite em Gherkin (feliz + exceção) para cada RF
- [ ]  Revisar em dupla (técnica) e ajustar ambiguidades encontradas
- [ ]  Reler as notas [[Especificação e DDR]] e [[Gerenciamento e Mudanças]] em perspectiva prática

---

## Referências

- [[Engenharia de Requisitos]]
- [[Especificação e DDR]]
- [[Tipos de Requisitos]]
- [[Levantamento de Requisitos]]
- [[Entrevistas]]
- [[Observação]]
- [[Desk Research]]
- [[Matriz CSD]]
- [[Persona]]
- [[Jobs to be Done]]
- [[Técnicas de Priorização]]
- [[Gerenciamento e Mudanças]]
- [[Verificação, Validação e Aprovação]]