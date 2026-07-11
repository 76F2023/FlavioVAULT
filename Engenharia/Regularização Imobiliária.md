# 📋 Regularização Imobiliária – Guia Rápido para Obsidian

_(Engenheiro Civil – +20 anos de experiência em SP)_

---

## 1️⃣ Visão geral do fluxo

mermaid

```
flowchart LR    A[Projeto/Planta] --> B[Alvará de Construção]    B --> C[Execução da Obra]    C --> D[INSS + Receita Federal]    D --> E[Habite‑se]    E --> F[Averbação / Registro no Cartório]
```

> Objetivo: Obter a documentação final que comprova a regularidade do imóvel e permite sua venda, financiamento ou uso comercial.

---

## 2️⃣ Etapas detalhadas

### 2.1 Alvará de Construção (Prefeitura)

|Item|O que fazer|Dicas/Obs.|
|---|---|---|
|Levantamento cadastral|Requerimento de Cota DCIE, CEP, endereço completo, número de ART (Direção de Obra).|Use o checklist de verificação (ver 📂 Checklist‑Alvará).|
|Projeto arquitetônico|Planta de implantação (DWG conforme modelo da prefeitura), planta baixa (PDF/DWF escala 1:100, folha A1), memorial descritivo.|Mantenha o mesmo padrão de camadas do modelo de Indaiatuba.|
|Documentos complementares|ART/RRT, certidão de uso do solo (≤ 180 dias), taxa de licença paga, comprovação de responsabilidade técnica (CREA).|Verifique validade antes de enviar.|
|Entrega|Protocolo digital via SPWeb ou entrega presencial. Guarde o número de protocolo.|Salve o PDF de protocolo em `📁 /Docs/Prefeitura/Alvará/`.|

### 2.2 INSS + Receita Federal (Obra)

|Item|O que fazer|Dicas/Obs.|
|---|---|---|
|CNPJ da obra|Se empresa já possui, usar CNPJ ativo; caso contrário, abrir CNPJ de obra.|Use o Código de Atividade (CNAE) 41.20‑4‑00 (Construção de edifícios).|
|Guia da GPS|Emitir Guia da GPS (INSS) para cada mês de obra (R$ 1,20 % sobre a folha de pagamento).|Automatize com planilha `🗂️/Finance/INSS‑GPS.xlsx`.|
|RAIS/CTPS|Registrar empregados, gerar Folha de Pagamento (eSocial).|Evite multas por falta de recolhimento.|
|Declaração de Imposto de Renda|Informar receitas/despesas da obra na DCTF e no DIRF.|Mantenha notas fiscais eletrônicas organizadas (`📁 /Docs/Finance/Notas/`).|

### 2.3 Habite‑se (Prefeitura)

|Item|O que fazer|Dicas/Obs.|
|---|---|---|
|Vistoria final|Agendar inspeção com a fiscalização municipal (pode ser presencial ou via foto).|Tenha a obra 100 % concluída e limpa (sem entulhos).|
|Documentos exigidos|ART final, laudos de instalações (elétrica, hidráulica, gás), Certificado de Conformidade de Sistema de Segurança (se houver).|Use a checklist 📂 Checklist‑Habite‑se.|
|Recolhimento de taxa|Taxa de Habite‑se (consultar tabela municipal).|Guarde o comprovante como `Habite‑se‑Taxa.pdf`.|
|Emissão|Recebe o certificado de conclusão e o número do Habite‑se.|Arquive em `📁 /Docs/Prefeitura/Habite‑se/`.|

### 2.4 Averbação / Registro no Cartório de Registro de Imóveis

|Item|O que fazer|Dicas/Obs.|
|---|---|---|
|Documentação|Escritura ou contrato de compra, Habite‑se, Alvará, ART, Certidão de ônus reais atualizada, IPTU quitado.|Consolidar tudo num “Dossiê de Averbação”.|
|Requerimento de averbação|Preencher formulário do cartório (geralmente disponível no site).|Use o modelo `🗂️/Templates/Averbação.docx`.|
|Pagamento de emolumentos|Tabela de custas cartoriais (varia por estado).|Salve o comprovante como `Emolumentos.pdf`.|
|Registro|O cartório registra as mudanças (área construída, taxa de ocupação, etc.) e devolve o "Matrícula Atualizada".|Escaneie a matrícula e armazene em `📁 /Docs/Cartório/Matrícula/`.|

---

## 3️⃣ Checklist‑Rápido (para copiar‑e‑colar)

markdown

```
- [ ] **Alvará**  
- [ ] Requerimento Cota DCIE preenchido 
- [ ] Planta de implantação (DWG) conforme modelo  
- [ ] Planta baixa (PDF/DWF 1:100, A1)  
- [ ] ART – Direção de Obra  
- [ ] Certidão de uso do solo ≤ 180 dias  
- [ ] Taxa de licença paga → comprovante salvo 
- [ ] **INSS/Receita**  
- [ ] CNPJ da obra ativo  
- [ ] GPS mensal emitida (planilha)  
- [ ] eSocial/CTPS atualizado  
- [ ] DCTF/DIRF enviadas 
- [ ] **Habite‑se**  
- [ ] Vistoria final concluída  
- [ ] Laudos de instalações (elétrica, hidráulica, gás)  
- [ ] Taxa de Habite‑se paga → comprovante salvo  
- [ ] Certificado de Habite‑se recebido 
- [ ] **Averbação**  
- [ ] Escritura/Contrato em mãos  
- [ ] Habite‑se, Alvará, ART anexados  
- [ ] Certidão de ônus reais atualizada  
- [ ] IPTU quitado  
- [ ] Emolumentos pagos → comprovante salvo  
- [ ] Matrícula atualizada recebida
```

> Dica Obsidian:
> 
> - Crie um template note chamado `🗒️ Regularização Imobiliária` e cole o checklist acima.
> - Use as tags `#regularizacao #obras #documentação` para facilitar a busca.
> - Vincule a nota ao seu project folder (`📁 /Projetos/NomeDoProjeto`) usando `[[Regularização Imobiliária]]`.

---

## 4️⃣ Atalhos úteis

|Ferramenta|Link rápido|Comentário|
|---|---|---|
|Portal SPWeb (Alvará/ Habite‑se)|https://www.prefeitura.sp.gov.br|Salve como bookmark no Obsidian (`[[Portal Prefeitura]]`).|
|eSocial|https://www.esocial.gov.br|Centraliza recolhimento de INSS e FGTS.|
|Site da Receita Federal|https://www.gov.br/receitafederal|Consulta CNPJ, DCTF, DIRF.|
|Cartório Online (Consulta de matrícula)|https://www.cartorios.gov.br|Use para solicitar certidões e solicitar averbação.|

---

## 5️⃣ Referências rápidas (PDF/Links)

- Manual de Alvarás – Prefeitura de SP – `📁 /Docs/Prefeitura/Manual_Alvará.pdf`
- Guia GPS – INSS – `📁 /Docs/Finance/Guia_GPS.pdf`
- Normas Técnicas NBR 15575 (Habitação) – `📁 /Docs/NBR/15575.pdf`
- Tabela de Custas Cartoriais – São Paulo – `📁 /Docs/Cartório/Tabela_Custas.pdf`
-----------------------------------------------------------------
