## Seção 1

Resposta 1: antes de tudo, faz-se necessário instalar o utilitário *zip* na máquina, rodando o sequinte comando: `sudo apt-get install zip`. Em seguida, uma forma de realizar a compatação dos 2 arquivos .txt, da pasta *codigos* e seus reeespectivos arquivos, é utilizar o seguinte comando: `zip entregas.zip tarefa_1.txt tarefa_2.txt codigos/*`.

Resposta 2: para descompactar todos os arquivos e pastas utilizando o utilitário *unzip*, é necessário utilizar o comando `unzip -l entregas.zip`.

## Seção 2

Resposta 1: 
*Textos
em arquivos
separados*

Resposta 2: pode ser utlizado o comando `strings -n 20 ./executavel/*`, que resulta na seguinte saída:
/lib64/ld-linux-x86-64.so.2

_ITM_deregisterTMCloneTable

_ITM_registerTMCloneTable

----- Text0 sup3r secr3to -----

deregister_tm_clones

__do_global_dtors_aux

__do_global_dtors_aux_fini_array_entry

__frame_dummy_init_array_entry

_GLOBAL_OFFSET_TABLE_

_ITM_deregisterTMCloneTable

__libc_start_main@GLIBC_2.2.5

_ITM_registerTMCloneTable

__cxa_finalize@GLIBC_2.2.5*

## Seção 3

Resposta 1: foi utilizado o comando `find ./ -name anotacoes_perdidas.txt`, em que foi retornado o diretório *./muitas_pastas/k/w/u/anotacoes_perdidas.txt*, este onde encontra-se o arquivo *.txt* em questão.

Resposta 2: para identificar apenas os arquivos maiores que 100k, pode-se utilizar o comando `find ./ -size +100k`, que retornará o diretório *./x/m/v/trabalho_final.java*.

Resposta 3: usando o comando `grep --recursive "guia de sobrevivencia do programador" ./`, encontramos a strings em *texto_5.txt* e *texto_2.txt*

## Seção 4

Resposta 1: <!-- Sua resposta vem aqui -->

Resposta 2: <!-- Sua resposta vem aqui -->

Resposta 3: <!-- Sua resposta vem aqui -->
