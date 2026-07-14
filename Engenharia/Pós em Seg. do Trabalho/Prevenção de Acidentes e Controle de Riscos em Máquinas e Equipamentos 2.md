## 📚 Resumo – Prevenção de Acidentes e Controle de Riscos em Máquinas e Equipamentos 2

> Objetivo: Complementar a Parte 1 apresentando metodologias avançadas de análise de risco, estratégias de manutenção segura, ergonomia aplicada, requisitos de documentação e boas práticas de gestão de segurança em máquinas e equipamentos.

---

### 1️⃣ Metodologias avançadas de análise de risco

|Técnica|Quando usar|Passos principais|Ferramentas típicas|
|---|---|---|---|
|HAZOP (Hazard and Operability Study)|Processos complexos, mudanças de projeto.|1. Definir “ponto de estudo” 2. Identificar desvios (‑/+) 3. Avaliar consequências 4. Propor medidas corretivas.|Software HAZOP, planilhas estruturadas.|
|FMEA / AMDEC (Análise de Modos de Falha e seus Efeitos)|Equipamentos críticos, alta taxa de falhas.|1. Listar funções do equipamento 2. Identificar modos de falha 3. Avaliar severidade, ocorrência, detecção 4. Calcular RPN (Risk Priority Number).|Excel, Minitab, ferramentas de FMEA.|
|Árvore de Falhas (FTA – Fault Tree Analysis)|Falhas catastróficas ou de segurança.|1. Definir evento top – falha 2. Decompô‑lo em causas lógicas (AND/OR) 3. Quantificar probabilidades.|Software de FTA (e.g., CAFTA).|
|Análise Quantitativa de Risco (QRA)|Decisões de investimento em controles.|1. Modelagem estocástica 2. Simulação Monte Carlo 3. Estimativa de perdas esperadas (€/ano).|@Risk, Crystal Ball.|

> Resultado esperado: Lista priorizada de riscos → definição de controles de acordo com a hierarquia (eliminação → engenharia → administrativo → EPI).

---

### 2️⃣ Estratégias de manutenção segura (MSM)

|Tipo de manutenção|Principais requisitos (NR‑12)|Controle recomendado|
|---|---|---|
|Preventiva|Planejamento de intervenções, registro no DSM.|Inspeções periódicas, lubrificação programada, substituição preventiva de peças críticas.|
|Corretiva|Bloqueio/Tag‑out (BTO) obrigatório antes da ação.|Checklist BTO, validação de energia isolada, liberação apenas após verificação.|
|Preditiva|Uso de monitoramento de condição (vibração, termografia).|Sistemas de análise de vibração, termografia infravermelha, análise de óleo.|
|Proativa (Redesign)|Eliminação de riscos no projeto.|Redesenho de componentes, substituição por tecnologias sem risco (ex.: acionamento hidráulico por elétrico com limitadores).|

#### Checklist de manutenção segura (para inserir no Obsidian)

markdown

```
- [ ] Verificar validade da **BTO** (cadernos, etiquetas, cadeados).  - [ ] Confirmar **energização** desligada (testes de voltagem, pressão).  - [ ] Inspecionar **guardas** e **intertravamentos** antes de iniciar.  - [ ] Registrar **tempo de parada** e **atividades realizadas**.  - [ ] Realizar **testes de funcionamento** após a manutenção.  - [ ] Atualizar **DSM** e **registros de manutenção**.  
```

---

### 3️⃣ Ergonomia aplicada a máquinas e equipamentos

|Aspecto ergonômico|Diretriz prática|Impacto na segurança|
|---|---|---|
|Postura e alcance|Projetar controles a < 65 cm da zona de alcance confortável.|Reduz LER/DORT e fadiga que podem causar erros.|
|Força necessária|Limitar esforço máximo a 25 N para manuseio manual.|Diminui risco de lesões musculares e acidentes por sobrecarga.|
|Visibilidade|Iluminação mínima 500 lux no ponto de operação e sinalização luminosa de emergência.|Previne erros de operação e quedas.|
|Vibração transmissível|Isolar fontes vibratórias; uso de suportes antivibração.|Evita Síndrome de Vibração de Mãos‑Braço.|
|Feedback tátil/auditivo|Implementar indicadores sonoros e vibro‑táteis ao iniciar/parar a máquina.|Aumenta a percepção do estado da máquina e reduz tempos de reação.|

> Recurso interno: `[[Ergonomia de Máquinas – Diretrizes ABNT NBR 13175]]`

---

### 4️⃣ Documentação avançada (extensão do DSM)

|Documento|Conteúdo essencial|Frequência de atualização|
|---|---|---|
|DSM – Manual de Segurança|Descrição técnica, diagramas de energia, procedimentos de emergência, lista de EPIs recomendados.|Sempre que houver alteração de projeto ou de normativa.|
|Relatório de Análise de Risco (RAR)|Metodologia usada, matriz de risco, medidas implantadas, RPN ou índices de risco.|Anual ou após mudança significativa.|
|Plano de Manutenção Segura (PMS)|Calendário, responsáveis, BTO, inspeções de dispositivos de segurança.|Semestral ou conforme MTBF.|
|Ficha de Inspeção de Segurança (FIS)|Check‑list de verificação diária (guardas, E‑stop, sinalização).|Diária – registro eletrônico.|
|Registro de Treinamento (RT)|Lista de trabalhadores, conteúdo, data, validade da certificação.|A cada renovação de competência (ex.: 2 anos).|

Sugestão de template Obsidian (front‑matter YAML):

yaml

```
---title: "DSM – Máquina X"date: 2026-07-14tags: [#NR12, #segurança, #documentação]status: "Ativa"---
```

---

### 5️⃣ Gestão de mudanças (MOC – Management of Change)

|Etapa|Ação|Responsável|
|---|---|---|
|Identificação|Registrar a mudança proposta (novo componente, ajuste de processo).|Engenheiro de projeto|
|Avaliação de risco|Aplicar FMEA/HAZOP ao impacto da mudança.|Analista de segurança|
|Aprovação|Revisão de documentos (DSM, RAR) e liberação de orçamento.|Gerente de SST|
|Implementação|Executar mudança com BTO, treinamento específico.|Supervisor de operação|
|Verificação|Inspeção pós‑implementação e atualização de documentos.|Auditor interno|

> Referência interna: `[[MOC – Procedimento de Controle de Mudanças]]`

---

### 6️⃣ Indicadores de desempenho (KPIs) avançados

|KPI|Fórmula / Fonte|Meta sugerida|
|---|---|---|
|Índice de Conformidade de Dispositivos de Segurança (ICDS)|(Dispositivos conformes ÷ total de dispositivos) × 100%|≥ 98 %|
|Tempo Médio de Resposta a Falhas (MTTR‑Seg)|Soma dos tempos de parada de segurança ÷ número de incidentes|≤ 30 min|
|RPN Médio Pós‑Análise|Média dos RPNs após FMEA/Avaliação|≤ 150|
|Taxa de Treinamento em MOC|(Operadores treinados após mudança ÷ total de afetados) × 100%|100 %|
|Número de Não‑Conformidades por Auditoria|Contagem de NC encontradas|≤ 2 por auditoria|

---

### 7️⃣ Boas práticas de implementação (checklist rápido)

- [ ]  Mapear todas as máquinas e equipamentos críticos.
- [ ]  Atualizar o DSM e criar o RAR para cada máquina.
- [ ]  Aplicar FMEA/HAZOP nas alterações de projeto.
- [ ]  Instalar guardas, intertravamentos e E‑stop conforme NR‑12.
- [ ]  Implementar programa de manutenção segura (BTO, PST).
- [ ]  Treinar operadores em procedimentos de emergência e uso de EPIs.
- [ ]  Realizar auditorias trimestrais e atualizar KPIs.
- [ ]  Documentar todas as mudanças via MOC.

---

### 8️⃣ Links internos sugeridos (para o seu vault)

- `[[NR‑12 – Segurança em Máquinas e Equipamentos]]`
- `[[Documento de Segurança da Máquina (DSM) – Modelo]]`
- `[[FMEA – Guia Prático]]`
- `[[HAZOP – Passo a Passo]]`
- `[[MOC – Gestão de Mudanças]]`
- `[[Ergonomia de Máquinas – Diretrizes ABNT NBR 13175]]`
- `[[KPIs de Segurança – Dashboard]]`

---

### 🏷️ Tags (adicione ao final da nota)

markdown

```
tags: #segurança #máquinas #NR12 #análise_de_risco #manutenção #ergonomia #MOC #SST
```

---

Como usar no Obsidian

1. Crie um novo arquivo: `Prevenção de Acidentes e Controle de Riscos em Máquinas e Equipamentos 2.md`.
2. Cole o conteúdo acima, mantendo a hierarquia (`##`, `###`).
3. Utilize os links internos sugeridos para conectar a outras notas do seu banco de conhecimento.
4. Atualize periodicamente os KPIs, checklist de manutenção e o RAR conforme novas medições ou mudanças de processo.

Pronto! Agora você possui um ponto de referência completo para avançar na gestão de segurança de máquinas e equipamentos.