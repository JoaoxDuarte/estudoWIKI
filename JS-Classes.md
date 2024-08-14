**Conceito Geral**

Classes são simplificações da linguagem para as heranças baseadas nos protótipos. Classes em JavaScript provêm uma maneira mais simples e clara de criar objetos e lidar com herança.

Para declarar uma classe precisamos utilizar a palavra chave `class` seguida do método `constructor`

**Definição**

As classes são, de fato, "funções especiais", a sintaxe de uma classe possui dois componentes: "class expressions" e "class declarations".

Class expression é uma das formas de definir uma classe no ECMAScript 2015. class expressions podem ser nomeadas ou não nomeadas. Se nomeada, o nome da classe é local para apenas o corpo da classe.

Class declaration cria uma classe com dado nome usando herança do protótipo base. 

**Métodos**

O método constructor é um tipo especial de método para criar e iniciar um objeto criado pela classe. Só pode existir um método especial com o nome "constructor" dentro da classe.

A palavra-chave static define um método estático de uma classe. Métodos estáticos são chamados sem a instanciação da sua classe e não podem ser chamados quando a classe é instanciada. Métodos estáticos são geralmente usados para criar funções de utilidades por uma aplicação.

**Modificadores de Acesso**

Os Modificadores de Acesso determinam o quão visível está os métodos e atributos diante das outras classes.
Existem três tipos de modificadores, são eles:

* Public: permite que qualquer classe acesse atributos e métodos da classe em questão;
* Private: limita os acessos à própria classe;
* Protected: permite o acesso de uma classe de outro pacote, no caso de uma herança.

**Campos/Propriedades**

Campos é o que guarda um estado do objeto. É uma das formas de se criar um atributo. É uma variável. É uma porção de dados de um todo (um registro de um objeto). É um mecanismo concreto e existente nas implementações das linguagens e outras ferramentas.

Propriedades é uma característica em específico que um objeto terá, mas não se define bem como esta característica será disponível no objeto.


**Prática**

```
class quadrado {
  constructor(altura){
    this.altura = altura;
  }
  get area() {
    return this.altura * this.altura
  }
}

const q = new quadrado(10);

console.log(q.area)
```








