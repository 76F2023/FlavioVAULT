---
tags:
  - programação
  - lógica
  - algoritmos
  - estudo
  - iniciante
aliases:
  - Lógica de Programação
  - Apostila de Lógica
created: 2026-08-01
author: "@beiamal@gmail.com"
---

# 🧠 Lógica de Programação — Apostila Completa

> [!abstract] Resumo
> Apostila introdutória de **Lógica de Programação** voltada para iniciantes. Cobre desde algoritmos e operadores até estruturas de dados, funções e exercícios resolvidos.

## 📑 Sumário

- [[#1. Algoritmos]]
- [[#2. Operadores]]
- [[#3. Tabela Verdade]]
- [[#4. Variáveis e Tipos]]
- [[#5. Condicionais]]
- [[#6. Laços de Repetição]]
- [[#7. Estruturas de Dados Básicas]]
- [[#8. Funções e Procedimentos]]
- [[#9. Tratamento de Dados]]
- [[#10. Exercícios com Respostas]]
- [[#11. Consulta Rápida]]

---

## 1. Algoritmos

> [!note] Definição
> **Algoritmo** é uma sequência finita de instruções bem definidas para resolver um problema ou executar uma tarefa.

### 🎯 Exemplo do dia a dia — Receita de bolo
1. Pegue a tigela
2. Adicione 2 xícaras de farinha
3. Adicione 1 xícara de açúcar
4. Adicione 3 ovos
5. Misture tudo
6. Leve ao forno por 30 minutos

### 💻 Exemplo em pseudocódigo

```pseudocode
ALGORITMO SomaDoisNumeros
VAR
    numero1, numero2, resultado: REAL
INICIO
    ESCREVA "Digite o primeiro número:"
    LEIA numero1
    ESCREVA "Digite o segundo número:"
    LEIA numero2
    resultado = numero1 + numero2
    ESCREVA "A soma é: ", resultado
FIM
```

> [!tip] Características de um bom algoritmo
> - **Finito**: termina em algum momento
> - **Definido**: cada passo é claro e sem ambiguidade
> - **Efetivo**: cada instrução pode ser executada
> - **Entrada/Saída**: recebe dados e produz resultados

---

## 2. Operadores

> [!info] Conceito
> Operadores são os **tijolos da lógica**. Permitem comparar, calcular e combinar valores.

### 2.1 Operadores Aritméticos

| Operador | Significado         | Exemplo   | Resultado |
|:--------:|---------------------|:---------:|:---------:|
| `+`      | Adição              | `10 + 5`  | `15`      |
| `-`      | Subtração           | `10 - 5`  | `5`       |
| `*`      | Multiplicação       | `10 * 5`  | `50`      |
| `/`      | Divisão             | `10 / 5`  | `2`       |
| `%`/`MOD`| Módulo (resto)      | `10 % 3`  | `1`       |

> [!tip] Uso do operador `%` (módulo)
> - Verificar se é **par**: `num % 2 = 0`
> - Verificar se é **ímpar**: `num % 2 = 1`
> - Verificar **múltiplos**: `num % 5 = 0`

### 2.2 Operadores Relacionais (Comparação)

| Operador | Significado      | Exemplo   | Resultado    |
|:--------:|------------------|:---------:|:------------:|
| `=`      | Igual a          | `5 = 5`   | VERDADEIRO   |
| `<>`/`!=`| Diferente de     | `5 <> 3`  | VERDADEIRO   |
| `>`      | Maior que        | `10 > 5`  | VERDADEIRO   |
| `<`      | Menor que        | `3 < 8`   | VERDADEIRO   |
| `>=`     | Maior ou igual   | `7 >= 7`  | VERDADEIRO   |
| `<=`     | Menor ou igual   | `4 <= 6`  | VERDADEIRO   |

### 2.3 Operadores Lógicos

|  Operador   | Efeito                         | Resulta em VERDADEIRO quando...     |
| :---------: | ------------------------------ | ----------------------------------- |
|  `E` (AND)  | Todas condições verdadeiras    | `(5 > 3) E (10 > 7)` = VERDADEIRO   |
|  `OU` (OR)  | Pelo menos uma verdadeira      | `(5 < 3) OU (10 > 7)` = VERDADEIRO  |
| `NAO` (NOT) | Inverte o valor                | `NAO (5 > 3)` = FALSO               |
| `XOU` (XOR) | Uma, e somente uma, verdadeira | `(5 > 3) XOU (10 < 7)` = VERDADEIRO |

> [!warning] Erros clássicos
> - **Confundir atribuição com comparação**: em C/Java/JS use `==` para comparar e `=` para atribuir.
> - **Trocar AND por OR**: `idade < 18 OU idade > 60` é diferente de `idade >= 18 E idade <= 60`.

---

## 3. Tabela Verdade

> [!danger] DECORE ISSO!
> A tabela verdade é a base de toda decisão em programação.

| A | B | A E B | A OU B | A XOU B | NAO A |
|:-:|:-:|:-----:|:------:|:-------:|:-----:|
| V | V |   V   |   V    |    F    |   F   |
| V | F |   F   |   V    |    V    |   F   |
| F | V |   F   |   V    |    V    |   V   |
| F | F |   F   |   F    |    F    |   V   |

> [!summary] Regras rápidas
> - **E (AND)**: só é verdadeiro se **AMBAS** forem verdadeiras
> - **OU (OR)**: é verdadeiro se **PELO MENOS UMA** for verdadeira
> - **XOU (XOR)**: é verdadeiro se as duas forem **DIFERENTES**
> - **NAO (NOT)**: **inverte** o valor lógico

---

## 4. Variáveis e Tipos

> [!note] Definição
> **Variáveis** são espaços na memória que armazenam valores temporários.

### Tipos primitivos

| Tipo             | Exemplo              | O que armazena                    |
|------------------|----------------------|-----------------------------------|
| `INTEIRO`        | `10, -5, 0`          | Números inteiros (sem decimais)   |
| `REAL`/`FLOAT`   | `3.14, -2.5`         | Números reais (com decimais)      |
| `TEXTO`/`STRING` | `"João"`, `'A'`      | Cadeia de caracteres              |
| `LOGICO`/`BOOL`  | `VERDADEIRO, FALSO`  | Estados lógicos binários          |
| `CARACTERE`      | `'A'`, `'9'`         | Um único caractere                |

### Declaração

```pseudocode
VAR
    idade: INTEIRO
    altura: REAL
    nome: TEXTO
    aprovado: LOGICO
```

> [!tip] Boas práticas
> - Use nomes **significativos** (`idade`, `salario`, `total`)
> - Evite nomes genéricos (`x`, `a`, `temp`)
> - Siga um padrão: `camelCase` ou `snake_case`

---

## 5. Condicionais

> [!info] Conceito
> Permitem que o programa tome **decisões** baseadas em condições.

### 5.1 SE / SENÃO (IF / ELSE)

```pseudocode
SE idade >= 18 ENTÃO
    ESCREVA "Maior de idade"
SENÃO
    ESCREVA "Menor de idade"
FIM SE
```

### 5.2 SENÃO SE (ELSE IF)

```pseudocode
SE nota >= 7 ENTÃO
    ESCREVA "Aprovado"
SENÃO SE nota >= 5 ENTÃO
    ESCREVA "Recuperação"
SENÃO
    ESCREVA "Reprovado"
FIM SE
```

### 5.3 ESCOLHA (CASE / SWITCH)

```pseudocode
ESCOLHA dia
    CASO 1: ESCREVA "Domingo"
    CASO 2: ESCREVA "Segunda-feira"
    ...
    CASO CONTRARIO: ESCREVA "Inválido"
FIM ESCOLHA
```

> [!tip] Quando usar cada um?
> - **SE/SENÃO**: poucas condições ou intervalos
> - **ESCOLHA**: valores discretos e conhecidos (menus, dias, opções)

---

## 6. Laços de Repetição

> [!note] Conceito
> **Loops** executam um bloco de código várias vezes enquanto uma condição for satisfeita.

### 6.1 PARA (FOR) — quando se sabe quantas vezes repetir

```pseudocode
PARA i = 1 ATE 10 PASSO 1
    ESCREVA i
FIM PARA
```

### 6.2 ENQUANTO (WHILE) — quando NÃO se sabe quantas vezes

```pseudocode
ENQUANTO tentativa <> senha E tentativas < 3 FAÇA
    LEIA tentativa
    tentativas = tentativas + 1
FIM ENQUANTO
```

### 6.3 FAÇA ENQUANTO (DO WHILE) — executa pelo menos 1 vez

```pseudocode
FACA
    ESCREVA "1 - Cadastrar  2 - Consultar  3 - Sair"
    LEIA opcao
ENQUANTO opcao <> 3
```

> [!warning] Cuidado com loop infinito!
> Sempre garanta que a condição do loop será **falsa em algum momento**.

### 🔁 Comandos de controle

| Comando     | Função                                        |
|:-----------:|-----------------------------------------------|
| `PARE`      | Sai do loop imediatamente (`break`)           |
| `CONTINUE`  | Pula para a próxima iteração                  |

---

## 7. Estruturas de Dados Básicas

### 7.1 Vetores (Arrays unidimensionais)

```pseudocode
VAR notas: VETOR[1..5] DE REAL
PARA i = 1 ATE 5
    LEIA notas[i]
FIM PARA
```

### 7.2 Matrizes (Arrays bidimensionais)

```pseudocode
VAR matriz: VETOR[1..3][1..3] DE INTEIRO
```

### 7.3 Listas Dinâmicas

```pseudocode
lista = []
lista.adicionar(10)
lista.inserir(1, 15)   // [10, 15, 20]
lista.remover(20)      // [10, 15]
```

### 7.4 Pilhas (LIFO — Last In, First Out)

```pseudocode
pilha.empilhar("A")
pilha.empilhar("B")
topo = pilha.desempilhar()  // Retorna "B"
```

> [!example] Uso real
> Botão **voltar** do navegador, desfazer/refazer (`Ctrl+Z`).

### 7.5 Filas (FIFO — First In, First Out)

```pseudocode
fila.enfileirar("Cliente 1")
fila.enfileirar("Cliente 2")
proximo = fila.desenfileirar()  // Retorna "Cliente 1"
```

> [!example] Uso real
> Fila de impressão, atendimento bancário, processamento de pedidos.

### 7.6 Dicionários (Mapas / Chave-Valor)

```pseudocode
agenda["João"] = "9999-1111"
agenda["Maria"] = "9999-2222"
telefone = agenda["João"]
```

> [!tip] Comparativo rápido

| Estrutura   | Ordem        | Acesso      | Uso típico              |
|-------------|--------------|-------------|-------------------------|
| Vetor       | Indexado     | `O(1)`      | Listas fixas            |
| Lista       | Indexado     | `O(n)`      | Listas dinâmicas        |
| Pilha       | LIFO         | Topo        | Histórico, desfazer     |
| Fila        | FIFO         | Início      | Agendamentos            |
| Dicionário  | Por chave    | `O(1)`      | Buscas rápidas          |

---

## 8. Funções e Procedimentos

> [!note] Diferença
> - **Procedimento**: executa uma ação, **não retorna** valor
> - **Função**: executa uma ação e **retorna** um valor

### 8.1 Procedimento

```pseudocode
PROCEDIMENTO ExibirCabecalho(titulo: TEXTO)
INICIO
    ESCREVA "========================"
    ESCREVA "  ", titulo
    ESCREVA "========================"
FIM PROCEDIMENTO
```

### 8.2 Função

```pseudocode
FUNCAO CalcularMedia(n1, n2, n3: REAL): REAL
VAR media: REAL
INICIO
    media = (n1 + n2 + n3) / 3
    RETORNE media
FIM FUNCAO
```

### 8.3 Função com validação

```pseudocode
FUNCAO VerificarPar(numero: INTEIRO): LOGICO
INICIO
    SE numero % 2 = 0 ENTÃO
        RETORNE VERDADEIRO
    SENÃO
        RETORNE FALSO
    FIM SE
FIM FUNCAO
```

### 8.4 Recursividade

> [!tip] Conceito
> Função que **chama a si mesma**. Útil para problemas divisíveis em subproblemas menores.

```pseudocode
FUNCAO Fatorial(n: INTEIRO): INTEIRO
INICIO
    SE n <= 1 ENTÃO
        RETORNE 1
    SENÃO
        RETORNE n * Fatorial(n - 1)
    FIM SE
FIM FUNCAO
```

> [!warning] Cuidado!
> Toda função recursiva precisa de um **caso base**, senão vira loop infinito.

---

## 9. Tratamento de Dados

### 9.1 Conversões entre tipos

```pseudocode
textoNumero = "42"
numeroInteiro = CONVERTER_PARA_INTEIRO(textoNumero)
numeroReal = CONVERTER_PARA_REAL(numeroInteiro)
```

### 9.2 Manipulação de Strings

| Função              | O que faz                         |
|---------------------|-----------------------------------|
| `COMPRIMENTO(s)`    | Retorna o tamanho da string       |
| `SUBSTRING(s,i,f)`  | Extrai parte da string            |
| `PARA_MAIUSCULO(s)` | Converte para maiúsculas          |
| `PARA_MINUSCULO(s)` | Converte para minúsculas          |
| `CONTEM(s, sub)`    | Verifica se contém substring      |
| `CARACTERE(s, i)`   | Retorna caractere na posição `i`  |

### 9.3 Funções com Datas

```pseudocode
dataAtual = DATA_ATUAL()
dataNasc = CRIAR_DATA(1990, 5, 15)
ESCREVA "Ano: ", ANO(dataNasc)
ESCREVA FORMATAR_DATA(dataAtual, "dd/mm/yyyy")
```

---

## 10. Exercícios com Respostas

### ✅ Exercício 1 — Par ou Ímpar

> [!question] Enunciado
> Leia um número e informe se é par ou ímpar.

<details>
<summary>Ver resposta</summary>

```pseudocode
ALGORITMO ParImpar
VAR num: INTEIRO
INICIO
    LEIA num
    SE num % 2 = 0 ENTÃO
        ESCREVA num, " é par."
    SENÃO
        ESCREVA num, " é ímpar."
    FIM SE
FIM
```

</details>

---

### ✅ Exercício 2 — Maior de Três

> [!question] Enunciado
> Leia três valores e retorne o maior.

<details>
<summary>Ver resposta</summary>

```pseudocode
ALGORITMO MaiorDeTres
VAR a, b, c, maior: REAL
INICIO
    LEIA a, b, c
    maior = a
    SE b > maior ENTÃO maior = b FIM SE
    SE c > maior ENTÃO maior = c FIM SE
    ESCREVA "O maior número é: ", maior
FIM
```

</details>

---

### ✅ Exercício 3 — Média de Notas com Aprovação

> [!question] Enunciado
> Leia 4 notas, calcule a média e informe: Aprovado (≥7), Recuperação (≥5) ou Reprovado.

<details>
<summary>Ver resposta</summary>

```pseudocode
ALGORITMO MediaAluno
VAR notas: VETOR[1..4] DE REAL
    soma, media: REAL
    i: INTEIRO
INICIO
    soma = 0
    PARA i = 1 ATE 4
        LEIA notas[i]
        soma = soma + notas[i]
    FIM PARA
    media = soma / 4
    SE media >= 7 ENTÃO
        ESCREVA "Aprovado"
    SENÃO SE media >= 5 ENTÃO
        ESCREVA "Recuperação"
    SENÃO
        ESCREVA "Reprovado"
    FIM SE
FIM
```

</details>

---

### ✅ Exercício 4 — Tabuada

> [!question] Enunciado
> Exiba a tabuada de 1 a 10 de um número informado.

<details>
<summary>Ver resposta</summary>

```pseudocode
ALGORITMO Tabuada
VAR numero, i: INTEIRO
INICIO
    LEIA numero
    PARA i = 1 ATE 10 PASSO 1
        ESCREVA numero, " x ", i, " = ", numero * i
    FIM PARA
FIM
```

</details>

---

### ✅ Exercício 5 — Fatorial

> [!question] Enunciado
> Calcule o fatorial de N.

<details>
<summary>Ver resposta</summary>

```pseudocode
FUNCAO Fatorial(n: INTEIRO): INTEIRO
VAR resultado, i: INTEIRO
INICIO
    resultado = 1
    PARA i = 1 ATE n
        resultado = resultado * i
    FIM PARA
    RETORNE resultado
FIM FUNCAO
```

</details>

---

### ✅ Exercício 6 — Fibonacci

> [!question] Enunciado
> Exiba os N primeiros termos da sequência de Fibonacci.

<details>
<summary>Ver resposta</summary>

```pseudocode
ALGORITMO Fibonacci
VAR n, i, atual, anterior, proximo: INTEIRO
INICIO
    LEIA n
    anterior = 0
    atual = 1
    PARA i = 1 ATE n
        ESCREVA anterior
        proximo = anterior + atual
        anterior = atual
        atual = proximo
    FIM PARA
FIM
```

</details>

---

### ✅ Exercício 7 — Contador de Vogais

> [!question] Enunciado
> Conte quantas vogais há em uma string.

<details>
<summary>Ver resposta</summary>

```pseudocode
ALGORITMO ContarVogais
VAR texto: TEXTO
    i, contador, tam: INTEIRO
    letra: CARACTERE
INICIO
    LEIA texto
    contador = 0
    tam = COMPRIMENTO(texto)
    PARA i = 0 ATE tam - 1
        letra = CARACTERE(texto, i)
        SE letra = 'a' OU letra = 'e' OU letra = 'i' 
           OU letra = 'o' OU letra = 'u' ENTÃO
            contador = contador + 1
        FIM SE
    FIM PARA
    ESCREVA "Vogais: ", contador
FIM
```

</details>

---

### ✅ Exercício 8 — Inverter String

> [!question] Enunciado
> Leia uma string e exiba-a invertida.

<details>
<summary>Ver resposta</summary>

```pseudocode
ALGORITMO InverterString
VAR original, invertida: TEXTO
    i, tamanho: INTEIRO
INICIO
    LEIA original
    invertida = ""
    tamanho = COMPRIMENTO(original)
    PARA i = tamanho - 1 ATE 0 PASSO -1
        invertida = invertida + CARACTERE(original, i)
    FIM PARA
    ESCREVA invertida
FIM
```

</details>

---

### ✅ Exercício 9 — Verificador de Número Primo

> [!question] Enunciado
> Verifique se um número é primo.

<details>
<summary>Ver resposta</summary>

```pseudocode
FUNCAO EhPrimo(n: INTEIRO): LOGICO
VAR i: INTEIRO
INICIO
    SE n < 2 ENTÃO RETORNE FALSO FIM SE
    PARA i = 2 ATE RAIZ_QUADRADA(n) PASSO 1
        SE n % i = 0 ENTÃO RETORNE FALSO FIM SE
    FIM PARA
    RETORNE VERDADEIRO
FIM FUNCAO
```

</details>

---

### ✅ Exercício 10 — Jogo da Adivinhação

> [!question] Enunciado
> Sorteie um número de 1 a 100 e dê dicas "maior" ou "menor" até o usuário acertar.

<details>
<summary>Ver resposta</summary>

```pseudocode
ALGORITMO JogoAdivinhacao
VAR secreto, palpite, tentativas: INTEIRO
INICIO
    secreto = SORTEAR(1, 100)
    tentativas = 0
    REPITA
        ESCREVA "Seu palpite:"
        LEIA palpite
        tentativas = tentativas + 1
        SE palpite < secreto ENTÃO
            ESCREVA "Maior!"
        SENÃO SE palpite > secreto ENTÃO
            ESCREVA "Menor!"
        SENÃO
            ESCREVA "Acertou em ", tentativas, " tentativas!"
        FIM SE
    ATE palpite = secreto
FIM
```

</details>

---

## 11. Consulta Rápida

> [!summary] Operadores — Resumo
> - **Aritméticos**: `+`, `-`, `*`, `/`, `%`
> - **Relacionais**: `=`, `<>`, `>`, `<`, `>=`, `<=`
> - **Lógicos**: `E`, `OU`, `NAO`, `XOU`

> [!summary] Estruturas de controle
> - **Condicionais**: `SE`, `SENÃO SE`, `SENÃO`, `ESCOLHA`
> - **Loops**: `PARA`, `ENQUANTO`, `FAÇA ENQUANTO`, `REPITA...ATE`

> [!summary] Estruturas de dados
> - **Vetor/Matriz**: acesso por índice
> - **Lista**: dinâmica
> - **Pilha**: LIFO
> - **Fila**: FIFO
> - **Dicionário**: chave-valor

---

## 📌 Extras — Conceitos Importantes

### 🧩 Fluxograma
> Representação **gráfica** de um algoritmo usando símbolos padronizados (início, processo, decisão, fim).

### 🎯 Pseudocódigo (Portugol)
> Linguagem **intermediária** entre o português e o código real. Ideal para aprender lógica antes de partir para uma linguagem específica.

### 🐞 Debugging
> Processo de **encontrar e corrigir erros** no código. Dicas:
> - Use `ESCREVA` para rastrear valores
> - Teste com casos extremos (0, negativos, vazios)
> - Leia a mensagem de erro com atenção

### 📐 Complexidade (noção básica)
> Medida de **quão eficiente** é um algoritmo:
> - `O(1)` — constante
> - `O(log n)` — logarítmico
> - `O(n)` — linear
> - `O(n²)` — quadrático

### 💡 Dicas de Estudo
1. **Pratique todos os dias** — nem que seja 20 minutos
2. **Resolva exercícios** antes de olhar a resposta
3. **Desenhe fluxogramas** antes de codificar
4. **Explique em voz alta** o que o código faz (técnica do *rubber duck*)
5. **Leia código de outros** para aprender novos padrões

---

> [!quote] 💭
> *"Programar não é sobre decorar sintaxe — é sobre aprender a pensar."*

---

## 🔗 Relacionadas
- [[Linguagens de Programação]]
- [[Estruturas de Dados]]
- [[Algoritmos de Ordenação]]
- [[Boas Práticas de Código]]
