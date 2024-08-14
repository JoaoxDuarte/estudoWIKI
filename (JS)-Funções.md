**TEORIA**

_Descrever sobre funções em JavaScript:_

A função consiste em uma instrução indicada para retornar um argumento. Ou seja, por meio da função realiza-se um conjunto de instruções que executa uma tarefa ou calcula-se um valor. É como um bloco de código reutilizável, a fim de evitar a repetição da lógica em diversos partes do projeto. Para utilizá-la basta invococá-la quando preciso for!

Para isso, antes, é necessário defini-la em algum lugar no escopo onde você quer chamá-la.

**DECLARANDO UMA FUNÇÃO**

A definição da função (também chamada de _declaração de função_) consiste no uso da palavra chave _function (en-US)_, seguida por:

- `Nome da Função`;
- `Argumento` para a função (ou lista de argumentos), entre parênteses e separados por vírgulas.
- `Declarações JavaScript` que definem a função, entre chaves { }.

**_Exemplo 1:_**

```
function primeiraFuncao (){

console.log(" Olá primeira Função!");
}

```

No exemplo acima criamos a função chamada `primeiraFuncao`, ainda sem argumento e com uma declaraçao JavaScript `console.log` (que serve para imprimir uma mensagem, no caso "Olá Primeria Função!").

Agora que definimos a função, podemos invocá-la. Faremos isso executando `nome da função()`. Veja:

```
function primeiraFuncao (){

console.log(" Olá primeira Função!");
}

primeiraFuncao()
```
_Rode o código acima em um shell para visualizar o resultado!_

**ARGUMENTOS DA FUNÇÃO**

_Argumentos de uma função é o valor(ou valores) que são passados. São expreessos dentro dos parênteses, nesse caso o argumento `nome`. 
**_Exemplo 2:_**

```
function dizerNome (nome){

console.log("Meu nome é "+nome);
}

```

Agora, acima temos uma função que utiliza um argumento `(nome)`. Vamos então invocar a mesma função `dizerNome` 3 vezes, mudando apenas o parâmetro _nome_. Veja:

```
function dizerNome (nome){

console.log("Meu nome é "+nome);
}

dizerNome ("Zé Pequeno"); 
dizerNome ("Maria Chiquinha"); 
dizerNome ("Pé de pano"); 
```

**Utilizando mais de um argumento em uma função:**

Vamos criar a funçao soma 

**_Exemplo 3:_**

```
function soma(a,b){
   var soma = a + b;

return soma;
}

var somaUm = soma(2, 5);
console.log (somaUm);

var somaDois = soma(20, 20);
console.log (somaDois);

```