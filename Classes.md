# Teoria 
Classes são representações de objetos do mundo real. Cada classe possui seus atributos e seus métodos. Por isso o nome de Programação Orientada a Objetos (POO). Para "usar" um método, é necessário chamá-lo.
- Atributos são características do objeto.
- Métodos é aquilo que o objeto faz, seu comportamento.

Por exemplo um carro: ele possui cor, marca, modelo e rodas. Ele é capaz de ligar, acelerar, frear e desligar.


> Modificadores de Acesso

Os Modificadores de Acesso determinam o quão visível está os métodos e atributos diante das outras classes. Há três tipos modificadores de acesso em POO. Caso não tenha um modificador explícito, denominamos de Default.
- Public: permite que qualquer classe acesse atributos e métodos da classe em questão;
- Private: limita os acessos à própria classe;
- Protected: permite o acesso de uma classe de outro pacote, no caso de uma herança.


> Campos/propriedades

Os campos armazenam um determinado valor, ou seja, são variáveis. É 
recomendado que os campos sejam privados.


As propriedade são funções membro que podem ser tratadas sintaticamente como se fossem campos, podendo ser de leitura ou escrita.

Propriedades fazem com que você oculte como as coisas funcionam na sua classe com indefinidos campos. As propriedades te permitem esconder suas variáveis (deixando as privadas) expondo métodos (get e set) que são interfaces que te permitem interagir com as variáveis. A diferença está na interação. Com variáveis, podemos alterar ou consumir o valor de uma variável diretamente acessando a própria, já com propriedades é necessário passar por validações para chegar até variável desejada


# Prática 
Declare uma classe que descreve um quadrado. Essa classe deve ter um método para calcular a área.

> Código:

``` 
class quadrado:
    def __init__(self, lado):
        self.lado = lado
        self.area = lado * lado
        self.perimetro = 4 * lado
        print('O lado é: ', self.lado)

#Métodos que usam parâmetros:         
    def calculoArea(self):
        print('A área é: ', self.area)
    def calculoPerimetro(self):
        print('O perímetro é: ', self.perimetro)       


lado = int(input('Digite o lado do quadrado (o quadrado possui lados iguais): '))
q1 = quadrado(lado)

#Chamando os métodos
q1.calculoArea()
q1.calculoPerimetro()
```