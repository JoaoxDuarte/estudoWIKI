# Teoria
Há sete tipos de dados em ECMAScript (JavaScript):

- Boolean: Boolean representa uma entidade lógica e pode ter dois valores: verdadeiro(true) ou falso(false).

- null: O tipo Null tem exatamente um valor: null(nulo). Variável nula (deve ser escrito em minúsculo)

- undefined: Variável indefinida. Uma variável que não foi atribuída a um valor específico, assume o valor undefined(indefinido).

- Number: Variável numérica. Pode ser inteira ou de ponto flutuante. 

- String: Textos, pode ser declarada com aspas ou apóstrofos. O tipo String em JavaScript é usado para representar dados textuais. Isto é um conjunto de "elementos" de valores de 16-bits unsigned integer. Cada elemento na string ocupa uma posição na string. O primeiro elemento está no índice 0, o próximo no índice 1, e assim por diante. O comprimento de uma string é o número de elementos nela.

- Symbol: Usados internamente como chaves de propriedades de objetos. Não se pode fazer operações com o tipo Symbol. 

E um  tipo não primitivo:

- Object: Objetos são estruturas de dados usadas para criar o equivalente em outras linguagens a listas, arrays, dicionários, arrays associativos, dentre outros. Um objeto é um valor na memória que pode ser possivelmente referenciado por um identifier.


> Dados Primitivos: valores tratados diretamente pelo JavaScript, essas variáveis guardam valores. Exemplo: números. Não primitivos: a aplicação guarda o endereço em memória e não o valor em si.


JavaScript é uma linguagem de tipagem dinâmica. Isso significa que você não necessita declarar o tipo de uma variável antes de sua atribuição. O tipo será automaticamente determinado quando o programa for processado. Isso também significa que você pode reatribuir uma mesma variável com um tipo diferente:

_**Exemplo :**_

```
  var foo = 42;    // foo é um Number agora

  foo = "bar"; // foo é um String agora

  foo = true;  // foo é um Boolean agora

```




> Casting 

Significa converter um tipo de dados para outro tipo de dados, ou seja, a conversão de um tipo de dados string para booleano ou a conversão de um tipo de dados inteiro para tipo de dados string, por exemplo.





> Diferença entre os tipos

Tipo Number: Inteiros (armazena 32 bits, ou 64 bits, dependendo da arquitetura do computador) e Pontos Flutuantes (armazena 32 bits, ou 64 bits, dependendo da arquitetura do computador).


Booleano: Um tipo booleano geralmente segue a menor alocação da memória pelo processador que é em byte. Então, os valores lógicos irão alocar-se na memória como sendo 1 byte (1 byte = 8 bits), para representar um booleano é preciso 2 bits.



> Por que uma string não é um tipo simples?


O tipo string não é um tipo por valor propriamente dito. Ele é um ponteiro para a sequência de caracteres, por isso ele é um tipo por referência, construídos de pedaços menores.


# Prática

> Execução do código em JavaScript - Convertendo um float em inteiro




``` 

 x = 11.6;

console.log(parseInt(x)); //Converte um valor float  x em um inteiro usando a função parseInt

``` 


