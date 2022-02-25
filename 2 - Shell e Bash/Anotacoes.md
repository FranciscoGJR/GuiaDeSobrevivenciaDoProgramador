# 2 - Shell e Bash

Bash: interpretador de comandos

## Variáveis de Ambiente

---

Printar variáveis: 

- `printenv` - irá mostrar todas as variáveis
- `printenv | grep TESTE` - irá mostrar apenas o valor de uma variável especifica
- `echo $PWD` - irá mostrar apenas o valor de uma variável especifica

Criar variável:

- `export TESTE=10`

> Por convenção, utiliza-se letras maiúsculas para identificar variáveis de ambiente
> 

## Variáveis especiais

---

- `$?` - Código de saída do último comando executado
- `$0..N` - Nésimo argumento (o argumento 0 é o nome do script do jeito que você escreveu para executá-lo).
- `$#` - Número de argumentos passados para o script ou alguma função. Contagem a partir do segundo argumento.
- `$*` - Todos os argumentos como uma única string
- `$@` - Todos os argumentos devidamente separados em strings

## Executar vários comandos

---

- Rodar vários comandos em sequências  `;`
    
    `echo Oi ; cat teste.txt`
    
- Se o 1ª comando executar, o  2ª será executado `&&`
    
    `echo Oi && cat teste.txt`
    
- Se o 1ª comando não executar, o 2ª será executado `||`
    
    `false || cat texto.txt`
    

> Esses comandos podem ser encadeados, ex.: `false && true || cat texto.txt`
> 

## Redirecionar entradas/saídas

---

- Para redirecionar a entra ou saída de um programa para outro, pode-se utilizar `>` ou `<`
    
    `read NOME < nome.txt`
    

> Nesse exemplo, o texto presente em *nome.txt* será redirecionado como a entrada de `read NOME`
> 
- Para concatenar uma a saída de um programa em algum texto, pode-se utilizar `>>`
    
    `echo $NOME >> nome.txt`
    

> Nesse caso, a saída do `echo` será inserida no final do *nome.txt* sem alterar o seu conteúdo
> 
- Pegar a saída de um programa enviar para outro com o `|`
    
    `cat frutas.txt | sort`
    

## ****Globbing****

---

O asterisco `*` é usado para indicar "qualquer coisa" (ex.: `*.c` significa "qualquer coisa que termine em `.c`"  e `saida/*` significa "qualquer coisa que está dentro da pasta `saida/`").

`ls *.c` 

> No exemplo acima, o `ls` irá mostrar apenas os documentos terminados em *.c*
>

