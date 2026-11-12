tipo: aula curso: Pós-Graduação em Desenvolvimento de Software Full Stack disciplina: data: 2026-11-04 fontes:

- "[[Desenvolvimento de Software Centrado no Usuário]]"
- "[[Descoberta de Sistemas]]" tags:
- aula
- estudo
- requisitos
- documentacao

---

# Especificação e DDR

## Resumo

A especificação transforma os requisitos levantados e analisados em uma base documental clara, completa e verificável. O DDR (Documento de Definição de Requisitos) é o artefato que consolida essa especificação — reunindo escopo, stakeholders, requisitos funcionais, não funcionais e regras de negócio com rastreabilidade e critérios de aceite.

## Conceitos principais

- Especificação de requisitos: processo de documentar os requisitos de forma a permitir que desenvolvedores, testadores e clientes entendam exatamente o que será construído.
- DDR (Documento de Definição de Requisitos): artefato formal que descreve o que o sistema deve fazer, sem definir _como_ será implementado.
- Atributo de qualidade de um requisito: não ambíguo, completo, consistente, verificável, priorizado e rastreável.
- Requisito de usuário vs. requisito de sistema: o primeiro expressa necessidade do negócio; o segundo detalha comportamento técnico mensurável.

## Conteúdo da aula

### O papel da especificação

- Fecha o ciclo iniciado na [[Engenharia de Requisitos]]: elicitação → análise → especificação → validação → gerenciamento.
- Serve de contrato entre stakeholders, time de desenvolvimento e área de testes.
- Evita retrabalho: requisito mal escrito custa caro quando descoberto tardiamente.

### Estrutura típica do DDR

1. Introdução — propósito, escopo do documento e do sistema.
2. Visão geral — contexto do produto e objetivos de negócio.
3. Stakeholders e usuários — perfis, papéis e necessidades.
4. Requisitos funcionais — o que o sistema faz (ver [[Tipos de Requisitos]]).
5. Requisitos não funcionais — desempenho, segurança, usabilidade, acessibilidade.
6. Regras de negócio — restrições da organização.
7. Rastreabilidade — origem e vínculo de cada requisito com as fontes (ver [[Levantamento de Requisitos]]).
8. Critérios de aceite — condição objetiva que define "pronto".
9. Glossário e referências — termos do domínio e documentos de apoio.

### Como escrever um bom requisito

- Um requisito por frase — não misturar ideias.
- Fórmula: _ator + ação + objeto + condição/critério_.
- Evitar ambiguidade: substituir "rápido", "fácil", "seguro" por medidas concretas.
- Exemplo:
    - ❌ "O sistema deve ser rápido ao carregar a lista de pedidos."
    - ✅ "O sistema deve exibir a lista de pedidos em até 2 segundos para 10.000 registros."

### Critérios de aceite

- Escritos antes do desenvolvimento, validando cada requisito.
- Formato comum: _Dado / Quando / Então_ (ou checklist verificável).
- Exemplo: "Dado um usuário autenticado, quando ele filtra por status 'aberto', então apenas pedidos abertos são exibidos."

### Ferramentas e boas práticas

- Ferramentas: wikis, rastreadores de requisitos, softwares de versionamento.
- Boas práticas:
    - Priorizar antes de detalhar (ver [[Técnicas de Priorização]]).
    - Manter versão e histórico de mudanças.
    - Revisar com stakeholders e usuários.
    - Ligar cada requisito a um caso de teste.

### DDR × casos de uso × histórias de usuário

- DDR descreve os requisitos de forma abrangente.
- Casos de uso detalham interações do ator com o sistema.
- Histórias de usuário são leves, de perspectiva do usuário, comumente complementadas por critérios de aceite.

## Conexões com as leituras

- Engenharia de Requisitos: a especificação é a terceira etapa do fluxo ER.
- Tipos de Requisitos: orienta a classificação dentro do DDR.
- Levantamento de Requisitos: garante a rastreabilidade da origem.
- Técnicas de Priorização: define a ordem em que os requisitos aparecem no documento.

## Exemplos e aplicações

- Pedido de compra: requisito funcional "cadastrar pedido com múltiplos itens", não funcional "processar checkout em até 3s", regra de negócio "pedido acima de R$ 500 exige aprovação".
- App de delivery: "usuário rastreia entregador em tempo real" (funcional), "mapa atualiza a cada 30s" (não funcional).

## Dúvidas para revisar

- [ ]  Diferença prática entre DDR e documento de arquitetura?
- [ ]  Quando usar história de usuário em vez de requisito formal?

## Aprendizados

- Especificação bem feita reduz ambiguidade e retrabalho.
- O DDR deve descrever o _quê_, nunca o _como_.
- Critérios de aceite transformam requisito em algo testável.

## Próximos passos

- [ ]  Praticar descrição de requisitos com a fórmula ator + ação + objeto + critério.
- [ ]  Revisar o DDR de um projeto de estudo usando [[Tipos de Requisitos]].

## Referências

- [[Engenharia de Requisitos]]
- [[Levantamento de Requisitos]]
- [[Tipos de Requisitos]]
- [[Técnicas de Priorização]]
- ISO/IEC/IEEE 29148 — Requisitos e avaliação de sistemas e software
- IEEE 830 — Especificação de Requisitos de Software (SRS)