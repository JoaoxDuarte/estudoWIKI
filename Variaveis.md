# Variaveis
## Teoria
As variáveis são como containers que servem para armazenar dados na memória, temporários(variaveis) ou permanentes(constantes) no contexto de um programa.
### Declaração
O programador realiza a declaração de variavel, ou seja, ele da um nome fácil a um container de espaço na memória que irá armazenar um determinado valor. Afinal, é muito mais fácil se referir a esse espaço na memoria como 'usuarioLogin' do que algo como '0x20859532c70'.
### Atribução
A atribuição de variável é a definição ou re-definição do valor que a variável declarada ocupa.

```python
variavelN = 10 #Declaração de variavel
```

### Tipagem
Python é uma linguagem que é dinamicamente tipadas, isso é, o proprío interpretador infere os tipos de dados que uma varíavel recebe, não há a necessidade de especificar o tipo de variável.

Python é uma linguagem de tipagem forte, ou seja, ele não faz coerções automáticas entre tipos não compatíveis

## Shadow Variables

Uma Shadow Variable ocorre quando um programador declara novamente uma váriavel em um escopo menor, tendo o mesmo nome que a variável do escopo maior, isso causa confusão, sendo a causa de vários bugs e problemas no desenvolvimento de um software


## Prática
```python
print("Digite uma variavel qualquer")
variavelUsuario = input() #Pega a variavel do usuario
print(variavelUsuario.upper()) #Imprime a variavel em caixa alta
```

