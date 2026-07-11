
Passo 1 - Fazer o CTF (Casdastro Técnico Federal)

	Emitir:  a)Comprovante de Inscrição.
			b)Certificado de Regularidade

A princípio essa fase dará acesso a apenas 2 módulos do SINAFLOR.
IMÓVEIS
EMPREENDIMENTOS

https://servicos.ibama.gov.br/sinaflor-ext/SigefExterno.html#visaoHome
--------------------------------

# Sinaflor: Cadastro de Empreendimento e Projeto (Corte de Árvores Isoladas)

## 1. Cadastro do Empreendimento
* **Módulos Iniciais:** Após a etapa do Cadastro Técnico Federal (CTF), o sistema libera os módulos **Imóveis** e **Empreendimentos**.
* **Identificação:** O nome do empreendimento pode ser o nome da propriedade (chácara, lote urbano ou denominação genérica).
* **Inscrição Estadual:** O sistema exige o preenchimento de todos os campos. Caso não possua inscrição estadual, digite "Isento" ou "000".
* **Competência (Estadual vs. Municipal):** É fundamental checar se o município já possui licenciamento descentralizado ou se o processo corre via escritório regional do órgão estadual (ex: IAP no Paraná).
* **Georreferenciamento:** Deve-se desenhar a área do imóvel utilizando a ferramenta de desenho à mão livre ou importando um arquivo *Shapefile* (`.shp`).
* **Envio para Homologação:** Revise tudo antes de enviar. Após clicar no ícone de envio no canto inferior direito, o status muda de *Em cadastro* para *Em homologação*. Os dados não podem mais ser alterados. O empreendimento precisa ficar **Ativo** para prosseguir.

## 2. Cadastro do Projeto
* **Estrutura:** O *Projeto* é criado dentro do *Empreendimento* ativo e é onde se inserem os dados específicos sobre o corte.
* **Vínculo:** O imóvel cadastrado anteriormente deve ser vinculado ao projeto (importando o polígono já desenhado).
* **Responsável Técnico:** Para corte de árvores isoladas, é possível marcar "Não" e gerenciar os documentos por conta própria (diferente de processos de desmate, que exigem RT obrigatório).

## 3. Informações Técnicas da Árvore
* **Dados Dendrométricos:** O sistema solicita o diâmetro (DAP), altura e o fator de forma (ex: 0,71 por convenção) para calcular automaticamente o volume de madeira.
* **Localização:** É obrigatório indicar a coordenada exata da árvore (em graus, minutos e segundos) inserindo manualmente ou marcando diretamente no mapa.
* **Documentação:** O único documento com marcação de preenchimento obrigatório direto no sistema é o **Plano de Exploração**.

## 4. Emissão de Taxa Ambiental (Exemplo: Paraná)
* **Importante:** O Sinaflor não emite a taxa ambiental automaticamente. 
* **Emissão Externa:** No caso do Paraná, deve-se acessar o site do IAP, ir em taxas/boletos e gerar a guia de autorização florestal usando o mesmo CPF cadastrado.
* **Cálculo:** O valor varia conforme o grupo de atividade, área do imóvel (em hectares) e a distância do imóvel até o escritório regional do órgão ambiental.
* **Finalização:** Com o boleto pago e o comprovante em mãos, o projeto deve ser enviado ao órgão ambiental dentro do Sinaflor para gerar o número de protocolo.


