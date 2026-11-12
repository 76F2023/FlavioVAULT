flowchart TD
    Start([Fim do ciclo de descoberta e especificação<br/>o que levar da teoria para a prática]) --> Fio["Considerações Finais e Próximos Passos<br/>consolidar o aprendizado · trilhar o caminho profissional"]

    Fio --> Mensagem["MENSAGEM CENTRAL"]
    subgraph M["MENSAGEM CENTRAL"]
        direction TB
        Mensagem --> M1["Requisitos de qualidade nascem de um processo"]
        M1 --> M2["CONTÍNUO · RASTREÁVEL · CENTRADO NO USUÁRIO"]
        M2 --> M3["O DDR transforma descoberta<br/>em software testável"]
    end

    Fio --> Marcos["OS 8 MARCOS DA DISCIPLINA"]
    subgraph E["FIO CONDUTOR"]
        direction TB
        Marcos --> E1["1 · Engenharia de Requisitos<br/>estruturar o processo"]
        E1 --> E2["2 · Levantamento<br/>descobrir necessidades"]
        E2 --> E3["3 · Análise<br/>organizar e priorizar"]
        E3 --> E4["4 · Especificação<br/>formalizar via DDR"]
        E4 --> E5["5 · Rastreabilidade<br/>origem e destino"]
        E5 --> E6["6 · Verificação e Validação<br/>qualidade e utilidade"]
        E6 --> E7["7 · Aprovação<br/>oficializar a baseline"]
        E7 --> E8["8 · Gerenciamento de Mudanças<br/>manter documento vivo"]
    end

    Fio --> Diferencia["O QUE DIFERENCIA UM BOM DDR"]
    subgraph D["BOM DOCUMENTO DE REQUISITOS"]
        direction TB
        Diferencia --> D1["Clareza e mensurabilidade"]
        Diferencia --> D2["Fonte declarada — sem requisito órfão"]
        Diferencia --> D3["Critério de aceite em Gherkin"]
        Diferencia --> D4["Priorização explícita"]
        Diferencia --> D5["Manutenção planejada — baseline"]
    end

    Fio --> Ciclo["VISÃO INTEGRADA DO CICLO"]
    subgraph C["CICLO NÃO LINEAR"]
        direction TB
        Ciclo --> C1["Descoberta → Análise → Especificação<br/>→ Rastreabilidade → V&V<br/>→ Aprovação → Manutenção"]
        C1 --> C2["Feedback contínuo reabre etapas anteriores"]
        C2 --> C3["Rastreabilidade permite navegar<br/>entre etapas com segurança"]
        C3 --> C4["Mudar uma etapa<br/>impacta todas as outras"]
    end

    Fio --> Impacto["CONCEITOS-CHAVE QUE FICAM"]
    subgraph I["CONCEITOS-CHAVE"]
        direction TB
        Impacto --> I1["Requisito não medido é opinião, não requisito"]
        I1 --> I2["Verificar ≠ Validar:<br/>conformidade × adequação"]
        I2 --> I3["Aprovação é decisão de responsabilidade<br/>com stakeholders"]
        I3 --> I4["IA é multiplicador — nunca substituto"]
    end

    Fio --> Imediato["PRÓXIMOS PASSOS IMEDIATOS"]
    subgraph A["APLICAR JÁ"]
        direction TB
        Imediato --> A1["Conduzir ciclo completo<br/>em projeto real ou simulado"]
        A1 --> A2["Montar DDR mínimo com 10 requisitos<br/>todos com fonte · prioridade · aceite"]
        A2 --> A3["Praticar Gherkin<br/>nos 3 requisitos mais críticos"]
    end

    Fio --> Aprofundar["APROFUNDAR"]
    subgraph P["APROFUNDAMENTO"]
        direction TB
        Aprofundar --> P1["Normas e modelos<br/>IEEE 830 · ISO/IEC 25010 · CMMI · MPS.BR"]
        P1 --> P2["Ferramentas de rastreabilidade<br/>Jira + Confluence · DOORS · CodeBeamer · Craft.io"]
        P2 --> P3["IA generativa na revisão<br/>sempre com validação humana"]
    end

    Fio --> Carreira["PARA A CARREIRA"]
    subgraph Y["CRESCIMENTO PROFISSIONAL"]
        direction TB
        Carreira --> Y1["Portfólio com DDR comentado<br/>decisões e trade-offs"]
        Y1 --> Y2["Mediação entre negócio, UX e dev"]
        Y2 --> Y3["Tornar-se referência<br/>em qualidade de requisitos"]
    end

    Fio --> Caso["CASO APLICADO — DELIVERY"]
    subgraph X["DO LEVANTAMENTO À MUDANÇA"]
        direction TB
        Caso --> X1["Entrevista revela filtro por distância"]
        X1 --> X2["Persona prioriza como Must"]
        X2 --> X3["RF-014 — filtro por raio, resposta ≤ 2s"]
        X3 --> X4["Fonte + Gherkin + revisão técnica"]
        X4 --> X5["Validação com 5 entregadores reais"]
        X5 --> X6["Aprovação → baseline v1.0"]
        X6 --> X7["Mudança 15→20 km → análise de impacto → v1.1"]
    end

    Fio --> Conex["CONEXÕES COM AS LEITURAS"]
    subgraph L["CONEXÕES"]
        direction TB
        Conex --> L1["Engenharia de Requisitos — arcabouço teórico"]
        Conex --> L2["Levantamento — qualidade começa na descoberta"]
        Conex --> L3["Tipos de Requisitos — RF/RNF/RN"]
        Conex --> L4["DDR na Prática — passo a passo operacional"]
        Conex --> L5["DDR com IA — acelerar sem perder responsabilidade"]
        Conex --> L6["VVA — filtro de qualidade antes do dev"]
        Conex --> L7["Gerenciamento e Mudanças — documento vivo"]
    end

    Fio --> Sintese["SÍNTESE FINAL"]
    subgraph S["APRENDIZADOS"]
        direction TB
        Sintese --> S1["Requisitos bem escritos<br/>são a base de todo o ciclo"]
        S1 --> S2["Rastreabilidade é o seguro<br/>contra decisões arbitrárias"]
        S2 --> S3["Validação com usuário real<br/>é insubstituível"]
        S3 --> S4["Mudança é inevitável — o que muda<br/>é o custo de lidar com ela"]
        S4 --> S5["Responsabilidade sobre requisitos<br/>é humana, não algorítmica"]
    end

    style Start fill:#f3f4f6,stroke:#6b7280,color:#111827
    style Fio fill:#111827,stroke:#374151,color:#ffffff
    style Mensagem fill:#fef3c7,stroke:#d97706,color:#7c2d12
    style M1 fill:#fef3c7,stroke:#d97706,color:#7c2d12
    style M2 fill:#fef3c7,stroke:#d97706,color:#7c2d12
    style M3 fill:#fef3c7,stroke:#d97706,color:#7c2d12
    style Marcos fill:#dbeafe,stroke:#2563eb,color:#1e3a8a
    style E1 fill:#dbeafe,stroke:#2563eb,color:#1e3a8a
    style E2 fill:#dbeafe,stroke:#2563eb,color:#1e3a8a
    style E3 fill:#dbeafe,stroke:#2563eb,color:#1e3a8a
    style E4 fill:#dbeafe,stroke:#2563eb,color:#1e3a8a
    style E5 fill:#dbeafe,stroke:#2563eb,color:#1e3a8a
    style E6 fill:#dbeafe,stroke:#2563eb,color:#1e3a8a
    style E7 fill:#dbeafe,stroke:#2563eb,color:#1e3a8a
    style E8 fill:#dbeafe,stroke:#2563eb,color:#1e3a8a
    style Diferencia fill:#dcfce7,stroke:#16a34a,color:#14532d
    style D1 fill:#dcfce7,stroke:#16a34a,color:#14532d
    style D2 fill:#dcfce7,stroke:#16a34a,color:#14532d
    style D3 fill:#dcfce7,stroke:#16a34a,color:#14532d
    style D4 fill:#dcfce7,stroke:#16a34a,color:#14532d
    style D5 fill:#dcfce7,stroke:#16a34a,color:#14532d
    style Ciclo fill:#fce7f3,stroke:#db2777,color:#831843
    style C1 fill:#fce7f3,stroke:#db2777,color:#831843
    style C2 fill:#fce7f3,stroke:#db2777,color:#831843
    style C3 fill:#fce7f3,stroke:#db2777,color:#831843
    style C4 fill:#fce7f3,stroke:#db2777,color:#831843
    style Impacto fill:#fef9c3,stroke:#ca8a04,color:#713f12
    style I1 fill:#fef9c3,stroke:#ca8a04,color:#713f12
    style I2 fill:#fef9c3,stroke:#ca8a04,color:#713f12
    style I3 fill:#fef9c3,stroke:#ca8a04,color:#713f12
    style I4 fill:#fef9c3,stroke:#ca8a04,color:#713f12
    style Imediato fill:#cffafe,stroke:#0891b2,color:#155e75
    style A1 fill:#cffafe,stroke:#0891b2,color:#155e75
    style A2 fill:#cffafe,stroke:#0891b2,color:#155e75
    style A3 fill:#cffafe,stroke:#0891b2,color:#155e75
    style Aprofundar fill:#ede9fe,stroke:#7c3aed,color:#4c1d95
    style P1 fill:#ede9fe,stroke:#7c3aed,color:#4c1d95
    style P2 fill:#ede9fe,stroke:#7c3aed,color:#4c1d95
    style P3 fill:#ede9fe,stroke:#7c3aed,color:#4c1d95
    style Carreira fill:#fce7e7,stroke:#e11d48,color:#881337
    style Y1 fill:#fce7e7,stroke:#e11d48,color:#881337
    style Y2 fill:#fce7e7,stroke:#e11d48,color:#881337
    style Y3 fill:#fce7e7,stroke:#e11d48,color:#881337
    style Caso fill:#d1fae5,stroke:#047857,color:#064e3b
    style X1 fill:#d1fae5,stroke:#047857,color:#064e3b
    style X2 fill:#d1fae5,stroke:#047857,color:#064e3b
    style X3 fill:#d1fae5,stroke:#047857,color:#064e3b
    style X4 fill:#d1fae5,stroke:#047857,color:#064e3b
    style X5 fill:#d1fae5,stroke:#047857,color:#064e3b
    style X6 fill:#d1fae5,stroke:#047857,color:#064e3b
    style X7 fill:#d1fae5,stroke:#047857,color:#064e3b
    style Conex fill:#fef2f2,stroke:#dc2626,color:#7f1d1d
    style L1 fill:#fef2f2,stroke:#dc2626,color:#7f1d1d
    style L2 fill:#fef2f2,stroke:#dc2626,color:#7f1d1d
    style L3 fill:#fef2f2,stroke:#dc2626,color:#7f1d1d
    style L4 fill:#fef2f2,stroke:#dc2626,color:#7f1d1d
    style L5 fill:#fef2f2,stroke:#dc2626,color:#7f1d1d
    style L6 fill:#fef2f2,stroke:#dc2626,color:#7f1d1d
    style L7 fill:#fef2f2,stroke:#dc2626,color:#7f1d1d
    style Sintese fill:#fef9c3,stroke:#ca8a04,color:#713f12
    style S1 fill:#fef9c3,stroke:#ca8a04,color:#713f12
    style S2 fill:#fef9c3,stroke:#ca8a04,color:#713f12
    style S3 fill:#fef9c3,stroke:#ca8a04,color:#713f12
    style S4 fill:#fef9c3,stroke:#ca8a04,color:#713f12
    style S5 fill:#fef9c3,stroke:#ca8a04,color:#713f12