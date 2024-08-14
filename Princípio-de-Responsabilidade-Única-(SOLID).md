# Teoria 
O Princípio de Responsabilidade Única, em inglês: Single Responsibility Principle (SRP), é o primeiro princípio dos 5 princípios/normas/regras da programação orientada a objetos — conhecida como S.O.L.I.D e, diz que uma classe deve possuir somente uma responsabilidade ("A class should have one, and only one, reason to change"), ou seja, uma classe deve ter apenas um motivo para mudar, pois quanto maior for o n° de responsabilidades, possivelmente maiores serão as modificações ulteriormente, aumentando assim,  os bugs e erros na classe.

# O Que É S.O.L.I.D?
A S.O.L.I.D é um conjunto de boas práticas que ajudam em facilitar a manutenção e organizar o código.

# Regras de Negócio e Responsabilidade Única (SOLID)
Regras de Negócio são diferentes de Requisitos de Software, requisitos esses, onde as boas práticas SOLID encaixam-se. Regras de negócio dizem como o sistema deverá fazer algo, não exige a existência de um sistema/software, possui condições e critérios, já requisitos aludem o que o sistema/software deverá fazer, não possuem condições, nem critérios e, precisam da existência de um sistema/software. E há casos que as próprias regras SOLID irão se contradizer, dependendo da equipe para escolher a melhor forma de implementar os requisitos, diante das regras de negócio. Diante do supracitado: "uma classe deve ter apenas um motivo para mudar" — sendo a regra de negócio, um desses motivos para mudar a classe.


> Exemplo da não aplicação do Princípio de Responsabilidade Única:

``` 
class quadrado:
    def __init__(self, lado):
        self.lado = lado
        self.area = lado * lado
        self.perimetro = 4 * lado
            
    def calculoArea(self):
        print('A área é: ', self.area)
    def calculoPerimetro(self):
        print('O perímetro é: ', self.perimetro)  
    def desenhar(self):
        pass    
```

A classe acima está calculando o lado, o perímetro e também está desenhando o quadrado. Possuindo um total de 3 responsabilidades.