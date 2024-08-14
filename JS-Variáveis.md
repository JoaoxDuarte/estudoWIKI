**Conceito geral**

Variável é o nome utilizado para definir um ou mais valores que são manipulados pelos programas durante a sua operação. O nome “variável” é utilizado por ser um tipo de conteúdo que pode apresentar diferentes valores enquanto o sistema está em execução.

**Variáveis em JavaScript**

Você usa variáveis como nomes simbólicos para os valores em sua aplicação. O nome das variáveis, chamados de identificadores, obedecem determinadas regras.  
Um identificador JavaScript deve começar com uma letra, underline (_), ou cifrão ($); os caracteres subsequentes podem também ser números (0-9). Devido JavaScript ser case-sensitive, letras incluem caracteres de "A" a "Z" (maiúsculos) e caracteres de "a" a "z" (minúsculos).  
Você pode usar a ISO 8859-1 ou caracteres Unicode tal como os identificadores å e ü. Você pode também usar as sequências de escape Unicode como caracteres e identificadores.  
Alguns exemplos de nomes legais são Numeros_visitas, temp99, e _nome.  
**Declarações**

Existem três tipos de declarações em JavaScript.  
*Var:* Declara uma variável, opcionalmente, inicializando-a com um valor.  
*Let:* Declara uma variável local de escopo do bloco, opcionalmente, inicializando-a com um valor.  
*Const:* Declara uma constante de escopo de bloco, apenas de leitura.

**Declarando variáveis**

Você pode declarar uma variável de três formas:  
Com a palavra chave var (a utilização da palavra VAR é opcional). Por exemplo, var x = 42. Esta sintaxe pode ser usada para declarar tanto variáveis locais como variáveis globais.

```
var x = 42
```

Por simples adição de valor. Por exemplo, x = 42. Isso declara uma variável global. Essa declaração gera um aviso de advertência no JavaScript. Você não deve usar essa variante.  
Com a palavra chave let. Por exemplo, let y = 13. Essa sintaxe pode ser usada para declarar uma variável local de escopo de bloco. Em tópicos seguintes falaremos mais sobre o escopo de bloco.

```
let y = 13
```

**Classificando variáveis**

Uma variável declarada usando a declaração `var` ou `let` sem especificar o valor inicial tem o valor `undefined`.  
Uma tentativa de acessar uma variável não declarada resultará no lançamento de uma exceção `ReferenceError`.  
Você pode usar `undefined` para determinar se uma variável tem um valor. No código a seguir, não é atribuído um valor de entrada na variável e a declaração `if` será avaliada como verdadeira (`true`).  
O valor `undefined` se comporta como falso (`false`), quando usado em um contexto booleano.
Quando você avalia uma variável nula, o valor nulo se comporta como 0 em contextos numéricos e como falso em contextos booleanos.  
*Constante*  
Você pode criar uma constante apenas de leitura por meio da palavra-chave `const`. A sintaxe de um identificador de uma constante é semelhante ao identificador de uma variável: deve começar com uma letra, sublinhado ou cifrão e pode conter caractere alfabético, numérico ou sublinhado.

`const PI = 3.14;`

*Variáveis globais*   
São propriedades do *objeto global*. Em páginas web o objeto global é a `window`, assim você pode configurar e acessar variáveis globais utilizando a sintaxe `window.variavel.`
Consequentemente, você pode acessar variáveis globais declaradas em uma janela ou frame ou frame de outra janela. Por exemplo, se uma variável chamada phoneNumber é declarada em um documento, você pode consultar esta variável de um frame como `parent.phoneNumber`.

**Escopo de variável**

Quando você declara uma variável fora de qualquer função, ela é chamada de variável *global*, porque está disponível para qualquer outro código no documento atual. Quando você declara uma variável dentro de uma função, é chamada de variável *local*, pois ela está disponível somente dentro dessa função.

JavaScript antes do ECMAScript 6 não possuía escopo de declaração de bloco (Uma declaração em bloco é utilizada para agrupar declarações. O bloco é delimitado por um par de chaves); pelo contrário, uma variável declarada dentro de um bloco de uma *função* é uma variável local (ou contexto *global*) do bloco que está inserido a função. Por exemplo o código a seguir exibirá 5, porque o escopo de `x` está na função (ou contexto global) no qual `x` é declarado, não o bloco, que neste caso é a declaração `if`.

**Shadow Variable**

Uma Shadow Variable é definido como quando uma variável "esconde" outra variável com o mesmo nome, ou seja, ocorre quando um programador declara novamente uma variável em um escopo menor, tendo o mesmo nome que a variável do escopo maior. Assim, quando ocorre o sombreamento de variáveis, existem *duas ou mais* variáveis ​​com o mesmo nome, e suas definições dependem de seu escopo.