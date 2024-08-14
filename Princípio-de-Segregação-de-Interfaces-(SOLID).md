# Princípio de segregação de Interface - *ISP* (SOLID)


## Teoria

O princípio de segregação de interface diz que interfaces específicas são melhores que do que uma interface de propósito geral

### O que é uma interface?
    Interface é um contrato que é estabelecido com as classes que desejam 
    implementar o comportamento da interface.

O ***ISP*** é violado quando uma classe é obrigada a implementar métodos que não utiliza, é por isso que o ***ISP*** fala que as interfaces devem ser as mais específica quanto for possível, assim as classes irão fazer os contratos com as respectivas interfaces e implementar todos os métodos da interface e, por consequência, somente os métodos necessários.

### Prática

### ***Má pratica***


```python

from abc import ABC, abstractmethod

class Usuario(ABC):

    @abstractmethod
    def liberarAgenda(self):
        pass

    @abstractmethod
    def agendarPresenca(self):
        pass


class Funcionario(Usuario):

    def liberarAgenda(self):
        liberarAgenda = int(input("Digite 1 para liberar agenda e 0 para não liberar:"))
        return bool(liberarAgenda)
    
    def agendarPresenca(self):
        print("Esse metodo so sera utilizado na classe de cliente!")
    

class Cliente(Usuario):

    def liberarAgenda(self):
        print("Esse metodo só sera usado na classe de funcionario!")

    def agendarPresenca(self):
         agendarPresenca = int(input("Digite o dia do mês que deseja agendar a presença:"))
         return agendarPresenca



funcionario1 = Funcionario()
funcionario1.liberarAgenda()

cliente1 = Cliente()
cliente1.agendarPresenca()
```
Pode perceber que a interface usada não é especifica o suficiente, e tanto o
cliente como o funcionario tem métodos que são obrigados a implementar que não
irão usar


### ***Boa prática***

```python
from abc import ABC, abstractmethod

class Funcionario(ABC):

    @abstractmethod
    def marcarPresenca(self):
        pass

class Cliente(ABC):

    @abstractmethod
    def agendarPresenca(self):
        pass

class atendente(Funcionario):

    def marcarPresenca(self):
        return "Presença marcada"

    def liberarAgenda(self):
        liberarAgenda = int(input("Digite 1 para liberar agenda e 0 para não liberar:"))
        return bool(liberarAgenda)



class novoCliente(Cliente):

    def agendarPresenca(self):
         agendarPresenca = int(input("Digite o dia do mês que deseja agendar a presença:"))
         return agendarPresenca


class fielCliente(Cliente):

    def __init__(self):
        print("Aviso: Voce tem tem direito a um desconto!")

    def agendarPresenca(self):
         agendarPresenca = int(input("Digite o dia do mês que deseja agendar a presença:"))
         return agendarPresenca


atendente1 = atendente()
atendente1.liberarAgenda()

cliente1 = novoCliente()
cliente1.agendarPresenca()


cliente2 = fielCliente()
cliente2.agendarPresenca()
```
Dessa vez, a interface está ***segregada*** o suficiente, tendo métodos específicos e atendendo somente as necessidades das classes que usam a interface e nada mais.