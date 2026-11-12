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

# Canvas de Proposta de Valor

## Resumo

O Canvas de Proposta de Valor é uma ferramenta visual de síntese que alinha o que o produto oferece ao que o usuário realmente valoriza. Ele é composto por dois blocos complementares: o Perfil do Cliente, que descreve as tarefas, dores e ganhos do usuário, e o Mapa de Valor, que descreve como produtos e serviços aliviam essas dores e criam esses ganhos. Seu objetivo central é eliminar o descompasso entre solução e necessidade: uma proposta só é forte quando o mapa de valor endereça diretamente as dores e os ganhos reais do perfil. É uma ferramenta de síntese, não de coleta — ela organiza o que foi descoberto na imersão e orienta decisões sobre o que construir e priorizar.

## Conceitos principais

- Canvas de Proposta de Valor: ferramenta visual que alinha a oferta do produto às necessidades do usuário, conectando o Perfil do Cliente ao Mapa de Valor.
- Perfil do Cliente: bloco que descreve as tarefas (jobs), as dores e os ganhos do usuário — o lado da necessidade.
- Mapa de Valor: bloco que descreve como produtos e serviços criam ganhos e aliviam dores — o lado da solução.
- Tarefas (Jobs): aquilo que o usuário está tentando realizar, seja funcional, emocional ou social.
- Dores: resultados, riscos e obstáculos indesejados que o usuário enfrenta ao tentar realizar suas tarefas.
- Ganhos: resultados e benefícios que o usuário deseja obter ou que o surpreenderiam positivamente.
- Aliviadores de dor: como o produto elimina ou reduz as dores do usuário.
- Criadores de ganho: como o produto produz os resultados e benefícios esperados pelo usuário.
- Encaixe (fit): o grau em que o Mapa de Valor endereça diretamente as dores e ganhos do Perfil do Cliente.

## Conteúdo da aula

### Dois lados que precisam se encontrar

O Canvas de Proposta de Valor parte de uma constatação central: muitos produtos falham porque a equipe constrói uma solução a partir de suposições, sem verificar se ela corresponde ao que o usuário valoriza. A ferramenta coloca frente a frente o lado da necessidade (Perfil do Cliente) e o lado da solução (Mapa de Valor), tornando visível onde há alinhamento e onde há descompasso.

### O Perfil do Cliente

O perfil descreve o usuário a partir de três elementos:

- Tarefas (Jobs): o que o usuário tenta realizar no trabalho e na vida — tarefas funcionais, emocionais e sociais. Exemplo: "registrar as despesas do mês sem perder tempo".
- Dores: tudo que incomoda antes, durante e depois da tarefa — riscos, obstáculos, frustrações e resultados indesejados. Exemplo: "preciso digitar tudo manualmente e ainda esqueço algum gasto".
- Ganhos: os resultados e benefícios que o usuário deseja — o que o faria se sentir bem, economizar tempo ou atingir um objetivo. Exemplo: "ter um resumo automático do que gastei por categoria".

### O Mapa de Valor

O mapa descreve a oferta a partir de três elementos:

- Produtos e serviços: aquilo que a solução entrega — funcionalidades, serviços, artefatos.
- Aliviadores de dor: como o produto elimina ou reduz as dores do perfil. Exemplo: "importação automática de extratos para evitar digitação manual".
- Criadores de ganho: como o produto produz os ganhos desejados. Exemplo: "classificação automática de despesas por categoria".

### O encaixe (fit)

O valor da ferramenta está no encaixe entre os dois blocos:

- Um aliviador de dor só importa se endereçar uma dor real registrada no perfil.
- Um criador de ganho só importa se corresponder a um ganho que o usuário realmente deseja.
- Funcionalidades que não aliviam dores nem criam ganhos são candidatas a despriorização — elas consomem esforço sem gerar valor percebido.

Existem três níveis de encaixe: problema-solução (a solução resolve um problema real do usuário), produto-mercado (a solução funciona e gera valor em escala) e modelo de negócio (a proposta é sustentável comercialmente).

### Relação com o JTBD e o processo de descoberta

O Canvas de Proposta de Valor tem forte ligação com a lente do Jobs to be Done: as tarefas do perfil são os jobs, e as dores e ganhos detalham as forças de progresso que puxam, empurram ou travam o usuário. A ferramenta também consolida os achados da imersão — entrevistas, observação, desk research — e alimenta a Matriz CSD, convertendo suposições sobre o valor da solução em evidências ou novas perguntas a investigar.

## Conexões com as leituras

- Descoberta de Sistemas: apresenta o Canvas de Proposta de Valor entre as ferramentas de síntese e ideação que conectam o entendimento do usuário à proposição de valor da solução, apoiando as decisões de priorização.
- Desenvolvimento de Software Centrado no Usuário: situa o Canvas no processo b_thinking como instrumento que materializa o valor a ser entregue ao usuário, reforçando o foco em dores e ganhos reais durante a descoberta.

## Exemplos e aplicações

- Antes de listar funcionalidades, preencher o Perfil do Cliente com as tarefas, dores e ganhos identificados nas entrevistas e observações.
- Preencher o Mapa de Valor apenas depois do perfil, garantindo que cada aliviador e criador de ganho responda a uma dor ou ganho real.
- Identificar "funcionalidades órfãs": itens do produto que não aliviam nenhuma dor nem criam nenhum ganho registrado — candidatas a corte.
- Avaliar o encaixe de uma ideia de solução antes de investir em desenvolvimento: se o mapa de valor não endereça as dores principais, a proposta precisa ser revista.
- Usar o canvas para priorizar o backlog, ordenando as funcionalidades pelo número de dores e ganhos que endereçam.

## Dúvidas para revisar

- [ ]  Como garantir que as dores e ganhos registrados vêm de evidências reais, e não de suposições da equipe?
- [ ]  Qual a diferença entre uma dor e a ausência de um ganho no Perfil do Cliente?
- [ ]  Como tratar o encaixe quando o usuário não consegue articular suas dores e ganhos?
- [ ]  Como o Canvas de Proposta de Valor se relaciona com o Canvas de Modelo de Negócios sem virar redundância?
- [ ]  Como medir, na prática, se o encaixe problema-solução foi alcançado?

## Aprendizados

- O Canvas de Proposta de Valor alinha necessidade e solução em dois blocos complementares.
- O Perfil do Cliente captura tarefas, dores e ganhos; o Mapa de Valor responde com produtos, aliviadores e criadores de ganho.
- O valor está no encaixe: cada elemento da solução deve endereçar uma dor ou ganho real.
- Funcionalidades que não geram valor percebido devem ser despriorizadas.
- A ferramenta consolida a imersão, dialoga com o JTBD e alimenta a Matriz CSD.

## Próximos passos

- [ ]  Reunir os achados das entrevistas, observações e desk research sobre o usuário.
- [ ]  Preencher o Perfil do Cliente com tarefas, dores e ganhos reais.
- [ ]  Preencher o Mapa de Valor correspondente, garantindo encaixe com cada dor e ganho.
- [ ]  Identificar e despriorizar funcionalidades que não aliviam dores nem criam ganhos.
- [ ]  Registrar as conclusões na Matriz CSD e nas decisões de priorização do projeto.

## Referências

- WAZLAWICK, Raul Sidnei; SANTOS, Ranieri Alves dos; HAMMES, Jades Fernando; CUNHA, Célio Luiz. _Desenvolvimento de Software Centrado no Usuário: Construindo produtos com b_thinking, UX e Agile_. UFSC, 2025.
- SANTOS, Ranieri Alves dos; PEREIRA, Nelma Rodrigues. _Descoberta de Sistemas: uma abordagem para engenharia_. Waiata Multimídia, 2025.