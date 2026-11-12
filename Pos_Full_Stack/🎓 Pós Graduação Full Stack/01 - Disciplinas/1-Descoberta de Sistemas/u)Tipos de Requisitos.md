tipo: aula curso: Pós-Graduação em Desenvolvimento de Software Full Stack disciplina: Descoberta de Sistemas data: 2026-11-04 fontes:

- "[[Desenvolvimento de Software Centrado no Usuário]]"
- "[[Descoberta de Sistemas]]" tags:
- aula
- requisitos
- engenharia-de-requisitos

---

# Tipos de Requisitos

## Resumo

Os achados do Levantamento de Requisitos só viram especificação útil quando são classificados. A aula separa os requisitos em três grandes grupos — funcionais, não funcionais e regras de negócio — e mostra como essa classificação influencia priorização, escrita e validação.

## Conceitos principais

- Requisito funcional: o que o sistema faz — comportamento, funcionalidades e transformações de entrada em saída.
- Requisito não funcional: como o sistema se comporta — qualidades como desempenho, segurança, usabilidade e acessibilidade.
- Regra de negócio: restrição ou diretriz imposta pela organização, independente do sistema.
- Requisito de usuário × requisito de sistema: o primeiro expressa a necessidade em linguagem do negócio; o segundo descreve o comportamento técnico que a atende.

## Conteúdo da aula

### 1. Requisitos funcionais

Descrevem capacidades concretas, sempre ligadas a um ator + ação + objeto:

- O usuário cadastra um pedido de compra.
- O sistema envia notificação quando o pagamento é aprovado.
- O administrador exporta o relatório em CSV.

Características:

- Respondem a "o que o sistema deve fazer?".
- São os mais fáceis de perceber e testar.
- Viram casos de uso, histórias de usuário e critérios de aceite.

### 2. Requisitos não funcionais

Definem qualidades e restrições globais do sistema. Não aparecem como "botão" ou "tela", mas determinam a experiência e a viabilidade técnica.

|Categoria|Exemplo|
|---|---|
|Desempenho|A tela de listagem carrega em até 2 segundos.|
|Segurança|Senhas armazenadas com hash e salt.|
|Usabilidade|O usuário conclui o cadastro em menos de 5 minutos.|
|Acessibilidade|Contraste mínimo WCAG AA em todos os textos.|
|Disponibilidade|O sistema fica indisponível no máximo 1% do mês.|
|Compatibilidade|Funciona nos navegadores Chrome e Firefox atuais.|

Características:

- Respondem a "como o sistema deve ser?".
- Costumam ser mensuráveis — todo adjetivo vago ("rápido", "fácil") vira uma métrica.
- Quando ignorados, geram retrabalho caro, porque atravessam todo o sistema.

### 3. Regras de negócio

São restrições que existem fora do sistema, definidas pela organização, legislação ou mercado:

- Pedidos acima de R$ 5.000 exigem aprovação de gerência.
- Cliente inadimplente não pode parcelar em mais de 3 vezes.
- O frete é grátis para compras acima de R$ 200.

Características:

- O sistema não cria a regra — ele a cumpre.
- Mudam por decisão de negócio, não por decisão técnica.
- Precisam ser explicitadas: muitas vezes estão implícitas na cabeça de stakeholders.

### 4. Requisito de usuário × requisito de sistema

Essa distinção evita misturar o quê com como:

- Requisito de usuário: "Quero acompanhar meus pedidos em tempo real."
- Requisito de sistema: "O sistema deve atualizar o status do pedido em até 5 segundos após cada evento de mudança, via API de eventos."

### 5. Por que classificar importa

- Priorização: requisito não funcional crítico (segurança) pode valer mais que vários funcionais.
- Escrita: cada tipo pede um vocabulário e um nível de detalhe diferente.
- Rastreabilidade: conecta o requisito à sua fonte (entrevista, documento, regra).
- Teste: funcional gera caso de teste; não funcional gera métrica e critério de aceite.

## Conexões com as leituras

- Engenharia de Requisitos ([[Engenharia de Requisitos]]): a classificação é a etapa de análise — organiza o que foi levantado antes de especificar.
- Levantamento de Requisitos ([[Levantamento de Requisitos]]): as fontes de informação geram os três tipos; uma única entrevista pode revelar regra de negócio e necessidade funcional.
- Descoberta de Sistemas: tipificar os achados evita tratar opinião de stakeholder como requisito funcional.

## Exemplos e aplicações

- E-commerce: "comprar com 1 clique" (funcional), "checkout em 3 passos" (usabilidade/não funcional), "cupom válido apenas em primeira compra" (regra de negócio).
- Fintech: "transferir via Pix" (funcional), "transação concluída em até 10 segundos" (não funcional), "limite de R$ 4.000 para Pix noturno" (regra de negócio).

## Dúvidas para revisar

- [ ]  Como separar regra de negócio de requisito funcional quando a regra é exclusiva do sistema?

## Aprendizados

- Requisito não é um bloco único: o mesmo achado pede tratamento diferente conforme o tipo.
- Todo requisito não funcional precisa de uma métrica.
- Regra de negócio vem da organização, não do software.

## Próximos passos

- [ ]  Revisar a nota [[Engenharia de Requisitos]] e aplicar a classificação nos exemplos.
- [ ]  Classificar requisitos de um caso real do módulo.

## Referências

- PRESSMAN, Roger S.; MAXIM, Bruce R. Engenharia de Software: uma abordagem profissional. 9. ed. Porto Alegre: AMGH, 2021. (Capítulos sobre requisitos).
- SOMMERVILLE, Ian. Engenharia de Software. 10. ed. São Paulo: Pearson, 2019.
- WIEGERS, Karl; BEATTY, Joy. Software Requirements. 3. ed. Redmond: Microsoft Press, 2013.