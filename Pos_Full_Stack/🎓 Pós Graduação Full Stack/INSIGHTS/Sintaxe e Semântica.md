## Sintaxe

A sintaxe é o conjunto de regras que determina como os símbolos de uma linguagem (palavras, sinais, tokens) podem ser combinados para formar estruturas válidas. Ela não se preocupa com o significado dessas estruturas, apenas com a sua forma correta.

- Linguística: regula a ordem das palavras nas frases (por exemplo, em português a ordem típica _Sujeito – Verbo – Objeto_).
- Programação: define a gramática da linguagem (por exemplo, a declaração de uma variável em JavaScript é `let nome = "Ana";` – a palavra‑chave `let`, seguida de um identificador, do operador `=` e de um valor).
- Exemplo de sintaxe incorreta:
    - Linguística: _“casa bonita a é”_ (ordem das palavras quebra a regra do português).
    - Código: `if (x > 0 console.log(x);` – falta o parêntese de fechamento.

Em resumo, a sintaxe responde à pergunta “Esta construção está bem‑formada?”.

---

## Semântica

A semântica trata do significado das construções que obedecem à sintaxe. Enquanto a sintaxe verifica a forma, a semântica verifica o conteúdo e a lógica por trás dela.

- Linguística: interpreta o sentido da frase (ex.: _“O gato está na caixa”_ descreve a localização de um gato).
- Programação: determina o que o código faz quando executado (ex.: a instrução `let x = 5;` cria uma variável `x` cujo valor é 5; a expressão `x / 0` tem semântica de erro de divisão por zero).
- Exemplo de semântica incorreta (mas sintaticamente correta):
    - Linguística: _“O cachorro comeu o carro.”_ – frase gramatical, mas o sentido é ilógico no mundo real.
    - Código: `let idade = -10;` – a sintaxe está correta, mas o valor negativo pode ser semânticamente inválido para representar idade.

Em resumo, a semântica responde à pergunta “O que isso significa ou que efeito tem?”.

---

### Resumindo a diferença

|Aspecto|Sintaxe|Semântica|
|---|---|---|
|O que verifica|Estrutura/formato corretos|Significado/efeito das estruturas|
|Foco|Regras de combinação de símbolos|Interpretação e validade do conteúdo|
|Erro típico|Erro de compilação ou gramática|Erro lógico ou de domínio (runtime)|
|Exemplo (código)|`if (x > 0) { console.log(x); }` – está bem‑formado|Se `x` for uma string, a comparação pode não fazer sentido no contexto da aplicação|

Esses conceitos são fundamentais tanto em linguística quanto em ciência da computação, pois permitem separar como algo é escrito (sintaxe) de o que aquilo representa ou executa (semântica).