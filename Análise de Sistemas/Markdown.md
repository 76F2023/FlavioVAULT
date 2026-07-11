### 1. Estrutura de título
# Título 1   ← H1 (máximo 1 por página)
## Título 2  ← H2
### Título 3 ← H3
#### Título 4
##### Título 5
###### Título 6


### 2. Ênfases

|Sintaxe|Resultado|
|---|---|
|`*italico*` ou `_italico_`|_italico_|
|`**negrito**` ou `__negrito__`|negrito|
|`***negrito + italico***`|_negrito + italico_|
|`` `código` ``|`código`|
|` ```lang<br>bloco de código``` `|`lang<br>bloco de código`|

### 3. Listas

#### Ordenadas

markdown

```
1. primeiro2. segundo   1. sub‑item   2. sub‑item
```

#### Desordenadas

markdown

```
- item •* item •+ item •
```

#### Tarefas (checkbox) – útil para _to‑do_

markdown

```
- [ ] pendente- [x] concluído
```

### 4. Links e imagens

markdown

```
[texto do link](https://exemplo.com)          ← link externo  [[nome‑da‑página]]                           ← link interno (Obsidian)  ![alt texto](caminho/arquivo.png)            ← imagem local  ![alt texto](https://url.com/ima.png)       ← imagem externa
```

### 5. Tabelas

markdown

```
| Cabeçalho 1 | Cabeçalho 2 ||------------|------------:|| alinh. esq | alinh. direita || centro     |   centrado   |
```

- `:` à esquerda = alinhamento à esquerda
- `:` à direita = alinhamento à direita
- `:` em ambos = centralizado

### 6. Citações (blockquote)

markdown

```
> Esta é uma citação.> > - pode conter listas> - ou **formatação**
```

### 7. Quebra de linha

- Termine a linha com dois espaços seguidos de _Enter_
- Ou use `<br>` (HTML)

### 8. Separadores (horizontal rule)

markdown

```
---   ← 3 ou mais `-`  ***   ← 3 ou mais `*`  ___   ← 3 ou mais `_`
```

### 9. Código embutido

- Inline: `` `código` ``
- Bloco (sem linguagem):
    
    linha 1  
    linha 2
    
- Bloco com destaque:
    
    ````
    ```python  print("Olá")  
    ````
    

### 10. URLs automáticas

markdown

```
<https://exemplo.com>
```

ou simplesmente digite a URL completa (Obsidian transforma em link).

### 11. Escapando caracteres especiais

Prefixe com `\` para que o caractere seja exibido literalmente.  
Ex.: `\*não‑itálico\*` → _não‑itálico_

### 12. Comentários (não renderizados) – útil em notas

markdown

```
%% Este texto será ignorado %%
```
