tipo: aula curso: Pós-Graduação em Desenvolvimento de Software Full Stack disciplina: UI/UX e desenvolvimento centrado no usuário data: 2026-11-02 fontes:

- "[[Desenvolvimento de Software Centrado no Usuário]]"
- "[[Descoberta de Sistemas]]" tags:
- aula
- estudo
- ux
- card-sorting
- arquitetura-da-informacao
- analise
- discovery

---

# Card Sorting

## Resumo

Card Sorting é uma técnica de pesquisa que investiga como as pessoas agrupam e rotulam informações. Os participantes recebem cartões — físicos ou digitais — com nomes de conteúdos, funcionalidades ou tópicos e os organizam em categorias que fazem sentido para eles. O resultado revela o modelo mental dos usuários: as associações que eles consideram naturais, os rótulos que esperam encontrar e a estrutura que lhes parece lógica. É uma ferramenta central para apoiar decisões de arquitetura da informação, como menus, navegação e agrupamentos de funcionalidades. Na descoberta e no design centrado no usuário, o Card Sorting transforma suposições da equipe sobre a organização do sistema em evidência vinda diretamente dos usuários.

## Conceitos principais

- Card Sorting: técnica em que os participantes agrupam e rotulam cartões com conteúdos ou funcionalidades, revelando como organizam mentalmente as informações.
- Card Sorting aberto: os participantes criam os próprios grupos e dão nomes às categorias livremente — útil para descobrir novos agrupamentos e rótulos.
- Card Sorting fechado: as categorias são definidas antecipadamente e os participantes apenas distribuem os cartões entre elas — útil para validar uma estrutura já proposta.
- Card Sorting híbrido: combina os dois formatos, permitindo criar novos grupos além dos predefinidos ou reorganizar os existentes.
- Modelo mental: a forma como o usuário entende e organiza o domínio, que orienta as associações que ele considera naturais.
- Arquitetura da informação: a estrutura que define como o conteúdo é organizado, nomeado e navegado no produto.

## Conteúdo da aula

### Entender como o usuário organiza o mundo

A equipe costuma organizar o sistema pela lógica interna do negócio — por áreas, processos ou módulos. O usuário, porém, pensa a partir das suas tarefas e do seu vocabulário. O Card Sorting expõe essa diferença: mostra como o público agrupa as informações e que nomes usaria para cada grupo. A técnica é simples de aplicar, mas gera insumos muito concretos para estruturar menus e fluxos.

### Tipos de Card Sorting

- Aberto: o participante cria os grupos e nomeia cada categoria. É o formato exploratório, ideal para descobrir como as pessoas veem o domínio quando não há uma estrutura pronta.
- Fechado: a equipe define as categorias e o participante apenas classifica os cartões. É o formato de validação, útil para testar se uma proposta de navegação faz sentido para o usuário.
- Híbrido: parte de categorias predefinidas, mas permite criar novas ou reorganizar. Combina descoberta e validação.

### Como conduzir

1. Selecionar os cartões: listar conteúdos, funcionalidades ou tópicos representativos — na quantidade certa para não cansar o participante (em geral entre 30 e 60 itens).
2. Escolher o formato: aberto, fechado ou híbrido, conforme a pergunta do projeto.
3. Recrutar participantes: priorizar pessoas do público-alvo, buscando diversidade de perfis.
4. Aplicar a sessão: pedir que agrupem os cartões e, no formato aberto, que deem um nome a cada grupo — observando o raciocínio e registrando comentários.
5. Analisar os resultados: identificar padrões de agrupamento, comparar rótulos usados e, quando houver, observar consensos e divergências.

### Análise dos resultados

A análise busca padrões: cartões frequentemente colocados juntos sugerem uma relação forte; rótulos recorrentes indicam a terminologia que o usuário espera. Ferramentas digitais produzem uma matriz de similaridade e representações como o dendrograma, que mostram visualmente os agrupamentos dominantes. O resultado alimenta decisões de navegação, taxonomia e agrupamento de funcionalidades — e ajuda a substituir rótulos internos por termos compreendidos pelos usuários.

### Card Sorting na descoberta

Na fase de análise e síntese da descoberta, o Card Sorting transforma dúvidas e suposições da Matriz CSD em evidência sobre a organização esperada pelo usuário. Enquanto entrevistas e observação aprofundam tarefas e dores, o Card Sorting atua na estrutura e no vocabulário: como agrupar e como nomear aquilo que o produto entrega. Os achados podem revelar tanto confirmações — categorias que os usuários reproduzem naturalmente — quanto surpresas — termos internos que ninguém entende ou conteúdos que os usuários agrupam de forma imprevista.

## Conexões com as leituras

- Descoberta de Sistemas: situa o Card Sorting entre as técnicas de pesquisa e análise que apoiam a definição da arquitetura da informação, conectando o entendimento do usuário às decisões de organização e navegação do sistema.
- Desenvolvimento de Software Centrado no Usuário: posiciona o Card Sorting como método centrado no usuário no processo b_thinking, em que a organização do conteúdo deve espelhar o modelo mental do usuário e não apenas a estrutura interna do negócio.

## Exemplos e aplicações

- Definir o menu de navegação principal de um site ou aplicativo a partir dos agrupamentos feitos pelos usuários.
- Testar uma taxonomia existente com um Card Sorting fechado, verificando se os usuários encontram cada conteúdo na categoria esperada.
- Renomear categorias de menu usando os rótulos que os participantes criaram espontaneamente.
- Aplicar um Card Sorting aberto no início de um redesign para descobrir como o público organiza o domínio antes de propor qualquer estrutura.
- Consolidar os resultados do Card Sorting na Matriz CSD, convertendo suposições sobre a navegação em certezas ou novas dúvidas.

## Dúvidas para revisar

- [ ]  Como escolher a quantidade ideal de cartões sem cansar o participante?
- [ ]  Quando usar Card Sorting aberto, fechado ou híbrido em cada fase do projeto?
- [ ]  Como tratar os resultados quando não há consenso claro entre os participantes?
- [ ]  Qual a relação entre o Card Sorting e outras técnicas de arquitetura da informação, como o teste de árvore?

## Aprendizados

- Card Sorting revela como os usuários agrupam e rotulam informações — o modelo mental deles.
- Os formatos aberto, fechado e híbrido atendem a perguntas diferentes: explorar, validar ou combinar.
- A análise busca padrões de agrupamento e rótulos recorrentes, que orientam a arquitetura da informação.
- Conecta a compreensão do usuário às decisões de navegação e taxonomia do produto.
- Os achados alimentam a Matriz CSD, transformando suposições sobre organização em evidência.

## Próximos passos

- [ ]  Selecionar os conteúdos ou funcionalidades que serão os cartões da sessão.
- [ ]  Definir o formato de Card Sorting (aberto, fechado ou híbrido) conforme a pergunta do projeto.
- [ ]  Recrutar participantes do público-alvo e conduzir as sessões.
- [ ]  Analisar os padrões de agrupamento e rótulos para propor a arquitetura da informação.
- [ ]  Registrar os achados na Matriz CSD e nas decisões de navegação do projeto.

## Referências

- WAZLAWICK, Raul Sidnei; SANTOS, Ranieri Alves dos; HAMMES, Jades Fernando; CUNHA, Célio Luiz. _Desenvolvimento de Software Centrado no Usuário: Construindo produtos com b_thinking, UX e Agile_. UFSC, 2025.
- SANTOS, Ranieri Alves dos; PEREIRA, Nelma Rodrigues. _Descoberta de Sistemas: uma abordagem para engenharia_. Waiata Multimídia, 2025.