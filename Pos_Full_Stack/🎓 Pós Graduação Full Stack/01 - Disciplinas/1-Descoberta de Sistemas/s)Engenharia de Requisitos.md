tipo: aula curso: Pós-Graduação em Desenvolvimento de Software Full Stack disciplina: Descoberta de Sistemas data: 2026-11-04 fontes:

- "[[Descoberta de Sistemas]]"
- "[[Desenvolvimento de Software Centrado no Usuário]]" tags:
- aula
- modulo-4
- requisitos

---

# Engenharia de Requisitos

## Resumo

Engenharia de Requisitos é o processo de descobrir, documentar, analisar e validar as necessidades e restrições de um sistema antes de construí-lo. Na Descoberta de Sistemas, ela transforma achados qualitativos — entrevistas, observação, Matriz CSD, personas — em uma base de decisão clara, mensurável e rastreável.

## Conceitos principais

- Requisito: uma condição ou capacidade que o sistema deve atender; expressa uma necessidade do usuário ou uma restrição do contexto.
- Requisito funcional: o que o sistema deve fazer — ações, comportamentos e fluxos.
- Requisito não funcional: qualidades e restrições — desempenho, segurança, usabilidade, disponibilidade, compatibilidade.
- Stakeholder: qualquer pessoa com interesse ou influência sobre o sistema (usuários, clientes, equipe, áreas de negócio).
- Escopo: fronteira entre o que está dentro e fora do sistema; evita requisitos impossíveis e retrabalho.

## Conteúdo da aula

### 1. Onde a Engenharia de Requisitos entra na descoberta

A Descoberta de Sistemas alimenta a Engenharia de Requisitos: os dados levantados viram hipóteses que, depois de validadas, são formalizadas como requisitos.

Fluxo típico:

1. Elicitação — levantar necessidades e restrições com técnicas de descoberta.
2. Análise — organizar, priorizar e resolver inconsistências.
3. Especificação — documentar de forma clara, mensurável e rastreável.
4. Validação — confirmar com stakeholders e usuários que o requisito reflete a necessidade real.
5. Gerenciamento — controlar mudanças, versões e rastreabilidade ao longo do projeto.

### 2. Elicitação de requisitos na prática

- Entrevistas → perguntas abertas, contexto e dor real.
- Observação → como o usuário executa a tarefa hoje, sem idealizações.
- Desk research → documentação, métricas e soluções concorrentes.
- Personas e Jobs to be Done → quem é o usuário e qual "trabalho" ele precisa concluir.
- Matriz CSD → separar certezas, suposições e dúvidas; requisito que nasce de suposição vira hipótese a validar.
- Prototipação e testes → validar a compreensão antes de especificar demais.

### 3. Classificação dos requisitos

- Funcionais (o que o sistema faz):
    - O sistema deve permitir criar um pedido de compra.
    - O usuário deve conseguir recuperar a senha por e-mail.
- Não funcionais (como o sistema é):
    - O tempo de resposta da busca deve ser inferior a 2 segundos.
    - Os dados de pagamento devem ser criptografados em trânsito.
    - A interface deve ser acessível conforme WCAG nível AA.
- Regras de negócio: restrições da organização. Ex.: somente gerente pode aprovar pedido acima de R$ 5.000.

### 4. Boas práticas ao escrever requisitos

- Um requisito por frase.
- Formato: ator + ação + objeto + condição/critério de aceite.
- Evitar ambiguidade: "rápido", "fácil" e "adequado" devem virar medidas.
- Manter rastreabilidade: cada requisito tem origem — usuário, hipótese, norma ou benchmarking.
- Priorizar antes de detalhar demais, com MoSCoW, Impacto × Esforço ou RICE.

Exemplo:

> O cliente deve conseguir filtrar os pedidos por status, com o resultado exibido em até 1,5 segundos, em uma lista clicável que leva ao detalhe do pedido.

### 5. Validação e mudança

- Valide com o usuário real: protótipo, teste de cenário, revisão de especificação.
- Requisitos mudam; mantenha versão e rastreabilidade.
- Distinga requisito do usuário (problema/necessidade) de requisito de sistema (solução técnica).

## Conexões com as leituras

- [[Entrevistas]] — a elicitação depende de boas perguntas e escuta ativa.
- [[Observação]] — revela requisitos que o usuário não verbaliza.
- [[Persona]] e [[Jobs to be Done]] — dão identidade e propósito aos requisitos.
- [[Matriz CSD]] — transforma suposições em hipóteses de requisito para validar.
- [[Técnicas de Priorização]] — ordenam os requisitos antes da especificação detalhada.

## Exemplos e aplicações

- Aplicativo de delivery: funcionais — buscar restaurantes, montar carrinho, acompanhar pedido; não funcionais — disponibilidade de 99,9%, carregamento em menos de 3 segundos, conformidade com LGPD.
- Sistema interno de RH: regra de negócio — aprovação de férias com alçada do gestor imediato.

## Dúvidas para revisar

- [ ]  Como diferenciar regra de negócio de requisito funcional em casos limítrofes?
- [ ]  Em que momento da descoberta "congelar" um requisito antes de prototipar?
- [ ]  Como priorizar requisitos não funcionais que parecem invisíveis ao usuário?

## Aprendizados

- Requisito bom nasce de necessidade validada, não de opinião interna.
- A Engenharia de Requisitos dá ordem à descoberta: sem rastreabilidade, o achado se perde.
- Requisito não funcional ignorado costuma virar dívida técnica e frustração do usuário.

## Próximos passos

- [ ]  Revisar a nota de [[Técnicas de Priorização]] para aplicar aos requisitos do caso.
- [ ]  Praticar a escrita de 5 requisitos funcionais e 3 não funcionais a partir de uma entrevista real.
- [ ]  Reler a [[Matriz CSD]] e transformar suposições em hipóteses de requisito.

## Referências

-  [[Descoberta de Sistemas]] — disciplina do Módulo 4 que contextualiza o processo de descoberta.
- [[Desenvolvimento de Software Centrado no Usuário]] — base conceitual do design centrado no usuário aplicado à descoberta.
- [[Entrevistas]] — técnica primária de elicitação; fonte da maioria das necessidades e dores.
- [[Observação]] — revela requisitos implícitos que o usuário não verbaliza.
- [[Persona]] — define para quem o requisito é escrito e qual contexto considerar.
- [[Jobs to be Done]] — conecta cada requisito a um "trabalho" real que o usuário precisa concluir.
- [[Matriz CSD]] — origem da rastreabilidade: certezas e suposições viram requisitos e hipóteses a validar.
- [[Técnicas de Priorização]] — MoSCoW, Impacto × Esforço, RICE e Kano aplicados à ordenação dos requisitos.