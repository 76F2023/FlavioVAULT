# Levantamento de Requisitos

> Módulo 4 · Descoberta de Sistemas Levantar é a etapa em que a descoberta qualitativa se transforma em material concreto para especificar o sistema.

## O que é

Levantamento de requisitos (elicitação) é o processo de descobrir, entender e registrar o que as pessoas precisam, o que o sistema deve fazer e sob quais condições ele deve operar.

- Sinônimos: elicitação, coleta, levantamento.
- É a primeira etapa dentro da [[Engenharia de Requisitos]].
- Não é apenas "perguntar o que o usuário quer" — é investigar, observar e validar.

> Ideia central: os usuários raramente conseguem descrever o problema completo. Nosso papel é juntar fragmentos de informação de várias fontes e transformá-los em requisitos claros.

---

## Objetivo

- Entender o problema real, não a solução imaginada.
- Identificar necessidades, dores, restrições e expectativas.
- Criar base para:
    - Priorizar funcionalidades ([[Técnicas de Priorização]]);
    - Especificar requisitos de forma mensurável;
    - Validar suposições antes de investir em desenvolvimento.

---

## Fontes de informação

O levantamento não depende de uma única fonte. As principais:

|Fonte|O que fornece|Notas relacionadas|
|---|---|---|
|Stakeholders|visão de negócio, metas, regras|[[Alinhamentos e Briefing]]|
|Usuários|contexto real, dor, expectativa|[[Entrevistas]], [[Observação]]|
|Documentos|processos, normas, métricas existentes|[[Desk Research]]|
|Sistemas legados|o que já funciona/falha hoje|[[Benchmarking]]|
|Mercado|concorrência, padrões, tendências|[[Benchmarking]]|
|Suposições do time|hipóteses para validar|[[Matriz CSD]]|

---

## Técnicas de levantamento

### 1. Entrevistas

- O que é: conversa semiestruturada, individual ou em grupo.
- Quando usar: para entender profundidade, contexto e motivação.
- Ver também: [[Entrevistas]]

### 2. Observação

- O que é: acompanhar o usuário realizando a tarefa no ambiente real.
- Quando usar: para captar o que as pessoas fazem, não o que dizem.
- Ver também: [[Observação]]

### 3. Questionários / Surveys

- O que é: perguntas padronizadas para muitas pessoas.
- Quando usar: para quantificar frequência, preferência ou alcance.
- Cuidado: resultado amplo, mas raso.

### 4. Workshops / Dinâmicas

- O que é: sessão colaborativa com stakeholders para levantar e convergir.
- Exemplos: [[Design Studio]], [[Design Studio na Prática]], [[Crazy 8's]].
- Quando usar: quando há divergência de visões e é preciso alinhar.

### 5. Análise de documentos

- O que é: revisão de manuais, processos, relatórios, normas.
- Quando usar: para entender regras de negócio e restrições legais.
- Ver também: [[Desk Research]]

### 6. Prototipação como levantamento

- O que é: criar versões simples para provocar feedback.
- Quando usar: quando o requisito está vago — o protótipo revela o que a pessoa realmente espera.
- Ver também: [[Prototipação: Design Sprint]], [[Processo de Design Thinking]]

### 7. Contexto e imersão

- Personas → identifica quem precisa.
- [[Jobs to be Done]] → identifica o "trabalho" que o usuário quer realizar.
- [[Mapa de Empatia]] → revela o que pensa, sente, vê, fala e faz.

---

## Processo prático

1. Planejar
    
    - Definir objetivo do levantamento.
    - Mapear stakeholders e fontes.
    - Escolher as técnicas (combinar, não usar uma só).
2. Coletar
    
    - Entrevistas, observação, documentos, workshops.
    - Registrar evidências (áudio, fotos, quadros, post-its).
3. Sintetizar
    
    - Agrupar achados por tema.
    - Separar fatos de suposições → [[Matriz CSD]].
    - Identificar necessidades latentes.
4. Validar
    
    - Voltar aos usuários e stakeholders.
    - Confirmar interpretação antes de especificar.
5. Documentar
    
    - Transformar achados em requisitos.
    - Manter rastreabilidade (de onde veio cada requisito).

---

## Boas práticas

- Combine técnicas: entrevista + observação + documento = visão mais completa.
- Separe problema de solução: o usuário descreve a solução; você investiga o problema.
- Pergunte "por quê?" — use os [[5 Porquês]] para chegar à causa raiz.
- Registre a origem: cada requisito precisa ter uma fonte rastreável.
- Valide cedo: não espere o final para confirmar com o usuário.
- Envolva diferentes perfis: usuário final, área de negócio, tecnologia, operação.

---

## Armadilhas comuns

- 🚫 Aceitar a primeira resposta como verdade absoluta.
- 🚫 Ouvir só o stakeholder de maior cargo e ignorar o usuário real.
- 🚫 Confundir opinião com requisito — opinião vira hipótese.
- 🚫 Pular a validação e partir direto para a especificação.
- 🚫 Usar uma única técnica e achar que o levantamento está completo.

---

## Conexões com a Descoberta

- [[Entrevistas]] e [[Observação]] → técnicas centrais do levantamento.
- [[Desk Research]] → fonte documental e de mercado.
- [[Matriz CSD]] → organiza certezas, suposições e dúvidas.
- [[Persona]] e [[Jobs to be Done]] → definem quem e o quê investigar.
- [[Técnicas de Priorização]] → decidem o que aprofundar primeiro.
- [[Engenharia de Requisitos]] → etapa seguinte: analisar, especificar, validar e gerenciar.

---

## Referências

- Ver referências da nota [[Engenharia de Requisitos]].
- Notas de apoio do módulo: [[Entrevistas]], [[Observação]], [[Desk Research]], [[Matriz CSD]].
- Material do módulo 4 — Descoberta de Sistemas.

---

_Nota criada para o cofre Obsidian — Módulo 4: Descoberta de Sistemas._