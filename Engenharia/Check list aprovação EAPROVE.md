
## Checklist Atualizado – Projeto para a Secretaria de [[Engenharia]]
([[Prefeitura de Indaiatuba-SP]])


_(Inclui os novos “COMUNIQUE‑SE” que você recebeu)_

---

### 1. Cadastro – Cota DCIE / Requerimento

|✔|Item|Como conferir|Observação|
|---|---|---|---|
||Logradouro|Verifique a grafia correta no cadastro municipal (ex.: RUA JEFFERSON HENRIQUE DE SOUZA).|Use o portal GeoSampa ou a base da Prefeitura.|
||Lote / Quadra|Lote 13 – Quadra P.|Deve constar exatamente no requerimento.|
||Loteamento|JARDIM BOM SUCESSO (nome oficial).|Sem abreviações.|
||Nome do proprietário|VICTOR ARRUDA NASSAR – exatamente como no cadastro.|Atenção a acentos e espaço antes de “NASSAR”.|
||Cota DCIE / Numeração|Preencha o campo com o número fornecido pelo sistema.|Número fora de sequência gera devolução.|
||Assinatura/Carimbo|Assinatura digital ou física do requerente e carimbo da empresa.|Não incluir telefone/e‑mail no corpo do documento.|

---

### 2. ART / RRT / TRT – Tipo de Atividade

|✔|Item|Como conferir|Observação|
|---|---|---|---|
||Tipo de atividade|ART deve estar “Direção de Obra” (não “Condução de equipe”).|Verifique na planilha de ART/RRT.|
||Número da ART|Inserir o número da ART na planta (campo “ART nº …”).|Atualizar em todos os documentos quando houver mudança.|
||Autor e Responsável|Logo abaixo da ART, colocar nome completo + CREA do autor e do responsável.|Ex.: “Autor: João Silva – CREA‑SP 1234567 – Responsável: Maria Costa – CREA‑SP 7654321”.|
||Validade|Data de validade da ART vigente na data de envio.|ART vencida = devolução automática.|

---

### 3. Planta (Croqui) – Instruções de Formato e Escala

|✔|Item|Como conferir|Observação|
|---|---|---|---|
||Escala|Croqui sem escala (quando exigido) ou escala 1:100 para impressão.|Se for croqui, remover barra de escala; se precisar imprimir, garantir 1:100.|
||Endereço completo|Inserir Rua, Lote, Quadra e Loteamento exatamente como no cadastro.|Revisar ortografia.|
||Situação|Campo “Situação” preenchido – sem escala.|Ex.: “Em construção”.|
||Número da ART|Atualizar com o novo número da ART.|Deve estar legível.|
||Autor/Responsável|Colocar abaixo da ART (ver tabela 2).|Não usar abreviações.|
||Contato|Remover telefone e e‑mail da planta.|Caso precise, use a “Ficha Técnica”.|
||Arquivo anexado|Verificar se o PDF da planta foi realmente anexado ao processo.|Erro comum: “arquivo da planta não foi anexado”.|
||Formato final|PDF 1.4 – fonte Arial 11 pt.|Evita problemas de leitura no portal.|
||Tamanho da folha|Para impressão em escala 1:100, folha A1 (841 × 594 mm).|Não enviar em A4.|

---

### 4. Implantação em DWG – Modelo da Prefeitura de Indaiatuba

|✔|Item|Como conferir|Observação|
|---|---|---|---|
||Arquivo DWG|Deve seguir exatamente o modelo disponível em: https://www.indaiatuba.sp.gov.br/download/67165/.|Baixe o modelo, compare camadas, blocos e textos.|
||Escala|Implantação em escala 1:100 (mesma escala da planta).|Verifique a escala nas propriedades do desenho.|
||Tamanho da folha|A1 (841 × 594 mm) ou tamanho equivalente indicado pelo modelo.|Não usar A4.|
||Camadas|Use as mesmas nomenclaturas de camada do modelo (ex.: _COTAS_, _PERIMETRO_, _ARQUIVOS_).|Facilita a análise da secretaria.|
||Anexar|Anexe o DWG na mesma entrega em que a planta (PDF/DWF) é enviada.|O portal aceita até 10 MB por arquivo.|
||Verificação final|Abra o DWG no AutoCAD e imprima em “Plot to DWF6ePlot.pc3” → Paper Size = A1 → Scale = 1:100 → Monochrome.ctb. Salve e re‑envie.|Confirma que o arquivo está pronto para impressão.|

---

### 5. Plantas em DWF – Escala Correta (1:100)

Passo a passo para gerar o DWF corretamente

1. File > Plot
2. Printer/Plotter → selecione DWF6ePlot.pc3.
3. Paper Size → escolha A1 (841 × 594 mm) (ou outro tamanho indicado).
4. Plot Area → clique em Window e selecione o desenho:
    - Clique _um pouco_ fora da margem inferior‑esquerda.
    - Clique _um pouco_ fora da margem superior‑direita (diagonal).
5. Desmarque Center the Plot e zere X e Y.
6. Desmarque Fit to Paper e insira 1 mm = 0,1 unit (ou 1 unit = 10 mm).
7. Plot Style Table → escolha monochrome.ctb (pode ajustar espessuras das linhas).
8. Clique Apply to Layout e OK → salve o DWF.

Instalação do visualizador DWF – Autodesk Design Review

1. Acesse www.autodesk.com → Menu > Downloads > File Viewers.
2. Clique em “Looking for DWG TrueView, Design Review, and other Viewers?”.
3. Na página seguinte, em File Types, selecione Design Review.
4. Clique em Download Design Review.
5. Selecione Brazilian Portuguese e salve o instalador.
6. Na mesma página, baixe o “Autodesk Design Review 2013 Hotfix” (atualização).
7. Instale ambos – o Hotfix deve ser aplicado após a instalação principal.

|✔|Item|Como conferir|Observação|
|---|---|---|---|
||Escala no DWF|Abra o DWF no Design Review → Measure → verifique que 1 mm = 0,1 unit (ou 1 unit = 10 mm).|Confirmação visual.|
||Tamanho da folha|No visualizador, veja a área de impressão – deve ser A1.|Evita devolução por “folha incorreta”.|
||Qualidade|Visualize em 100 % – linhas e textos legíveis.|DWF monocromático sem hachuras desnecessárias.|
||Arquivo anexado|No portal da Prefeitura, faça o upload do DWF e confirme que o download funciona.|Teste rápido: clique no link de preview.|

---

### 6. Documentação Complementar (sem alterações)

|✔|Item|Como conferir|
|---|---|---|
||Memorial Descritivo|Ortografia correta, normas técnicas (NBR) citadas.|
||Planta de Implantação (PLI)|Recuos frontais, laterais e de fundo dentro do zoneamento.|
||Certidão de Uso do Solo|Data ≤ 180 dias.|
||Licença Ambiental (se houver)|Anexar, número e validade.|
||Comprovante de taxa|QR‑code ou boleto quitado.|
||Ficha de Responsável Técnico (FRT)|CREA e número da ART preenchidos.|

---

### 7. Revisão Final – “Pré‑Check” Unificado

Copie‑e‑cole este bloco no final do seu processo antes de clicar em Enviar:

```
[ ] Dados cadastrais (logr., lote, quadra, loteamento) conferidos.[ ] Nome do proprietário exatamente como no cadastro: VICTOR ARRUDA NASSAR.[ ] Cota DCIE/Numeração preenchida.[ ] ART revisada – tipo de atividade = Direção de Obra.[ ] Número da ART atualizado nas plantas.[ ] Planta (PDF) sem escala ou em escala 1:100 (folha A1) – sem telefone/e‑mail.[ ] Autor e responsável listados abaixo da ART.[ ] Arquivo da planta (PDF) anexado.[ ] Implantação DWG conforme modelo <https://www.indaiatuba.sp.gov.br/download/67165/> – escala 1:100, folha A1.[ ] DWF gerado seguindo o passo a passo – escala 1:100, folha A1, Monochrome.ctb.[ ] Design Review instalado – DWF visualizado OK.[ ] Memorial descritivo revisado.[ ] PLI com recuos corretos.[ ] Certidão de uso do solo (≤ 180 dias) incluída.[ ] Licença ambiental (se necessária) incluída.[ ] Comprovante de pagamento da taxa anexado.[ ] FRT preenchida e assinada.[ ] Todos os PDFs em versão 1.4, fonte Arial 11 pt.[ ] Revisão interna feita por colega.[ ] Protocolo de envio registrado e número salvo.
```

---

### 8. Dicas para minimizar “COMUNIQUE‑SE”

1. Use o modelo DWG da Indaiatuba como “baseline” para todas as implantações.
2. Padronize a geração de DWF – salve um _template_ de plot com as opções já configuradas.
3. Checklist digital – mantenha este documento em um arquivo Excel/Google Sheets com checkboxes que mudam de cor automaticamente.
4. Validação automática – pequeno script em Python que abre o PDF/DWF e verifica a presença das palavras‑chave: “ART”, “Autor”, “Responsável”, “Escala 1:100”.
5. Contato pré‑vio – envie um e‑mail curto à secretaria (ex.: “Boa tarde, gostaria de confirmar se o modelo DWG da Indaiatuba ainda está vigente para a implantação”). Evita surpresas de última hora.

---

Com este checklist já ampliado, você cobre todos os pontos que geraram as últimas devoluções e tem um fluxo de trabalho pronto para novos projetos. Boa sorte, Flávio, e conte comigo caso precise de ajustes pontuais antes do envio!