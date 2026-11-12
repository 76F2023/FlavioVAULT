tipo: aula curso: Pós-Graduação em Desenvolvimento de Software Full Stack disciplina: Descoberta de Sistemas data: 2026-11-04 fontes:

- "[[Desenvolvimento de Software Centrado no Usuário]]"
- "[[Descoberta de Sistemas]]"
- "[[Engenharia de Requisitos]]"
- "[[Especificação e DDR]]"
- "[[Gerenciamento e Mudanças]]" tags:
- aula
- estudo
- requisitos
- validacao
- verificacao

---

# Verificação, Validação e Aprovação

## Resumo

Etapa que encerra o ciclo de um requisito: verificar se ele foi construído corretamente, validar se atende à necessidade real do usuário e aprovar formalmente para liberar a entrega. São três atividades distintas e complementares.

## Conceitos principais

- Verificação: "Construímos o produto corretamente?" — conferência contra a especificação.
- Validação: "Construímos o produto certo?" — conferência contra a necessidade real.
- Aprovação: decisão formal do stakeholder autorizando a liberação do requisito/entrega.
- Critério de aceite: condição objetiva que liga verificação e validação — sem ele, nada fica "pronto".

## A tríade no processo

|Atividade|Pergunta-chave|Referência|Foco|
|---|---|---|---|
|Verificação|Está conforme o [[Especificação e DDR\|DDR]]?|Especificação|Conformidade técnica|
|Validação|Resolve a dor real do usuário?|Necessidade|Valor de negócio|
|Aprovação|O responsável aceita formalmente?|Governança|Decisão de liberação|

> Ordem lógica: verifica-se primeiro (contra o documento) e valida-se depois (contra o mundo real). Só então se aprova.

## Verificação na prática

- Compara entrega × requisito especificado.
- Técnicas comuns:
    - Revisão de código e inspeção de documentos.
    - Testes unitários, de integração e de sistema.
    - Análise estática e conferência de rastreabilidade.
- Saída: lista de não conformidades.

## Validação na prática

- Coloca o produto na mão do usuário real.
- Técnicas comuns:
    - Teste de aceite com [[Critérios de aceite|critérios de aceite]].
    - Protótipo navegável e testes de usabilidade.
    - Piloto, beta ou homologação em ambiente próximo do real.
- Saída: confirmação (ou não) de que a dor do usuário foi resolvida.

## Aprovação e responsabilidades

- Quem aprova é o stakeholder com autoridade (dono do produto, gestor, cliente).
- Não é "achismo": aprovação se apoia em evidências de verificação e validação.
- Deve ficar registrada — com data, responsável e versão aprovada.
- A aprovação alimenta o controle de mudanças em [[Gerenciamento e Mudanças]].

## Conexões com as outras notas

- [[Engenharia de Requisitos]]: validação é a 4ª etapa do fluxo.
- [[Especificação e DDR]]: o DDR guarda os critérios de aceite usados na validação.
- [[Tipos de Requisitos]]: requisito não funcional precisa de critério mensurável para ser verificável.
- [[Gerenciamento e Mudanças]]: a aprovação define a baseline liberada; mudanças posteriores passam por novo ciclo.

## Exemplos e aplicações

- Verificação: o relatório carrega em 1,8s com 10.000 registros — atende ao critério "≤ 2s" do DDR. ✅
- Validação: o usuário de testes encontra o filtro de status em menos de 30s e conclui a tarefa. ✅
- Aprovação: o Product Owner assina a liberação da versão 1.2 após revisar os resultados. ✅

## Dúvidas para revisar

- [ ]  Diferença entre "teste de verificação" e "teste de validação" com exemplos.
- [ ]  Quem deve assinar a aprovação em cada tipo de projeto?
- [ ]  Como registrar evidências de validação no DDR?

## Aprendizados

- Verificar e validar são coisas diferentes — e ambas são necessárias.
- Sem critério de aceite mensurável, nem verificação nem validação têm "fim".
- Aprovação é decisão formal, não opinião informal.
- A tríade fecha o ciclo de qualidade e alimenta o gerenciamento de mudanças.

## Próximos passos

- [ ]  Revisar o DDR do projeto aplicando os atributos de qualidade (verificável, rastreável).
- [ ]  Montar um checklist de aprovação para cada entrega.
- [ ]  Relacionar esta nota com [[Gerenciamento e Mudanças]] no grafo do Obsidian.

## Referências

- [[Engenharia de Requisitos]]
- [[Especificação e DDR]]
- [[Tipos de Requisitos]]
- [[Gerenciamento e Mudanças]]