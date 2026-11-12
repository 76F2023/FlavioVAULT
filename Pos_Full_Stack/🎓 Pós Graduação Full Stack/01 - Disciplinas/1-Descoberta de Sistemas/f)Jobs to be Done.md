tipo: aula curso: Pós-Graduação em Desenvolvimento de Software Full Stack disciplina: UI/UX e desenvolvimento centrado no usuário data: 2026-11-01 fontes:

- "[[Desenvolvimento de Software Centrado no Usuário]]"
- "[[Descoberta de Sistemas]]" tags:
- aula
- estudo
- ux
- jtbd
- discovery
- descoberta

---

# Jobs to be Done

## Resumo

Jobs to be Done (JTBD) é uma lente de pesquisa que muda o foco do produto para o trabalho que o usuário quer realizar. Em vez de perguntar "o que você quer no sistema?", a equipe procura entender qual "job" a pessoa está tentando fazer — a tarefa funcional que precisa cumprir, somada às dimensões emocionais e sociais envolvidas. A ideia central é que as pessoas não compram ou usam um produto por ele mesmo: elas o "contratam" para progredir em uma situação concreta. No Discovery, o JTBD ajuda a compreender a necessidade por trás do pedido, evitando que a solução seja desenhada a partir de funcionalidades soltas.

## Conceitos principais

- Job (trabalho): aquilo que o usuário quer realizar em uma dada situação — o progresso que busca, não a funcionalidade que pede.
- Job funcional: a tarefa objetiva que precisa ser cumprida (ex.: "preciso registrar minhas despesas").
- Job emocional: como o usuário quer se sentir ao realizar a tarefa (ex.: "quero me sentir no controle das minhas finanças").
- Job social: como o usuário quer ser percebido pelos outros (ex.: "quero parecer organizado para minha equipe").
- Declaração de job (job statement): frase que sintetiza o trabalho no formato "quando [situação], quero [motivação], para [resultado esperado]".
- Contratar o produto: metáfora que expressa que o usuário escolhe uma solução para realizar um job específico, não pelo produto em si.
- Forças de progresso: fatores que puxam o usuário para a nova solução (pull), empurram para longe da situação atual (push) e os freios (ansiedade e hábito) que dificultam a mudança.
- Não é persona nem segmento demográfico: o JTBD foca na situação e na motivação, não em idade, gênero ou cargo.

## Conteúdo da aula

### O usuário não quer o produto, quer o progresso

A frase-símbolo do JTBD é: "as pessoas não querem uma furadeira de 8 mm, querem um furo de 8 mm na parede". O produto é apenas o meio; o que importa é o trabalho que ele permite realizar. No contexto de software, isso significa que usuários não pedem "uma tela de cadastro" — eles querem poder registrar um cliente rapidamente, sem retrabalho, em um momento de pressão.

### As três dimensões do job

Um job completo raramente é só funcional. Para compreendê-lo, observa-se:

- funcional — a tarefa objetiva;
- emocional — o sentimento que o usuário quer ter durante e depois;
- social — a imagem que ele quer projetar para os outros.

Ignorar as dimensões emocional e social é um erro comum: duas soluções podem cumprir a mesma função e, ainda assim, o usuário preferir a que o faz se sentir mais seguro ou mais competente diante do time.

### Declaração de job

Uma boa declaração de job segue o formato "quando [situação], quero [motivação], para [resultado]". Ela ajuda a equipe a alinhar o entendimento antes de propor solução. Exemplo: "quando estou fechando um pedido no fim do mês, quero conferir os dados em um só lugar, para não atrasar a entrega ao cliente".

### As forças de progresso

O modelo das forças ajuda a entender por que o usuário muda (ou não) de solução:

- push — o que incomoda na situação atual (a dor que empurra para longe);
- pull — o que atrai na nova solução (o ganho que puxa);
- ansiedade — o medo do novo (receio de errar, migrar, perder tempo);
- hábito — a inércia da forma atual de fazer (a força que mantém no lugar).

Uma solução só "cola" quando o push e o pull superam a ansiedade e o hábito.

### JTBD no Discovery

O JTBD complementa as técnicas de imersão: as entrevistas deixam de perguntar apenas "o que você faz?" e passam a investigar a situação, a motivação e o resultado buscado. As dúvidas da Matriz CSD ganham foco quando expressas como jobs, e os achados retroalimentam a matriz com novas certezas, suposições e dúvidas. O resultado é uma visão do problema centrada no progresso do usuário, não na lista de funcionalidades.

## Conexões com as leituras

- Descoberta de Sistemas — módulos de imersão: o JTBD dialoga com as técnicas de aproximação com o usuário, ajudando a transformar observações e relatos em declarações de trabalho que orientam a definição do problema.
- Desenvolvimento de Software Centrado no Usuário — capítulo 5: ao detalhar os métodos de pesquisa na descoberta do b_thinking, reforça a importância de compreender a necessidade real do usuário antes de desenhar soluções — mesmo princípio que sustenta o JTBD.

## Exemplos e aplicações

- Antes de listar funcionalidades, escrever a declaração de job de cada necessidade identificada.
- Em entrevistas, substituir "o que você quer no sistema?" por "qual era a última vez que você precisou…? O que estava tentando fazer?".
- Mapear, para cada job, as dimensões funcional, emocional e social — e não apenas a tarefa.
- Usar as forças de progresso para avaliar por que um usuário resiste a adotar uma solução.
- Consolidar os jobs identificados na Matriz CSD, separando o que já é certeza do que ainda precisa ser investigado.

## Dúvidas para revisar

- [ ]  Qual a diferença entre um job e uma simples tarefa ou funcionalidade?
- [ ]  Como distinguir job funcional, emocional e social na prática, durante uma entrevista?
- [ ]  Como transformar as dúvidas da Matriz CSD em declarações de job?
- [ ]  Quando vale a pena aplicar JTBD em vez de personas tradicionais?

## Aprendizados

- JTBD muda o foco do produto para o progresso que o usuário busca.
- Um job completo tem dimensões funcional, emocional e social.
- A declaração de job alinha o entendimento do problema antes da solução.
- As forças de progresso explicam por que o usuário muda — ou permanece na situação atual.
- JTBD fortalece entrevistas e Matriz CSD, evitando soluções centradas em funcionalidades soltas.

## Próximos passos

- [ ]  Reescrever as necessidades identificadas no briefing como declarações de job.
- [ ]  Incluir perguntas de JTBD no roteiro das próximas entrevistas.
- [ ]  Mapear as dimensões funcional, emocional e social de cada job identificado.
- [ ]  Consolidar os resultados na Matriz CSD.

## Referências

- WAZLAWICK, Raul Sidnei; SANTOS, Ranieri Alves dos; HAMMES, Jades Fernando; CUNHA, Célio Luiz. _Desenvolvimento de Software Centrado no Usuário: Construindo produtos com b_thinking, UX e Agile_. UFSC, 2025.
- SANTOS, Ranieri Alves dos; PEREIRA, Nelma Rodrigues. _Descoberta de Sistemas: uma abordagem para engenharia_. Waiata Multimídia, 2025.