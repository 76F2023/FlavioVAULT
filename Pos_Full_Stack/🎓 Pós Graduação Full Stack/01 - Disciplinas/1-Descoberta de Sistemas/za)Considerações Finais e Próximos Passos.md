tipo: aula curso: Pós-Graduação em Desenvolvimento de Software Full Stack disciplina: Desenvolvimento de Software Centrado no Usuário data: 2026-11-04 fontes:

- "[[Engenharia de Requisitos]]"
- "[[Levantamento de Requisitos]]"
- "[[Tipos de Requisitos]]"
- "[[Especificação e DDR]]"
- "[[DDR na Prática]]"
- "[[DDR com Inteligência Artificial]]"
- "[[Verificação, Validação e Aprovação]]"
- "[[Gerenciamento e Mudanças]]" tags:
- aula
- estudo
- síntese
- próximos-passos

---

# Considerações Finais e Próximos Passos

## Resumo

Encerramento do ciclo de descoberta e especificação de sistemas, com foco na consolidação do aprendizado e na transição da teoria para a prática profissional. A mensagem central: requisitos de qualidade nascem de um processo contínuo, rastreável e centrado no usuário — e o DDR é o instrumento que transforma descoberta em software testável.

## Conceitos principais

- Processo contínuo: descoberta e especificação não terminam no documento — evoluem com feedback, validação e mudanças controladas.
- Rastreabilidade como espinha dorsal: todo requisito nasce de uma fonte e termina em um critério de aceite e um caso de teste.
- Verificar ≠ Validar: verificação confere conformidade com a especificação; validação confere adequação à necessidade real do usuário.
- Aprovação é decisão de responsabilidade: envolve stakeholders, registra o aceite e estabelece a baseline.
- IA como multiplicador, não substituto: acelera e revisa, mas quem decide, prioriza e aprova é sempre o humano.

## Conteúdo da aula

### 1. O fio condutor da disciplina

Do primeiro contato com o problema até a entrega do documento de requisitos, percorremos um caminho que pode ser resumido em oito marcos:

|Etapa|Objetivo|Instrumento-chave|
|---|---|---|
|Engenharia de Requisitos|Estruturar o processo|Ciclo de vida e boas práticas|
|Levantamento|Descobrir necessidades|Entrevistas, observação, desk research|
|Análise|Organizar e priorizar|Personas, JTBD, Matriz CSD, priorização|
|Especificação|Formalizar requisitos|DDR: RF, RNF, RN|
|Rastreabilidade|Garantir origem e destino|Matriz de rastreabilidade|
|Verificação e Validação|Confirmar qualidade e utilidade|Revisões, testes, protótipos|
|Aprovação|Oficializar a baseline|Aceite formal dos stakeholders|
|Gerenciamento de Mudanças|Manter o documento vivo|Versionamento, análise de impacto|

Cada etapa alimenta a seguinte; nenhuma funciona isoladamente.

### 2. O que de fato diferencia um bom documento de requisitos

- Clareza e mensurabilidade: um requisito não medido é opinião, não requisito.
- Fonte declarada: elimina o "requisito órfão", produto de suposição.
- Critério de aceite em Gherkin: transforma intenção em teste executável.
- Priorização explícita: detalhar antes de priorizar é desperdício.
- Manutenção planejada: documento sem baseline vira ruído.

### 3. A visão integrada do ciclo

```
Descoberta → Análise → Especificação → Rastreabilidade → V&V → Aprovação → Manutenção      ↑                                                                      ↓      └────────────────────────── feedback contínuo ─────────────────────────┘
```

O ciclo não é linear: cada mudança reabre etapas anteriores, e a rastreabilidade é o que permite navegar entre elas com segurança.

### 4. Próximos passos na prática

Para aplicar imediatamente:

- Escolher um projeto real (ou simulado) e conduzir o ciclo completo, do levantamento à aprovação.
- Montar um DDR mínimo com 10 requisitos, todos com fonte, prioridade e aceite.
- Praticar escrita de cenários em Gherkin para os 3 requisitos mais críticos.

Para aprofundar:

- Estudar normas e modelos: IEEE 830, ISO/IEC 25010, CMMI, MPS.BR.
- Explorar ferramentas de rastreabilidade (Jira + Confluence, DOORS, CodeBeamer, Craft.io).
- Aplicar IA generativa em revisão de requisitos, sempre com validação humana.

Para a carreira:

- Construir um portfólio com um DDR comentado, mostrando decisões e trade-offs.
- Desenvolver habilidade de mediação entre negócio, UX e desenvolvimento.
- Tornar-se referência em qualidade de requisitos no time.

## Conexões com as leituras

- Engenharia de Requisitos: fornece o arcabouço teórico que sustenta todo o processo.
- Levantamento de Requisitos: a qualidade do DDR começa na qualidade da descoberta.
- Tipos de Requisitos: a taxonomia RF/RNF/RN evita confusão e retrabalho.
- DDR na Prática: o passo a passo operacional que materializa a teoria.
- DDR com IA: como acelerar etapas sem perder responsabilidade humana.
- Verificação, Validação e Aprovação: o filtro de qualidade antes do desenvolvimento.
- Gerenciamento e Mudanças: mantém o documento vivo e a baseline protegida.

## Exemplos e aplicações

Caso aplicado — Aplicativo de delivery:

1. Levantamento: entrevistas com entregadores e restaurantes revelam necessidade de "filtro por distância".
2. Análise: persona "Entregador Carlos" prioriza esse filtro como _Must_.
3. Especificação: `RF-014: O entregador autenticado filtra pedidos disponíveis por raio em km, com resposta em até 2s.`
4. Rastreabilidade: fonte = entrevista 3; critério de aceite = cenário Gherkin de filtro com raio mínimo e máximo.
5. Verificação: revisão técnica confirma formato e unicidade.
6. Validação: protótipo navegável testado com 5 entregadores reais.
7. Aprovação: stakeholder de operações aprova com assinatura digital e baseline v1.0.
8. Mudança: após feedback, raio máximo alterado de 15 km para 20 km — mudança registrada com análise de impacto e nova versão v1.1.

## Dúvidas para revisar

- [ ]  Qual a diferença prática entre baseline e versão corrente?
- [ ]  Como priorizar requisitos quando stakeholders discordam?
- [ ]  Quando um requisito deve ser removido em vez de modificado?
- [ ]  Como medir a qualidade de um DDR em números?
- [ ]  Até que ponto a IA pode participar da aprovação?

## Aprendizados

- Requisitos bem escritos são a base de todo o ciclo de desenvolvimento.
- Rastreabilidade é o seguro contra decisões arbitrárias.
- Validação com usuário real é insubstituível.
- Mudança é inevitável; o que muda é o custo de lidar com ela.
- Responsabilidade sobre requisitos é humana, não algorítmica.

## Próximos passos

- [ ]  Revisar todas as notas do curso e criar um mapa-mestre no Obsidian.
- [ ]  Aplicar o ciclo completo em um projeto pessoal.
- [ ]  Estudar duas normas (IEEE 830 e ISO/IEC 25010).
- [ ]  Criar um template de DDR no Obsidian com os campos padronizados.
- [ ]  Praticar 10 cenários Gherkin com casos negativos.
- [ ]  Compartilhar o DDR comentado com colegas para feedback.

## Referências

- [[Engenharia de Requisitos]]
- [[Levantamento de Requisitos]]
- [[Tipos de Requisitos]]
- [[Especificação e DDR]]
- [[DDR na Prática]]
- [[DDR com Inteligência Artificial]]
- [[Verificação, Validação e Aprovação]]
- [[Gerenciamento e Mudanças]]
