**Definição**
Estruturas de dados são modos de armazenar e organizar dados na memória de um computador para que possam ser usados com mais eficiência. Podem ser usados em vários tipos de aplicativos. Em alguns casos, são bem especializados e orientados a tarefas específicas. As estruturas de dados clássicas são:

Vetores e matrizes (Arrays);
Pilha (stack);
Fila;
Lista;
Árvore;

_Vetores (Arrays)_

É uma estrutura homogênea que mantém uma série de elementos de dados do mesmo tipo. Além de possuírem tamanho fixo, podem ter uma dimensão (vetores) ou mais de uma (matriz).
Alguns exemplos de vetor unidimensional:
``` js
const num = [1, 2, 3, 4, 5];
const blackPink = ["Jisoo", "Lisa", "Jennie", "Rosé"];
```
Um exemplo de vetor bidimensional
```js
const moreNumbers = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
];
```
_Pilha (stack)_

A pilha (stack) é uma estrutura de dados usada para colecionar elementos e permitir o acesso somente a um item da coleção armazenado - o último item que foi incluído na estrutura (item do topo). A pilha funciona com o método LIFO (Left In, First Out). O último item é o primeiro a sair da pilha.
```js
class Stack {
  constructor(maxSize) {
    // definir o número máximo de elementos da pilha caso não seja fornecido
    if (isNaN(maxSize)) return maxSize = 10;
    this.maxSize = maxSize; // iniciar um array que conterá os valores da pilha
    this.container = []; // vetor que terá os elementos da pilha
  }
}
```
_Fila_

Estrutura de dados que usa o método FIFO (First In, First Out). O primeiro item é o primeiro a sair da fila.
```js
class Queue {
  constructor(value) {
    this._size = 0;

    if (value === undefined) return this._first = null, this._last = null;
    else this.enqueue(value);
  }

  // retornar tamanho da fila
  get size() {
    return this._size;
  }

  // verificar se a fila está vazia
  get empty() {
    return this.size === 0;
  }
}
```
_Lista Encadeada_

Listas encadeadas são estruturas de dados feitas de grupos de nós que juntos representam uma sequência.
```js
class LinkedList {
  constructor(value) {
    this._head = null;
    this._size = 0;

    if (value !== undefined) {
      this.append(value);
    }
  }
}
```

_Árvore_

A árvore é uma estrutura não linear, ou seja, é uma coleção de nós conectados por arestas. Os nós de menor valor ficam do lado esquerdo e os de maior valor ficam no lado direito.
```js
// criar a árvore
class ArvoreBuscaBinaria {
  constructor(root = null) {
    this.root = null;
  }
}
```

**Notação BIG O**

A notação BIG O é um método para descrever a eficiência e a complexidade de um determinado algoritmo ou compará-lo com outros pelo número de operações realizadas. Diferentes estruturas de dados apresentam diferentes notações BIG O, ou seja, uma estrutura de dados se difere de outra tanto na eficiência, quanto na velocidade e tempo de execução dos algoritmos.
Ficou com dúvidas? Acesse a Wiki notação big o: https://gitlab.sedes.df.gov.br/igor.costa/estudo-de-python-e-logica-de-programacao/-/wikis/REFINAMENTO-BIG-O-NOTATION