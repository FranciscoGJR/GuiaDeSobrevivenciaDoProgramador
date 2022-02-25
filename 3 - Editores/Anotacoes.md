# 3 - Editores

# ⛔ VIM

---

## Modo NORMAL

---

### Movimentação

---

- Movimentar o curso por **caractere:** `h` (esquerda), `j` (baixo), `k` (cima), `l` (direita).
- Movimentar o curso por **palavra:**`w` (início da próxima palavra), `e` (final da próxima palavra), `b` (começo da palavra anterior).
- Movimentar o curso pela **linha**: `0` (início da linha), `$` (final da linha).
- Movimentar por **arquivo**: `gg` (início do arquivo), `G` (final do arquivo), `_G` ( _ sendo a linha), `_%` (tantos % do arquivo)

> Toda movimentação pode receber uma quantidade antes que indica quantas vezes será repetida. Ex: `4j` ou `50l`
> 

### Desfazer e refazer

---

- Desfazer: `u`
- Refazer: `^R`

### Deletar

---

- Deletar por movimento: `d` + movimento (`h-j-k-l`)
- Deletar linha inteira: `dd`
- Deletar até o final da linha: `D`
- Substituir uma letra por outra: `r_` (_ sendo a nova letra)

## **Copiar e Colar**

---

- Copiar por movimento: `y` + movimento (`h-j-k-l`)
- Copiar linha inteira: `Y` ou `yy`
- Colar antes do cursor: `P`
- Colar depois do cursor: `p`

## **Procurar por texto**

---

- Procurar ocorrências depois do cursor: `/` + padrão de pesquisa + Enter
- Procurar ocorrências antes do cursor: `?` + padrão de pesquisa + Enter

## Modo Inserção

---

- Inserir antes do cursor: `i`
- Inserir antes do primeiro caractere que não é whitespace na linha: `I`
- Adicionar ao final do cursor: `a`
- Adicionar ao final da linha: `A`
- “Autocomplete”: `^n`

> `^n` desce entre as palavras repetidas, `^p` sobe
> 

### ****Modo visual****

---

- Ativar modo visual por caractere: `v`
- Ativar modo visual por linha: `V`
- Ativar modo visual por coluna: `^V`

### ****Modo de comandos****

---

- Ativar modo: `:`
- Sair e salvar: `wq`

