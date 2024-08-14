# Teoria
 No python existem os seguintes tipos de dados:

- Números
- Strings
- Booleanos

> Números em Python:

O mais básico e importante. Em toda aplicação estará presente.

Inteiros:
São aqueles que não possuem parte decimal.
Exemplo: Zero (0) , números positivos (1,2,3,4,5,6,7,8,9…) e os negativos (-1, -2, -3…).

Flutuantes:
São “números quebrados”, ou seja com base decimal.
Exemplo: 0.2 / 0.5 / 21.7…

> Strings

Se trata de um conjunto de caracteres.
Muitas vezes é usada em um input.

Exemplo: 
- “PALAVRA”
- “489498”
- “A, B, C”

> Booleanos

O booleano pode receber apenas dois valores: True (VERDADEIRO) e False (FALSO).

Logo, quando uma variável é definida com TRUE seu valor será verdadeiro, quando definida como FALSE será falso.

> Casting:

Se trata da conversão do tipo de dados de um objeto no tipo de dados necessário. 


> Diferença de tamanho entre tipos:

O tipo int (números inteiros) armazena 32 bits (ou 64 bits, dependendo da arquitetura do computador ultilizado), já o tipo float (números quebrados/decimais) também armazena 32 bits (ou 64 bits, dependendo da arquitetura).

> Por que uma string não é um tipo simples?

Diferentemente dos tipos int, float e bool que são considerados tipos simples pois seus valores não formados por uma parte menor, a string é construída de pedaços menores.

# Prática
> Execução do código em Python

``` 
number=float(input("Digite um número decimal (float): ")) 
print ("Seu número em float: ",number)
number = int(number)
print ('Seu número em int agora é:', number)

```
