# Pyton-jupyter-notebook
Projeto de aprendizado Pyton em andamento


# LISTAS

Definição de Listas: É um objeto representado por uma sequência de outros objetos. Estes objetos são separados por vírgulas e iniciados e terminados pelos colchetes [ ]
Existem algumas formas de criação de listas e eu vou mostrar a maioria delas em alguns exemplos.

A criação de lista e bem simples, basta adicionar o nome da lista com o sinal de = e o cochete []

1. criando listas

Exemplo 1
```bash
listaGithub =  [1,2,3,4]
```
Como sabemos se isso que criamos é uma lista? Para ter certeza basta comprovar com o TYPE e o nome da lista dentro de parênteses.

![1](https://github.com/JulioMancini/Pyton---jupyter-notebook/assets/145502330/1787d4e2-421e-4c60-ab70-ccc15f1a0c22)

Exemplo 2
```bash
listaGithub2 = list((1, 2, 3))
```
Exemplo 3
```bash
listaGithub3 = list([1, 2, 3])
```
Exemplo 4 (Nesse exemplo ele transformou os caracteres em sequência)
```bash
listaGithub4 = list("123")
```
![2](https://github.com/JulioMancini/Pyton---jupyter-notebook/assets/145502330/45ed3ddd-c22b-4768-886c-be9b4acabe3d)

Exemplo 5 
```bash
listaGithub5 = ['a', 2, 4, 'C']
```
Exemplo 6
```bash
listaGithub6 = [1, [2, 3], 'w']
```
Exemplo 7
```bash
listaGithub7 = [1, (2, 3)]
```
2. Juntando listas

lista1 + lista2

Exemplo 1 
```bash
listaGithub + listaGithub6
```
![3](https://github.com/JulioMancini/Pyton---jupyter-notebook/assets/145502330/2a9eb659-d820-4ab9-be6a-a2983714d365)

podemos repetir os valores da lista

exemplo 2
```bash
listaGithub2*3
```
3. Verificar se um objeto pertence à lista

```bash
"1"
```

4. Métodos

apagando elementos da lista

exemplo ( se não adicionar nada no parêntese ele vai apagar o último elemento )
```bash
listaGithub7.pop()
```
Exemplo 2 (ponto + tab + remove)
```bash
listaGithub.remove('1')
```
Exemplo 3 (ordenado)

primeiro vamos criar uma nova lista

```bash
lst9 = [3, 9, 1, 0, 3, 10, 4, 6]
```
ordenar
```bash
lst9.sort()
```
![4](https://github.com/JulioMancini/Pyton---jupyter-notebook/assets/145502330/865e21a4-0f21-4109-afe5-5dc46cff03c1)

exemplo 4 (reverse)
```bash
lst9.sort(reverse=True)
```
