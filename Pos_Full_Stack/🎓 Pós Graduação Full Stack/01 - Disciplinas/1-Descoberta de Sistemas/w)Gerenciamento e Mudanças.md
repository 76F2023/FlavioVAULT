tipo: aula curso: Pós-Graduação em Desenvolvimento de Software Full Stack disciplina: data: fontes:

- "[[Desenvolvimento de Software Centrado no Usuário]]"
- "[[Descoberta de Sistemas]]"
- "[[Engenharia de Requisitos]]" tags:
- aula
- estudo

---

# Gerenciamento e Mudanças

## Resumo

Requisitos mudam o tempo todo — a descoberta amadurece, o negócio evolui e o usuário ensina. O gerenciamento é a etapa contínua da Engenharia de Requisitos que controla versões, mudanças, rastreabilidade e comunicação, garantindo que cada alteração seja avaliada, registrada e refletida em todo o projeto sem virar caos.

## Conceitos principais

- Linha de base (baseline): versão oficial de um conjunto de requisitos aprovado, a partir do qual as mudanças passam a ser controladas.
- Rastreabilidade: vínculo entre requisito, origem (stakeholder, entrevista, técnica) e artefatos derivados (testes, código, casos de uso).
- Controle de mudanças: processo formal para solicitar, avaliar, aprovar/rejeitar e registrar alterações.
- Análise de impacto: entender o que muda (custo, prazo, escopo, outros requisitos) antes de aprovar.
- Versionamento: histórico de alterações com autor, data e justificativa.

## Conteúdo da aula

### Por que gerenciar?

- Mudanças não são inimigas — são inevitáveis e, muitas vezes, melhoram o produto.
- O problema é a mudança não controlada: requisito alterado sem registro vira retrabalho, teste quebrado e decisão perdida.
- O objetivo é decisão consciente e rastreável, não rigidez.

### O fluxo de uma mudança

1. Solicitação — alguém identifica necessidade e registra o pedido (posição, expectativa, justificativa).
2. Comitê de controle de mudanças (CCB) — grupo que avalia a solicitação com critérios claros.
3. Análise de impacto — o que afeta: requisitos dependentes, esforço, prazo, risco, custo.
4. Decisão — aprovar, rejeitar ou adiar, com justificativa registrada.
5. Implementação — atualizar requisito, baseline e artefatos vinculados.
6. Comunicação — avisar stakeholders, equipe e documentação afetada.

### Rastreabilidade na prática

- Cada requisito precisa de origem (de onde veio) e destino (para onde vai).
- Matriz de rastreabilidade: requisito → fonte → teste → código → status.
- Sem rastreabilidade, não dá para medir impacto de uma mudança.

### Versionamento

- Toda alteração gera nova versão do documento de requisitos (ex.: DDR v1.1).
- Registro de mudanças: o que mudou, por quê, quem aprovou e quando.
- Baseline + mudanças controladas = histórico confiável.

### Ferramentas

- Rastreadores de requisitos (Jira, Azure DevOps, Trello estruturado).
- Wikis e documentos versionados (Obsidian, Notion, Confluence).
- Planilhas de matriz de rastreabilidade para projetos menores.
- Versionamento de código estendido a documentos (Git).

## Conexões com as leituras

- [[Engenharia de Requisitos]]: o gerenciamento é a 5ª etapa do fluxo — muda a visão de "documento pronto" para "requisito vivo".
- [[Levantamento de Requisitos]]: a origem de cada requisito alimenta a rastreabilidade.
- [[Especificação e DDR]]: o DDR é a linha de base; mudanças geram novas versões dele.
- [[Tipos de Requisitos]]: a classificação ajuda a prever impacto (não funcional de segurança, por exemplo, costuma ter impacto amplo).

## Exemplos e aplicações

- Mudança de regra de negócio: "pedido cancelado não pode ser reaberto" — análise de impacto descobre que afeta o fluxo de devolução e o relatório financeiro.
- Mudança de requisito não funcional: "carregar em 1s em vez de 3s" — impacta infraestrutura, arquitetura e custo.
- Matriz de rastreabilidade ligando uma entrevista à validação de um requisito funcional.

## Dúvidas para revisar

- [ ]  Diferença entre controle de mudanças e rigidez no escopo.
- [ ]  Como decidir o que é "mudança formal" vs. "ajuste simples".
- [ ]  Quem participa do CCB e com que periodicidade?

## Aprendizados

- Gerenciar mudanças é proteger a decisão, não impedir a evolução.
- Baseline e rastreabilidade são a base para qualquer análise de impacto.
- Comunicação é parte do processo — mudança aprovada sem aviso vira problema.

## Próximos passos

- [ ]  Montar um modelo de solicitação de mudança (formulário simples).
- [ ]  Criar uma matriz de rastreabilidade a partir das notas de levantamento.
- [ ]  Revisar o DDR e marcar os requisitos com prioridade e origem.

## Referências

- [[Engenharia de Requisitos]]
- [[Especificação e DDR]]
- [[Levantamento de Requisitos]]