# 4 - Manipulação De Dados

## ****Manipulações básicas e padrões de texto com `grep`**

---

Com o `grep` é passível coletar alguns dados específicos em um documento de texto. Ao utilizar tal comando, é retornado todas as ocorrências definidas como parâmetro

- Ocorrências em documentos de texto

```bash
grep 'banana' vendas.txt                                        # retorna todas as ocorrências ‘banana’
grep 'banana' vendas.txt | wc -l                                # retorna a quantidade ocorrências ‘banana’
grep 'banana' vendas.txt | wc -l >> tatalVendas.txt             **# concatena a quantidade de bananas no arquivo totalVendas.txt**

cat vendas.txt | grep 'banana'                                  # retorna todas as ocorrências ‘banana’
cat vendas.txt | grep 'banana' | wc -l                          # retorna a quantidade ocorrências ‘banana’
**cat cendas.txt | grep 'banana' | wc -l >> totalVendas.txt       # concatena a quantidade de bananas no arquivo totalVendas.txt**
```

- Ocorrências em diretórios

```bash
ls -l | grep '.txt'                          # retorna a quantidade de arquivos terminados .txt
```

## API - `curl`

---

- Acessar API de CEP

```bash
curl -X GET 'viacep.com.br/ws/68555161/json'
```

- Filtrar informações do objeto em *json com o* `jq`

```bash
curl -X GET 'viacep.com.br/ws/68555161/json' | jq .logradouro
```

> Irá retornar apenas o logradouro do objeto selecionado
> 
- Acessar API de IP público

```bash
curl -X GET ipinfo.io/ip                         # IP da máquina
curl -X GET ipinfo.io/000.000.00.000             # IP específico
```

