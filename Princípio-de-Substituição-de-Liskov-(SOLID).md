# Princípio de Substituição de Liskov
## Teoria
### Introdução
Na programação orientada a objeto, o princípio de substituição de Liskov diz que objetos devem ser substituídos por seus subtipos sem que isso afete a execução correta do programa.
"Sempre que uma classe cliente esperar uma instância de uma classe base X, uma instância de uma subclasse Y de X deve ser usada no seu lugar"
É formalmente definido como: "Se q(x) é uma propriedade demonstrável dos objetos x de tipo T; Então q(y) deve ser verdadeiro para objetos y de tipo S onde S é um subtipo de T.
Sem esse princípio, a hierarquia das classes seria uma bagunça.
A classe Quadrado é um retângulo que tem uma característica especial: a largura e a altura são iguais. Será que na orientação a objetos essa é uma boa abstração? Vamos ver!

é importante ressaltar, ao fazer um sistema de orientação a objetos, deve atribuir a cada tipo (Classe, estrutura, Interface) as responsabilidades adequadas. Uma interface é útil porquê ela estabelece contratos, onde você tem certeza do comportamento que uma classe terá.

Na prática, esse princípio serve para saber quando uma classe pode ou não ser classe derivada de outra classe. Muito útil para perceber quando você esta "forçando a barra" nas derivações, como no exemplo abaixo de quadrados e Triângulos

### Injeção de dependências
Imagine que você esta fazendo um programa que envolve armazenamento e conversão de vídeos, e portanto, há  uma classe "Videos". Você planeja implementar uma funcionalidade de conversão nesses vídeos, sendo possível converter qualquer objeto da classe "Vídeo" em MP4, AVI ou MKV. Pensando nessa abstração, a classe de Vídeos é dependente das seguintes classes: "MP4, AVI e MKV". Em vez de inserirmos a variáveis destes tipos dentro da classe em si, aumentando a dependência e ferindo o princípio aberto-fechado do SOLID, podemos diminuir um pouco essa dependência, passando como argumento no construtor da classe Videos e "setando" as variáveis da classe ali usando os parâmetros passados. Assim podemos "injetar" as dependências necessárias sem interferência direta da classe de Videos. Qualquer modificação de "MP4, AVI E MKV" não irá interferir na classe "Videos", já que aqueles estão sendo passados como parâmetros. As variáveis da própria classe e dos parâmetros precisam compartilhar a mesma interface, pra ser possível "setar".
Caso o princípio de substituição de Liskov seja quebrado e ocorra a injeção de dependência, irá ocasionar vários bugs no software. Visto que a injeção de dependência é justamente substituir a classe mãe pela classe filho sem afetar a execução do programa
 

### Quadrados e Triângulos na orientação a objetos
De forma intuitiva, podemos pensar que o Retangulo é a classe base e o Quadrado a classe derivada. Esse tipo de pensamento pode levar à alguns problemas. Imagine o seguinte cenário:

Uma classe quadrado herda de uma classe retangulo. na classe retangulo há setLargura e setAltura, o que pra um quadrado não faz muito sentido já que a largura e a altura são iguais. Por isso que o Princípio de subsituição de liskov fala: Uma classe filha(Quadrado) deve ser capaz de substituir uma classe base(Retângulo)


### Pratica

```python

import abc
class FormasGeometricas( abc.ABC ):
    @abc.abstractclassmethod
    def calcularArea():
        pass


    
class Quadrado(FormasGeometricas):

    def __init__(self,tamanhoLados):
        self.tamanhoLados = tamanhoLados
        
    
    def calcularArea(self):
        return self.tamanhoLados*2

class Triangulo(FormasGeometricas):

    def __init__(self,base,altura):
        self.base = base
        self.altura = altura
        
    def calcularArea(self):
        return (self.base/2) * self.altura

class Retangulo(FormasGeometricas):
    
    def __init__(self,base,altura):
        self.base = base
        self.altura = altura
    def calcularArea(self):
        return self.base * self.altura


quadradoLado = int(input("Digite o lado de um quadrado  ->"))
quadrado1=Quadrado(quadradoLado)

print("Area do quadrado informado:",quadrado1.calcularArea())


trianguloBase = int(input("Digite a base de um triangulo  ->"))
trianguloAltura = int(input("Digite a altura de um triangulo  ->"))
triangulo1 = Triangulo(trianguloBase,trianguloAltura)
print("Area do triangulo informado:",triangulo1.calcularArea())


retanguloBase = int(input("Digite a base de um retangulo  ->"))
retanguloAltura = int(input("Digite a altura de um retangulo  ->"))
retangulo1 = Retangulo(retanguloBase,retanguloAltura)
print("Area do retangulo informado:",retangulo1.calcularArea())
```


