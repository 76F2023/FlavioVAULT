## 📄 Nota Obsidian – CLCB vs AVCB (São Paulo)

> _Use a estrutura abaixo como “template”_ – copie‑coloque em uma nova nota no Obsidian e preencha os campos com os dados do seu projeto (área, uso, localização etc.).

---

### 1️⃣ Definições rápidas

|Sigla|Nome completo|Quando é obrigatório|Tipo de risco|Principal procedimento|
|---|---|---|---|---|
|CLCB|Certificado de Licença do Corpo de Bombeiros|Edificações baixo risco (até 750 m², ≤ 3 pavimentos, altura ≤ 12 m)|Baixo|Processo simplificado – autodeclaração, entrega de documentos, pagamento da Guia D.|
|AVCB|Auto de Vistoria do Corpo de Bombeiros|Edificações alto risco, áreas > 750 m², ocupação > 250 pessoas, altura > 12 m, etc.|Alto|Projeto Técnico (PT/PTS) + vistoria presencial + pagamento de taxa de análise + taxa de vistoria.|

---

### 2️⃣ Critérios de enquadramento (IT‑42/SP)

|Critério|CLCB (✓)|AVCB (✗)|
|---|---|---|
|Área construída ≤ 750 m²|✔|–|
|Altura ≤ 12 m|✔|–|
|≤ 3 pavimentos|✔|–|
|Sem sistemas de pressurização de escadas, sprinklers ou alarme interligado|✔|–|
|Carga de incêndio < 300 MJ/m²|✔|–|
|Uso de inflamáveis ou risco especial (hospital, depósito químico…)|–|✔|
|Subsolo ocupado|–|✔|
|Necessidade de projetos de hidrantes, pressurizadores, etc.|–|✔|

> Dica: Se qualquer item acima for “✗”, o imóvel deve seguir o fluxo AVCB.

---

### 3️⃣ Passo‑a‑passo – CLCB (São Paulo)

1. Contratar responsável técnico (Eng.º ou Arq.) – gerar ART.
2. Reunir documentação
    - Projeto Arquitetônico (plantas, cortes).
    - Memória de cálculo de extintores, sinalização e iluminação de emergência.
    - Declaração de conformidade (autodeclaração).
    - Documentos do proprietário (CPF/CNPJ, IPTU, certidão de regularidade).
3. Abrir processo no portal _Via Fácil_
    - URL: `https://www.bombeiros.sp.gov.br/via-facil`
    - Selecionar “Emissão de CLCB / PTS”.
    - Inserir área, uso, altura e número de pavimentos.
4. Gerar a Guia D (Taxa).
    - Valor mínimo: R$ 106,02 (taxa fixa).
    - Se a UFESP estiver atualizada, pode aparecer ~ R$ 120‑R$ 145 (ex.: R$ 131).
5. Pagamento (Boleto ou Pix).
6. Upload da documentação (ART + arquivos).
7. Aguardar análise (até 7 dias úteis).
8. Receber CLCB (PDF digital).

> Validade: 2 – 5 anos (segundo a classificação). Renove 60 dias antes do vencimento.

---

### 4️⃣ Passo‑a‑passo – AVCB (São Paulo)

|Etapa|O que fazer|Prazo típico|
|---|---|---|
|1. Responsável técnico|ART + elaboração de Projeto Técnico (PT) ou Projeto Técnico Simplificado (PTS)|–|
|2. Documentação|Projeto de PCI (extintores, hidrantes, sinalização, iluminação de emergência, rota de fuga).|–|
|3. Portal _Via Fácil_|Selecionar “Emissão de AVCB”. Inserir dados (área, risco, etc.).|–|
|4. Taxas|- Taxa de análise = Área × 0,003 × UFESP  <br>- Taxa de vistoria = Área × 0,004 × UFESP|- Ex.: 800 m² → R$ 48,33 (análise) + R$ 64,44 (vistoria) (valores de 2025).|
|5. Pagamento|Emissão de guias (Boleto/PIX).|–|
|6. Vistoria presencial|Agendar com o CBPMESP – inspeção de extintores, rotas, sinalização.|Até 30 dias após pagamento.|
|7. Correções (se houver)|Ajustar pendências e reenviar.|–|
|8. Emissão do AVCB|PDF digital + validade (2‑5 anos).|–|

---

### 5️⃣ Tabela resumida de custos (2026 – SP)

|Item|CLCB (até 750 m²)|AVCB (exemplo 800 m²)|
|---|---|---|
|Taxa do Corpo de Bombeiros|R$ 106,02 (mínimo)  <br>_(ou R$ 131 ≈ valor da Guia D atual)_|Análise: Área × 0,003 × UFESP  <br>Vistoria: Área × 0,004 × UFESP|
|ART (CREA)|R$ 96,00 (média)|R$ 96,00 (média)|
|Projetos e honorários|R$ 1.500 – 3.000 (dependendo da complexidade)|R$ 2.000 – 6.000 (mais detalhado)|
|Equipamentos (extintores, sinalização, iluminação)|R$ 2.000 – 4.000 (aprox.)|R$ 4.000 – 10.000 (dependendo do risco)|
|Total estimado (cliente)|R$ 3.600 – 7.200|R$ 8.000 – 20.000|

> Obs.: Valores de equipamentos variam conforme a carga de incêndio e a quantidade de extintores exigidos.

---

### 6️⃣ Checklist rápido (para copiar‑colar)

markdown

```
## 📋 Checklist CLCB / AVCB – Projeto: {{Nome do Projeto}}

- [] Contratar Engenheiro/Arquiteto → gerar ART (R$ 96) 
- [] Área construída: {{m²}} 
- [] Altura: {{m}} 
- [] Nº de pavimentos: {{n}} 
- [] Uso: {{Comercial/Industrial/Residencial...}} 
- [] Verificar risco (IT‑42) → CLCB ou AVCB? 
- [] Reunir documentos:    
- [ ] Projeto arquitetônico    
- [ ] Memória de cálculo PCI    
- [ ] Declaração de conformidade (autodeclaração)    
- [ ] CPF/CNPJ + IPTU + certidão regularidade 
- [] Acessar portal Via Fácil:     
- [ ] Inserir dados → gerar Guia D    
- [ ] Pago? (R$ 106,02 ou cálculo UFESP) 
- [] Upload da documentação no portal 
- [] Aguardar aprovação (CLCB ≤ 7 dias / AVCB ≤ 30 dias + vistoria) 
- [] Receber PDF → salvar em Obsidian → vincular ao projeto 
- [] Agendar renovação (60 dias antes do vencimento)
  
**Próximos passos:**  

- [] Comprar extintores ({{qtde}}) – estimativa R$ {{valor}}  
- [] Instalar sinalização de saída de emergência  
- [] Treinamento de brigada (se necessário)  
```

---

### 7️⃣ Recursos úteis (links)

|Tipo|URL|
|---|---|
|Portal oficial – Via Fácil (SP)|https://www.bombeiros.sp.gov.br/via-facil|
|Instrução Técnica 42 – CBPMESP|https://www.bombeiros.sp.gov.br/it/it-42|
|Tabela UFESP (valor fiscal)|https://www.fazenda.sp.gov.br/ufesp|
|Artigos de apoio|- https://www.portalinsights.com.br/o-que-e-clcb  <br>- https://www.cabolavo.com.br/clcb-5-passos-para-emitir-seu-clcb|
|Vídeo explicativo (Soraia Pereira)*|https://www.youtube.com/watch?v=Nk3V4cYBp-o|
|Modelo de nota fiscal / orçamento (exemplo)|https://github.com/obsidianmd/obsidian-sample-notes|

---

### 8️⃣ Resumo de “quando usar”

|Tipo de empreendimento|Área|Altura|Nº de pavimentos|Risco|Recomendação|
|---|---|---|---|---|---|
|Loja de conveniência|≤ 750 m²|≤ 12 m|≤ 3|Baixo|CLCB|
|Restaurante (público > 250)|> 750 m²*|> 12 m|> 3|Médio/alto|AVCB|
|Adega (uso próprio)|≤ 750 m²*|≤ 12 m|≤ 3|Baixo|CLCB|
|Indústria de químicos|Qualquer|Qualquer|Qualquer|Alto|AVCB|

--------------------------------
