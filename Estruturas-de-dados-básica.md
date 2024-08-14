# Estruturas de dados em Python

Em Python, <span dir="">podemos utilizar diversos tipos de estruturas de dados, que permitem guardar valores e manipular dados recebidos, com a possibilidade de controlar grandes coleções de dados de modo organizado. As principais estruturas de dados são as Listas, Tuplas e Dicionários</span>.

## Listas

<span dir="">É uma estrutura onde armazena qualquer tipo de dado primitivo, seja uma string, inteiro ou float em sequência, onde cada elemento possui sua posição na lista</span>.

<span dir="">Para criação de uma lista </span>é utilizado colchetes, com cada elemento sendo separados com vírgula. Exemplos:

```
nome_da_lista = []  # Criação de uma lista vazia
nome_da_lista = [1, 2, 3]  # Criação de uma lista de inteiros
nome_da_lista = [1, "Olá, mundo!", 1.1]  # Criação de uma lista com vários tipos diferentes
```

**<span dir="">OBS.: O primeiro elemento sempre será o índice zero.</span>**

## Tuplas

<span dir="">É uma estrutura similar a Lista, com a diferença de que na Lista, elementos inseridos podem ser alterados livremente, já nas Tuplas, elementos inseridos não podem ser alterados</span>.

<span dir="">Para criação de uma tupla </span>é utilizado parênteses, com cada elemento sendo separados com vírgula. Exemplos:

```
nome_da_tupla = (1, 2, 3)  # Tupla de inteiros
nome_da_tupla = (1, "olá", 1.5)  # Tupla heterogênea
```

## Dicionários

É uma estrutura de coleções de dados, <span dir="">armazenados de forma não ordenada. Seus elementos contém uma chave e valor, isto é, uma chave que vai servir para indexar determinado elemento no dicionário, e um valor, que pode ser de diversos tipos como listas, outros dicionários, strings, etc.</span>

<span dir="">Há dois modos para criação de um Dicionário: </span>

<span dir="">1º) Por meio de chaves ( {} ) e separando os elementos das chaves com dois pontos ( : ) e os outros elementos por vírgula ( ,</span> ). Exemplos: 

```
nome_do_dicionario = {1: "João", 2: "José"})  # {Chave: "valor", chave: "valor"}
nome_do_dicionario = {"nome": "João", "sobrenome": "Silva"})  # {"Chave": "valor", "chave": "valor"}
```

<span dir="">2º) Por meio do método dict(), com o dicionário sendo passado como parâmetro. Exemplos:</span>

```
nome_do_dicionario = dict({1: "João", 2: "José"})  # dict({Chave: "valor", chave: "valor"})
nome_do_dicionario = dict({"nome": "João", "sobrenome": "Silva"})  # dict({"Chave": "valor", "chave": "valor"})
```

## Notação BIG O

<span dir="">A notação BIG O é um método para descrever a eficiência e a complexidade de um determinado algoritmo ou compará-lo com outros pelo número de operações realizadas</span>. <span dir="">Diferentes estruturas de dados apresentam diferentes notações BIG O, ou seja, uma estrutura de dados se difere de outra tanto na eficiência, quanto na velocidade e tempo de execução dos algoritmos.</span>

## Prática

```
estagiarios = ["Victor","João","Gabriel"]  # Criação da lista de strings
print(estagiarios)  # Imprime os elementos da lista
print(estagiarios[2])  # Imprime um elemento da lista 

numeros_estagiarios = {1:'Victor',2:'João',3:'Gabriel'}  # Criação do dicionário de strings pelo 1º método
print(numeros_estagiarios)  # Imprime os elementos do dicionário

nomes = dict(numeros_estagiarios)  # Criação do dicionário de strings pelo 2º método
print(nomes) # Imprime os elementos do dicionário
```