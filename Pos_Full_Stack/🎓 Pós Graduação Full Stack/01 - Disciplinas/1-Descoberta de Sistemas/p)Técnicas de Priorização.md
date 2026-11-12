tipo: aula curso: Pós-Graduação em Desenvolvimento de Software Full Stack disciplina: UI/UX e desenvolvimento centrado no usuário data: 2026-11-02 fontes:

- "[[Desenvolvimento de Software Centrado no Usuário]]"
- "[[Descoberta de Sistemas]]" tags:
- aula
- estudo
- ux
- priorizacao
- moscow
- rice
- kano
- discovery

---

# Técnicas de Priorização

## Resumo

Técnicas de priorização são métodos estruturados usados para decidir, entre muitas possibilidades, o que merece atenção, esforço e investimento primeiro. Em contextos de descoberta e desenvolvimento centrado no usuário, a priorização aparece o tempo todo: escolher quais dúvidas investigar na Matriz CSD, quais ideias do Design Studio e do Crazy 8's levar adiante, quais funcionalidades prototipar e quais dores atacar. As principais técnicas — MoSCoW, Matriz Impacto × Esforço, RICE e Modelo Kano — ajudam a transformar o julgamento subjetivo em decisão comparável e defensável, alinhando o time em torno de critérios explícitos em vez de preferências individuais.

## Conceitos principais

- Priorização: decisão deliberada sobre quais itens têm maior valor relativo diante de recursos limitados.
- MoSCoW: classifica itens em Must-have (obrigatório), Should-have (importante, mas adiável), Could-have (desejável) e Won't-have (fora do escopo agora).
- Matriz Impacto × Esforço: cruza o valor potencial de uma iniciativa com o esforço para realizá-la, gerando quadrantes de decisão.
- RICE: pontuação numérica a partir de Reach (alcance), Impact (impacto), Confidence (confiança) e Effort (esforço).
- Modelo Kano: distingue atributos básicos, de desempenho e encantadores conforme o efeito que geram na satisfação do usuário.
- Critérios explícitos: a base de qualquer boa priorização, que impede que a decisão seja puro gosto ou política.

## Conteúdo da aula

### Por que priorizar

Equipes de produto sempre têm mais ideias do que capacidade de executar. Sem um critério claro, a discussão vira disputa de opiniões, e itens que "gritam mais" vencem os que de fato importam. Priorizar é escolher de forma transparente: definir critérios, comparar alternativas com eles e registrar a decisão para poder revisitá-la quando as condições mudarem.

### MoSCoW

- Must-have (obrigatório): sem isso, a solução não cumpre sua promessa básica. Se não couber, o escopo precisa encolher.
- Should-have (deveria ter): importante e valioso, mas a entrega sobrevive sem ele por um tempo.
- Could-have (poderia ter): desejável, agrega se sobrar espaço ou tempo.
- Won't-have (não terá por agora): explicitamente fora do escopo atual, o que é tão importante quanto escolher o que entra.

A força do MoSCoW não está só nos dois primeiros níveis, mas na honestidade de declarar o Won't-have — é isso que protege o time da sobrecarga e do escopo infinito.

### Matriz Impacto × Esforço

Cruza duas dimensões em quatro quadrantes:

- Quick wins (alto impacto, baixo esforço): fazer já.
- Grandes apostas (alto impacto, alto esforço): planejar com cuidado, dividir e validar antes de investir tudo.
- Tarefas secundárias (baixo impacto, baixo esforço): encaixar quando houver folga.
- Desperdício de tempo (baixo impacto, alto esforço): evitar.

É uma técnica visual e rápida, ótima para alinhar o time em uma sessão colaborativa, mas depende de estimativas honestas de impacto e esforço.

### RICE

Converte uma decisão em número único:

RICE=Reach×Impact×ConfidenceEffortRICE=EffortReach×Impact×Confidence​

- Reach: quantas pessoas são afetadas em um período.
- Impact: quanto muda a experiência (1 = pequeno, 3 = grande).
- Confidence: quão segura é a estimativa (percentual).
- Effort: tempo de trabalho necessário (pessoas × meses).

O RICE é útil quando há muitas iniciativas a comparar e se quer uma ordem clara e defensável. Seu limite é a quantidade de estimativa que exige — números ruins geram prioridades ruins.

### Modelo Kano

Classifica atributos pelo efeito na satisfação:

- Básicos (esperados): não encantam quando presentes, mas frustram profundamente quando ausentes.
- De desempenho: quanto mais, melhor — geram satisfação proporcional.
- Encantadores: não esperados; quando aparecem, surpreendem e diferenciam. Com o tempo, tendem a virar básicos.
- Indiferentes: não afetam a satisfação.
- Reversos: alguns usuários gostam, outros rejeitam.

Kano ajuda a decidir onde investir: cobrir os básicos primeiro, escolher onde competir nos de desempenho e reservar espaço para encantadores que diferenciam.

### Outros recursos

- Dot voting: cada participante distribui votos limitados entre opções; rápido para convergir em grupo.
- Value × Complexity: variação da matriz impacto × esforço, com foco no risco técnico.
- Ranking forçado: ordenar itens um contra o outro quando tudo parece importante.

### O lugar da priorização na descoberta

A descoberta gera um volume grande de incertezas, achados e ideias. A priorização decide o próximo passo:

- ordena as dúvidas e suposições da Matriz CSD por risco e relevância;
- seleciona as direções mais fortes do Design Studio e do Crazy 8's;
- escolhe quais funcionalidades do Canvas de Proposta de Valor merecem primeiro protótipo;
- equilibra fatos (chapéu branco), valor (chapéu amarelo) e riscos (chapéu preto) para decidir com rigor.

## Conexões com as leituras

- Descoberta de Sistemas — módulos de análise e decisão: a priorização fecha o ciclo da descoberta, transformando incertezas registradas na Matriz CSD em uma ordem de investigação e validação.
- Desenvolvimento de Software Centrado no Usuário: situa a priorização como etapa contínua do processo centrado no usuário, em que escolher o que construir é tão importante quanto construir bem, e toda decisão deve remeter ao valor para o usuário.

## Exemplos e aplicações

- Aplicar MoSCoW para separar o que é obrigatório no MVP do que pode esperar, declarando explicitamente o que não será feito agora.
- Usar a matriz Impacto × Esforço em uma reunião para classificar ideias vindas do Crazy 8's e escolher os quick wins.
- Calcular RICE para ordenar um backlog de funcionalidades quando as opções são muitas e comparáveis.
- Usar o Modelo Kano para descobrir que um item tratado como obrigatório é, na verdade, um encantador que pode ser adiado.
- Priorizar as dúvidas da Matriz CSD pelo risco de seguir sem respondê-las, começando pelas que bloqueiam as decisões maiores.

## Dúvidas para revisar

- [ ]  Como estimar Impact e Confidence no RICE sem dados históricos?
- [ ]  Qual a diferença prática entre um Must-have e um Should-have que o usuário considera essencial?
- [ ]  Quando o Modelo Kano é mais útil do que a matriz Impacto × Esforço?
- [ ]  Como evitar que a priorização vire apenas uma disputa de poder mascarada por critérios?
- [ ]  De que forma registrar a priorização para que ela possa ser revista sem retrabalho?

## Aprendizados

- Priorizar é uma decisão deliberada com critérios explícitos, não um acerto pessoal.
- MoSCoW protege o escopo ao declarar o que não será feito agora.
- A matriz Impacto × Esforço é rápida e visual, ideal para sessões colaborativas.
- RICE transforma comparação em número, útil quando há muitas iniciativas.
- O Modelo Kano revela que nem todo atributo tem o mesmo efeito na satisfação.
- A priorização aparece em todas as etapas da descoberta, da Matriz CSD à prototipagem.

## Próximos passos

- [ ]  Selecionar uma lista real de itens do projeto e aplicar duas técnicas, comparando os resultados.
- [ ]  Definir, com o time, os critérios de valor que serão usados nas próximas priorizações.
- [ ]  Registrar as decisões de priorização na Matriz CSD e no backlog, com o critério usado.
- [ ]  Revisar as prioridades a cada novo aprendizado, sem medo de mudar de ideia com base em evidência.

## Referências

- WAZLAWICK, Raul Sidnei; SANTOS, Ranieri Alves dos; HAMMES, Jades Fernando; CUNHA, Célio Luiz. _Desenvolvimento de Software Centrado no Usuário: Construindo produtos com b_thinking, UX e Agile_. UFSC, 2025.
- SANTOS, Ranieri Alves dos; PEREIRA, Nelma Rodrigues. _Descoberta de Sistemas: uma abordagem para engenharia_. Waiata Multimídia, 2025.