## 📋 Resumo – Higiene do Trabalho 3: Agentes Físicos

_(Formato de nota para Obsidian – markdown)_

---

### 1️⃣ Principais agentes físicos

|Agente|Principais fontes|Efeitos à saúde|Limites regulatórios (NR‑15/NR‑17)|
|---|---|---|---|
|Ruído|Máquinas, ferramentas, veículos, processos industriais|Perda auditiva induzida por ruído (PAIR), estresse, fadiga|85 dB(A) – nível de ação (exposição diária de 8 h). Cada 3 dB acima aumenta a dose em 2×.|
|Vibração mão‑braço (VMB)|Ferramentas portáteis, grampos, martelos pneumáticos|Síndrome de vibração mão‑braço (neuropatia, vasoconstrição, dor).|2,5 m/s² (A(8)) – ação; 5 m/s² – limite de tolerância (NR‑15).|
|Vibração corporal (VCB)|Veículos, máquinas de grande porte, plataformas vibratórias|Dor lombar, fadiga, lesões musculoesqueléticas.|0,5 m/s² (A(8)) – ação; 1,15 m/s² – limite.|
|Temperatura extrema|Calor de fornos, soldagem, clima frio intenso.|Calor: exaustão, insolação, perda de fluido. Frio: hipotermia, chilblains, perda de destreza.|28 °C (WBGT) – ação para calor; 10 °C – ação para frio (NR‑17).|
|Radiações ionizantes|Raios‑X, gama, partículas β/α.|Cancerígenas, efeitos estocásticos e determinísticos.|20 mSv/ano (exposição ocupacional).|
|Radiações não ionizantes (ultravioleta, infravermelho, laser, campos eletromagnéticos)|Soldagem (UV), lasers industriais, antenas, micro‑ondas.|Queimaduras, catarata (UV), lesões cutâneas, efeitos térmicos (infravermelho), distúrbios neurológicos (EMF).|Varia por tipo – ex.: 5 J/cm² (UV) por 8 h, 0,1 W/cm² (laser).|
|Iluminação|Luminárias, luz natural insuficiente, reflexos.|Fadiga visual, redução de produtividade, acidentes.|300–500 lx (área de trabalho) – NR‑17.|

---

### 2️⃣ Avaliação dos agentes

|Etapa|Metodologia|Ferramentas típicas|
|---|---|---|
|Planejamento|Levantamento de fontes, definição de áreas críticas.|Checklist, entrevistas.|
|Medição|- Ruído: dosímetro de nível de pressão sonora (NL), ANALISADOR FFT.  <br>- Vibração: acelerômetro triaxial, analisador de vibração (A(8)).  <br>- Temperatura/Umidade: termômetro, higrômetro, WBGT.  <br>- Radiação: dosímetro pessoal (ionizante), sensores UV, medidor de potência laser.|Equipamentos calibrados conforme ABNT NBR 15625 (ruído) e NBR 15677 (vibração).|
|Comparação|Confrontar resultados com limites de tolerância (TL) das NR‑15/NR‑17.|Planilhas de cálculo (ex.: dose de ruído (D = 10 \log_{10}\left(\frac{1}{T}\sum_{i} T_i 10^{L_i/10}\right))).|
|Relatório|Descrição da exposição, gráfico de distribuição, recomendações.|Markdown/Obsidian note, tabelas, gráficos inseridos via imagem ou mermaid.|

---

### 3️⃣ Hierarquia de Controle (aplicável a todos os agentes)

1. Eliminação – remover a fonte (ex.: desativar máquina).
2. Substituição – trocar por equipamento menos nocivo (ex.: ferramenta antic vibração, motor silencioso).
3. Controles de engenharia – enclausuramento, amortecimento, isolamento acústico, ventilação, blindagem.
4. Controles administrativos – rodízio de tarefas, limites de tempo, pausas, treinamento, sinalização.
5. EPI – protetores auriculares, luvas antivibração, vestimentas térmicas, óculos de proteção, filtros solares.

---

### 4️⃣ Medidas preventivas por agente

#### 4.1 Ruído

- Engenharia: Cabines acústicas, manutenção preventiva (lubrificação, balanceamento).
- Administrativa: Rodízio, limites de exposição (ex.: 4 h a 92 dB(A)).
- EPI: Protetor auricular (espuma ou concha), abafadores eletrônicos.

#### 4.2 Vibração (Mão‑Braço & Corporal)

- Engenharia: Ferramentas antivibratórias certificadas, amortecedores de base.
- Administrativa: Pausas curtas a cada 30 min, rodízio de operadores.
- EPI: Luvas antivibração (auxilia, não elimina).

#### 4.3 Calor/Frio

- Engenharia: Sistemas de climatização, barreiras térmicas, ventilação natural ou forçada.
- Administrativa: Controle de exposição (tempo), ingestão de fluidos, treinamento de primeiros socorros.
- EPI: Roupas de proteção térmica, roupas refletivas, cobertores térmicos.

#### 4.4 Radiações

- Ionizantes: Blindagem de chumbo, distanciamento, tempo de exposição controlado.
- Não ionizantes: Barreira física (tela laser), filtros UV, roupas com filtro UV.

#### 4.5 Iluminação

- Engenharia: Luminárias de alta eficiência, controle de ofuscamento.
- Administrativa: Manutenção de limpeza de lentes, reposição de lâmpadas.

---

### 5️⃣ Monitoramento da saúde ocupacional

- Exames audiométricos (anual) – detectar PAIR precoce.
- Avaliação de vibração – teste de sensibilidade (ex.: 2‑point discrimination), exame clínico.
- Exames de sangue (radiações ionizantes) – contagem de linfócitos.
- Exames de aptidão térmica – teste de tolerância ao calor (WBGT).
- Exames oftalmológicos – para exposição UV/laser.

---

### 6️⃣ Checklist rápido (para usar no Obsidian)

markdown

```
- [ ] Levantar fontes de agentes físicos na área.- [ ] Medir níveis (ruído dB(A), vibração m/s², WBGT °C, etc.).- [ ] Comparar com TL (NR‑15/NR‑17).- [ ] Aplicar hierarquia de controle:    - [ ] Eliminar/Substituir?    - [ ] Implementar controle de engenharia.    - [ ] Definir ações administrativas (rodízio, pausas).    - [ ] Selecionar EPI adequado.- [ ] Registrar resultados e plano de ação.- [ ] Agendar exames médicos periódicos.- [ ] Revisar procedimentos a cada 12 meses ou após mudanças.
```

---

### 7️⃣ Referências rápidas (para consulta)

- NR‑15 – Agentes físicos (ruído, vibração, radiações, temperatura).
- NR‑17 – Ergonomia (exposição ao calor, frio, postura).
- ABNT NBR 15625 – Medição de ruído em ambientes de trabalho.
- ABNT NBR 15677 – Medição de vibração em mãos‑braço.

---

_Esta nota está pronta para ser copiada para o seu vault do Obsidian. Basta criar um novo arquivo (`Agentes Físicos - Higiene do Trabalho 3.md`) e colar o conteúdo acima._