tipo: aula curso: Pós-Graduação em Desenvolvimento de Software Full Stack disciplina: data: 2026-11-04 fontes:

- "[[DDR na Prática]]"
- "[[Especificação e DDR]]"
- "[[Tipos de Requisitos]]"
- "[[Levantamento de Requisitos]]"
- "[[Engenharia de Requisitos]]" tags:
- aula
- estudo
- ia
- requisitos
- ddr

---

# DDR com Inteligência Artificial

## Resumo

A Inteligência Artificial entrou no fluxo da Engenharia de Requisitos como aceleradora e revisora do Documento de Definição de Requisitos (DDR). Ela não substitui o engenheiro de requisitos, mas transforma o trabalho: ajuda a transformar achados brutos de descoberta em requisitos candidatos, identifica ambiguidades, sugere critérios de aceite, aponta inconsistências e gera cenários de teste. O valor está em usar a IA como par de revisão, não como autor definitivo — todo conteúdo gerado precisa ser validado por humanos e rastreado até sua fonte.

## Conceitos principais

- DDR (Documento de Definição de Requisitos): artefato vivo que especifica requisitos funcionais, não funcionais e regras de negócio, com rastreabilidade e critérios de aceite.
- IA generativa: modelos treinados para gerar texto, que podem transformar insumos estruturados em esboços de requisitos.
- IA como copiloto: apoio em tarefas mecânicas e analíticas, mantendo a decisão final com o time de requisitos.
- Prompt engineering: arte de construir comandos claros com contexto, papel, formato e exemplos para obter respostas úteis.
- Validação humana no loop (_human-in-the-loop_): toda saída da IA passa por revisão crítica antes de entrar no DDR.

## Onde a IA entra no ciclo do DDR

O DDR segue o ciclo visto em [[DDR na Prática]]: levantamento → candidato → priorização → especificação → rastreabilidade → revisão → manutenção. A IA atua em cada etapa:

|Etapa do DDR|Papel da IA|Resultado esperado|
|---|---|---|
|Levantamento|Sintetizar entrevistas, atas e observações em temas e demandas candidatas|Reduzir o tempo de consolidação|
|Análise|Detectar duplicidades, lacunas e contradições entre achados|Matriz CSD mais precisa|
|Especificação|Gerar rascunhos de RFs, RNFs e RNs no formato padrão|Esboço inicial mais rápido|
|Critérios de aceite|Sugerir cenários em Gherkin (Dado/Quando/Então/E)|Cobertura de casos felizes e negativos|
|Rastreabilidade|Cruzar requisitos com fontes, personas e JTBD|Menos requisitos órfãos|
|Revisão|Apontar ambiguidades, adjetivos vagos e erros de consistência|Documento mais objetivo|
|Manutenção|Analisar impacto de mudanças e sugerir renumeração/versionamento|Menos retrabalho|

## Como extrair valor real da IA — blocos práticos

### Bloco 1 — Preparação do insumo

A IA só é boa se o contexto for bom. Regra de ouro: nunca peça requisito sem entregar contexto.

- Alimente com personas, JTBD, achados de entrevistas, observações, desk research e regras de negócio conhecidas.
- Use a [[Matriz CSD]] para separar o que é certeza, suposição e dúvida — a IA deve declarar suposições, não disfarçá-las de requisito.
- Peça que a IA identifique o que está faltando antes de gerar requisitos: "quais perguntas ainda não foram respondidas?"

Prompt de exemplo (preparação):

> Você é analista de requisitos em um produto de e-commerce. Abaixo estão achados de descoberta. Liste os temas candidatos a requisito, classifique cada trecho como Certeza, Suposição ou Dúvida e aponte três lacunas no material.

### Bloco 2 — Geração de requisitos funcionais

A IA ajuda a escrever no formato canônico, mas o engenheiro valida cada um.

- Padrão: ID + título + ator + ação + objeto + condição + prioridade + fonte + aceite.
- Regra de ouro: ATOR + AÇÃO + OBJETO + CRITÉRIO MENSURÁVEL.
- Peça um requisito por frase, sem "e" ligando ações diferentes.
- Solicite que a IA proponha priorização inicial (MoSCoW ou RICE) e justifique.

Prompt de exemplo (RF):

> Com base nos achados abaixo, gere 5 requisitos funcionais no formato: RF-XXX | título | ator | ação | objeto | condição | prioridade (MoSCoW). Não misture duas ações no mesmo requisito. Para cada um, indique a fonte (trecho do achado).

Cuidado crítico: a IA tende a inventar requisitos "plausíveis" sem fonte. Exija sempre o vínculo com o insumo original — requisito sem fonte não entra no DDR.

### Bloco 3 — RNFs e regras de negócio

- A IA ajuda a converter adjetivos vagos em métricas: "rápido" → "≤ 2s para 10.000 registros".
- Para cada RNF, peça critério mensurável + como será verificado.
- Regra de negócio deve ser separada de requisito do sistema: peça que a IA identifique "limites organizacionais" vs "comportamento do sistema".

Prompt de exemplo (RNF/RN):

> Transforme os requisitos abaixo em não funcionais mensuráveis. Para cada adjetivo vago, proponha uma métrica concreta e o método de verificação. Separe também as regras de negócio das funcionalidades do sistema.

### Bloco 4 — Critérios de aceite e rastreabilidade

- A IA é excelente em gerar Gherkin, mas precisa de contexto sobre ator e regra.
- Peça sempre caso feliz + caso negativo + caso de exceção.
- Monte a matriz com: ID · requisito · fonte · prioridade · aceite · caso de teste · status.
- Use a IA para detectar órfãos — requisitos sem fonte ou sem aceite.

Prompt de exemplo (Gherkin):

> Para o requisito RF-014 (cancelamento de pedido antes da expedição), gere critérios de aceite em Gherkin cobrindo: caminho feliz, pedido já expedido, usuário sem permissão e pagamento estornado.

### Bloco 5 — Revisão e manutenção

- A IA atua como revisor adversarial: procure ambiguidade, inconsistência, requisitos duplicados e contradições entre RN e RF.
- Use para análise de impacto: "se a RN-002 mudar, quais RFs são afetados?"
- Na manutenção, a IA sugere a diferença entre versões e o histórico de mudanças, mas quem aprova é o dono do documento.

Prompt de exemplo (revisão):

> Revise o trecho abaixo como revisor de requisitos. Aponte: ambiguidades, adjetivos vagos, requisitos compostos, falta de aceite e inconsistências com as regras de negócio. Sugira a correção para cada ponto.

## Boas práticas no uso da IA

### O que FAZER

- Contexto primeiro: entregar personas, JTBD e achados antes de pedir qualquer requisito.
- Formato de saída definido: solicitar o padrão do DDR explicitamente (ID, título, ator, ação, aceite).
- Rastreabilidade obrigatória: exigir que toda saída cite a fonte de origem.
- Revisão humana sempre: a IA propõe, o time dispõe.
- Iteração com feedback: "o RF-002 está errado porque mistura duas ações; corrija seguindo o padrão."

### O que EVITAR

- Pedir requisito de "cadeira solta", sem insumo — a IA vai inventar (alucinação).
- Copiar e colar a saída direto no DDR sem revisão.
- Dar à IA a palavra final sobre priorização ou aprovação.
- Alimentar a ferramenta com dados sensíveis ou de clientes sem autorização.
- Confiar que a IA "lembra" todo o contexto anterior — reafirme os pontos essenciais no prompt.

## Limites e riscos da IA no DDR

- Alucinação: requisitos plausíveis, porém inexistentes nos achados.
- Viés de generalização: soluções genéricas que ignoram particularidades do domínio.
- Perda de rastreabilidade: a IA pode "suavizar" a origem de um requisito.
- Segurança e privacidade: não colocar dados confidenciais em ferramentas não autorizadas.
- Falsa confiança: texto fluente não é requisito correto; a forma impecável esconde conteúdo errado.

## Conexões com as leituras e notas

- [[DDR na Prática]] → a IA acelera exatamente os cinco blocos: preparação, RF, RNF/RN, rastreabilidade/aceite e revisão/manutenção.
- [[Especificação e DDR]] → a estrutura do documento é a mesma; a IA apenas ajuda a preencher com consistência.
- [[Tipos de Requisitos]] → a IA precisa da distinção entre RF, RNF e RN para não misturar categorias.
- [[Levantamento de Requisitos]] → a qualidade da IA depende da qualidade dos achados de entrevistas, observação e desk research.
- [[Engenharia de Requisitos]] → a IA não substitui o processo; ela o instrumenta.
- [[Verificação, Validação e Aprovação]] → a aprovação continua humana; a IA participa da verificação, não da aprovação.
- [[Gerenciamento e Mudanças]] → a IA pode apoiar a análise de impacto, mas baseline e versionamento seguem governança humana.

## Exemplos e aplicações

### Exemplo 1 — De achado bruto a requisito com ajuda da IA

Achado (entrevista): "O atendente reclama que não consegue filtrar os pedidos por status; hoje tem que rolar a lista inteira."

Prompt:

> Converta o achado abaixo em um requisito funcional no formato: ID, título, ator, ação, objeto, condição, prioridade, fonte. Declare suposições explicitamente.

Saída útil da IA (após revisão humana):

> RF-031 — Filtrar pedidos por status · Ator: atendente autenticado · Ação: filtra a lista de pedidos · Objeto: por status · Condição: resultado exibido em até 2 segundos · Prioridade: Must · Fonte: Entrevista 03.

### Exemplo 2 — RNF mensurável

Trecho vago: "O sistema precisa ser rápido."

Prompt:

> Transforme 'o sistema precisa ser rápido' em um RNF mensurável com método de verificação.

Saída útil:

> RNF-003 — Desempenho · A listagem de até 10.000 registros deve retornar em ≤ 2 segundos. Verificação: teste de carga com 10.000 registros.

## Dúvidas para revisar

- [ ]  O que diferencia um prompt eficaz de um prompt genérico no contexto de requisitos?
- [ ]  Como detectar alucinação em saídas de IA no DDR?
- [ ]  Quais dados não podem, em hipótese alguma, ir para uma ferramenta de IA externa?
- [ ]  Em que etapa do ciclo do DDR a IA agrega mais valor e em qual agrega mais risco?
- [ ]  A IA pode participar da aprovação de um requirement? Por quê?

## Aprendizados

- IA no DDR é multiplicador de produtividade, não substituto de responsabilidade.
- A qualidade da saída é limitada pela qualidade do contexto de entrada.
- Toda saída precisa de fonte, aceite e revisão humana antes de entrar no documento.
- Prompt bem estruturado = contexto + papel + formato + exemplo + restrição.
- O engenheiro de requisitos continua responsável por: decidir, priorizar, validar e aprovar.

## Próximos passos

- [ ]  Testar um prompt de geração de RF com os achados reais da disciplina
- [ ]  Revisar uma saída de IA apontando as alucinações encontradas
- [ ]  Comparar uma especificação escrita "na mão" com uma gerada por IA (pontos fortes e fracos)
- [ ]  Adicionar à matriz de rastreabilidade a coluna "gerado por IA? revisado por?"