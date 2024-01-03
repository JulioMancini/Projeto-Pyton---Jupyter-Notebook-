# Pyton-jupyter-notebook
Projeto de aprendizado Pyton do basico ao avançado (em andamento)


# LISTAS

Definição de Listas: É um objeto representado por uma sequência de outros objetos. Estes objetos são separados por vírgulas e iniciados e terminados pelos colchetes [ ]
Existem algumas formas de criação de listas e eu vou mostrar a maioria delas em alguns exemplos.

A criação de lista e bem simples, basta adicionar o nome da lista com o sinal de = e o cochete []

1. criando listas

Exemplo 1

`listaGithub =  [1,2,3,4]`

Como sabemos se isso que criamos é uma lista? Para ter certeza basta comprovar com o TYPE e o nome da lista dentro de parênteses.

![1](https://github.com/JulioMancini/Pyton---jupyter-notebook/assets/145502330/1787d4e2-421e-4c60-ab70-ccc15f1a0c22)

Exemplo 2

`listaGithub2 = list((1, 2, 3))`

Exemplo 3

`listaGithub3 = list([1, 2, 3])`

Exemplo 4 (Nesse exemplo ele transformou os caracteres em sequência)

`listaGithub4 = list("123")`

![2](https://github.com/JulioMancini/Pyton---jupyter-notebook/assets/145502330/45ed3ddd-c22b-4768-886c-be9b4acabe3d)

Exemplo 5 

`listaGithub5 = ['a', 2, 4, 'C']`

Exemplo 6

`listaGithub6 = [1, [2, 3], 'w']`

Exemplo 7

`listaGithub7 = [1, (2, 3)]`

2. Juntando listas

lista1 + lista2

Exemplo 1 

`listaGithub + listaGithub6`

![3](https://github.com/JulioMancini/Pyton---jupyter-notebook/assets/145502330/2a9eb659-d820-4ab9-be6a-a2983714d365)

podemos repetir os valores da lista

exemplo 2

`listaGithub2*3`

3. Verificar se um objeto pertence à lista

`"1"`

4. Métodos

apagando elementos da lista

exemplo ( se não adicionar nada no parêntese ele vai apagar o último elemento )

`listaGithub7.pop()`

Exemplo 2 (ponto + tab + remove)

`listaGithub.remove('1')`

Exemplo 3 (ordenado)

primeiro vamos criar uma nova lista

`lst9 = [3, 9, 1, 0, 3, 10, 4, 6]`

ordenar

`lst9.sort()`

![4](https://github.com/JulioMancini/Pyton---jupyter-notebook/assets/145502330/865e21a4-0f21-4109-afe5-5dc46cff03c1)

exemplo 4 (reverse)

`lst9.sort(reverse=True)`

# DICIONÁRIOS 

Definição de Dicionário: É um objeto que representa a coleção de um ou mais objetos. Cada objeto tem sua chave e seu valor. Assim, para acessar um valor de determinado objeto, basta chamramos sua chave. Os dicionários são iniciados e terminados por chaves { }

1. Criando dicionários

` dict1 = {'chave1': 'valor1', 
         'chave2': 'valor2'}`

`dict2 = dict(a = 1, 
             b=2, 
             c=3, 
             d= 'a')`

`dict3 = dict([('a', 1), 
              ('b', 2), 
              ('c', 3)])` 

`dict4 = {'chave1': ['valor1', 2, 3], 
         'chave2': [2, 'idade', 'nome']}`

`dict5 = {'id': [1, 2, 3], 
         'user': {'nome': ['Caio', 'Rodrigo', 'Rafael'], 
                  'idade': [29, 30, 29]}}`

`dict6 = dict(zip(['chave1', 'chave2', 'chave3'], 
                 ['valor1', 'valor2', 'valor3']))`

`dict7 = {'nomes': ('Caio', 'Rafael'), 
         'idade': (29, 30)}` 

2. Acessando valores do dicionário

![1](https://github.com/JulioMancini/Projeto-Pyton---Jupyter-Notebook-/assets/145502330/c2e4b24f-edcf-4d74-840c-f9fb805753ca)

Neste caso, como eu faço para acessar o valor da chave1? Então, eu só chamar o nome do dicionário e abrir colchetes, no caso digo o nome da nossa chave.

`dict1['chave1']`

Outros exemplos 

`dict1.get('chave2')`

`dict1.get(list(dict1)[1])`

`for chave in dict1.keys():
    print(chave, dict1[chave])`

`for chave, valor in dict1.items():
    print(chave, valor)`

3. Juntando dicionários

`dict1.update(dict2)`

![2](https://github.com/JulioMancini/Projeto-Pyton---Jupyter-Notebook-/assets/145502330/c1b4aa4e-a474-4e65-bd57-b1fc27613550)

Posso adicionar uma nova chave no dict1

`dict1["NOVA CHAVE"] = 1000`

![1](https://github.com/JulioMancini/Projeto-Pyton---Jupyter-Notebook-/assets/145502330/094928ec-7fa7-45f4-8f85-16c753470a9d)

# DATAFRAMES  - CRIANDO

Diferentemente das listas e dicionários, o Dataframe precisa que a gente importe uma biblioteca. Essa biblioteca e o Pandas, ela e muito utilizada para manipulação de dados, criação de tabelas, leitura de CSV, transformação de dados e carregamento, etc. Ou seja, Pandas é uma forte ferramenta de análise e manipulação de dados.
O pandas está simplesmente embutido dentro da linguagem Pyton. A gente consegue criar sem precisar dar nenhum importe.

1. Importando o Pandas

`import pandas as pd` (as pd é um apelido para chamar o pandas)

2. Criando DataFrames (pandas.tab)

exemplo 1
`df1 = pd.DataFrame()`

![2](https://github.com/JulioMancini/Projeto-Pyton---Jupyter-Notebook-/assets/145502330/801e65be-1308-44b6-b1a7-0e1555178b6b)

exemplo 2

`dict1 = {'identificacao': [1, 2, 3, 4, 5], 
         'nome': ['Caio', 'Rodrigo', 'Rafael', 'Mariane', 'Nathane']}`
         
`df2 = pd.DataFrame(data = dict1)`

![3](https://github.com/JulioMancini/Projeto-Pyton---Jupyter-Notebook-/assets/145502330/6c9f2136-9dbe-42d5-a56d-ffdfe16e7fe7)

exemplo 3 (mudando o índice)

`df3 = pd.DataFrame(data = dict1, index = [29, 1, 0, 2222, 88])`

![4](https://github.com/JulioMancini/Projeto-Pyton---Jupyter-Notebook-/assets/145502330/1fa4f6e2-fdbc-4d53-a829-57019b8bc93b)

exemplo 4 (com series)

`serie1 = pd.Series([1, 2, 3])`

`serie2 = pd.Series(['a', 'b', 'c'])`

`df4 = pd.DataFrame({'coluna1': serie1, 
                    'coluna2': serie2})`

![5](https://github.com/JulioMancini/Projeto-Pyton---Jupyter-Notebook-/assets/145502330/4d2d3ac5-c757-4cf3-ba9a-efa8489e237b)

exemplo 5 (numpy)

`import numpy as np`

`array1 = np.array([[1, 2, 3], 
                   ['São Paulo', 'Rio de Janeiro', 'Campinas'], 
                   ['SP', 'RJ', 'SP']])`

`df5 = pd.DataFrame(data = array1.transpose(), 
                   index = ['linha1', 'linha2', 'linha3'], 
                   columns = ['identificacao', 'cidade', 'estado'])`

![6](https://github.com/JulioMancini/Projeto-Pyton---Jupyter-Notebook-/assets/145502330/c1868a1d-c676-48f6-917d-f38ab504481b)
