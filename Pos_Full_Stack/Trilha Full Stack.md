Este plano de estudos foi estruturado em **4 fases (24 semanas)** com foco prático. Em vez de criar sistemas genéricos (como listas de tarefas ou lojas virtuais), cada etapa utiliza o seu repertório em **automação industrial, engenharia e telemetria** para construir um portfólio diferenciado para o mercado de **Indústria 4.0 e IoT**.

## Fase 1: Fundamentos Web e Controle de Versão (Semanas 1 a 4)

O objetivo inicial é dominar a base da comunicação na web e as ferramentas padrão de desenvolvimento de software.

- **Controle de Versão:** Git e GitHub (commits semânticos, branches, pull requests).
    
- **Base Front-End:** HTML5 semântico, CSS3 (Flexbox e Grid) e JavaScript moderno (ES6+: `async/await`, manipulação de arrays, `fetch`).
    
- **TypeScript:** Tipagem estática essencial para aplicações corporativas escaláveis.
    
- **Projeto Prático 1 — Calculadora de Engenharia Web:** Crie uma interface responsiva para cálculos técnicos do seu dia a dia (ex.: dimensionamento de inversores, queda de tensão ou geração fotovoltaica) com validação de entradas e exportação de resultados.
    

## Fase 2: Back-End, APIs e Bancos de Dados (Semanas 5 a 10)

Nesta etapa, você aprende a construir o servidor que recebe, processa e armazena dados de campo ou de usuários.

- **Runtime e Linguagem:** **Node.js** com **TypeScript** (usando Express ou Fastify) — ou **Python** (FastAPI), caso queira alinhar com análise de dados industriais.
    
- **Bancos de Dados:** **PostgreSQL** (modelagem relacional, queries SQL, índices) e **TimescaleDB** ou **InfluxDB** (conceitos de séries temporais para leitura de sensores).
    
- **Integração e Protocolos:** Construção de APIs RESTful, autenticação via JWT e introdução a **MQTT** ou **WebSockets** para comunicação em tempo real.
    
- **Projeto Prático 2 — API de Telemetria e Coleta de Dados:** Desenvolva um back-end que recebe leituras simuladas de sensores (temperatura, pressão, corrente) via HTTP ou MQTT, valida os limites operacionais e grava o histórico no PostgreSQL.
    

## Fase 3: Front-End Moderno e Dashboards em Tempo Real (Semanas 11 a 16)

Aqui você une a interface visual ao back-end criado na fase anterior, aplicando conceitos semelhantes aos de sistemas SCADA/IHM, mas em arquitetura web moderna.

- **Framework Front-End:** **React** com TypeScript (componentes, hooks, gerenciamento de estado).
    
- **Estilização e Gráficos:** Tailwind CSS para layout rápido e bibliotecas de visualização de dados (Recharts ou Chart.js).
    
- **Comunicação em Tempo Real:** Consumo da API REST e atualização dinâmica de tela via WebSockets.
    
- **Projeto Prático 3 — Sistema Supervisório Web (Mini-SCADA):** Conecte um front-end em React à API da Fase 2 para exibir indicadores (KPIs), gráficos de tendência em tempo real e alertas visuais quando uma variável ultrapassar o limite configurado.
    

## Fase 4: Arquitetura, Testes e Cloud/DevOps (Semanas 17 a 24)

Para atingir o nível de engenheiro, o código precisa ser testável, empacotado e publicado em ambiente de produção.

- **Conteinerização:** **Docker** e Docker Compose (rodar front-end, back-end e banco de dados em contêineres isolados).
    
- **Testes Automatizados:** Testes unitários e de integração (Vitest ou Jest) garantindo que as regras de negócio e cálculos não quebrem.
    
- **Deploy e Nuvem:** Publicação da aplicação completa em provedores como AWS (EC2/ECS), Railway ou Render, com configuração de variáveis de ambiente e CI/CD básico via GitHub Actions.
    
- **Projeto Prático 4 (Capstone) — Plataforma IoT Ponta a Ponta:** Integre um microcontrolador real (como um **ESP32** ou **Arduino** com módulo Wi-Fi) enviando dados reais para a sua API na nuvem, exibidos no seu dashboard React com autenticação de usuário.
    

### Cronograma Resumido

|**Fase**|**Foco Principal**|**Stack Recomendada**|**Entregável de Portfólio**|
|---|---|---|---|
|**1 (Sem. 1–4)**|Base Web e Tipagem|Git, HTML/CSS, JS, TypeScript|Calculadora Técnica Web|
|**2 (Sem. 5–10)**|Servidor e Dados|Node.js (Fastify/Express), PostgreSQL, MQTT|API de Telemetria Industrial|
|**3 (Sem. 11–16)**|Interface e Tempo Real|React, Tailwind CSS, WebSockets|Dashboard Supervisório (IHM Web)|
|**4 (Sem. 17–24)**|Produção e Hardware|Docker, Testes (Vitest), Cloud, ESP32/Arduino|Sistema IoT Completo em Nuvem|

### Rotina Semanal Sugerida (8 a 10 horas/semana)

1. **Estudo dirigido (30% do tempo):** Documentação oficial, leitura de arquitetura e exemplos pontuais.
    
2. **Prática e código (70% do tempo):** Implementação direta nos projetos acima, subindo código no GitHub pelo menos 3 vezes na semana.