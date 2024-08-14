# Teoria

<span dir="">Uma classe abstrata apenas com métodos abstratos tem um comportamento quase igual ao de uma interface. A diferença é que interfaces podem ser implementadas ao invés de herdadas como classes abstratas. Isso significa que podemos implementar quantas interfaces quiser e aproveitar do polimorfismo disso.</span>

<span dir="">Já com classes abstratas só podemos herdar uma vez. Além disso, interfaces não permitem a criação de atributos. Classes abstratas permitem. Em Python, podemos criar uma classe abstrata herdando do módulo ABC.</span>

<span dir="">A maior parte das linguagens não da suporte a campos privados em interfaces por que esses campos precisam ser públicos para não ocorrer a limitação de acessos na própria classe. </span>



* <span dir="">Associação: Objeto A depende de B. São independentes entre eles, mas se relacionam em algum momento. (exemplo: Professor e aluno, são independentes, mas um professor pode ensinar a vários alunos e assim ter uma relação entre eles).</span>
* <span dir="">Composição: Objeto A consiste de B e gerencia o ciclo de vida de B. (exemplo: Um prédio de apartamentos consiste de apartamentos, se o prédio deixar de existir, os apartamentos também deixarão).</span>

## Prática

Declare uma interface que simboliza uma forma geométrica. Essa interface deve ter um método para calcular a área da forma.

```
from abc import ABC, abstractmethod


#ABSTRACT BASE CLASS
class IFormaGeometrica(ABC):

    @abstractmethod
    def calculoArea(self):
        pass

    @abstractmethod
    def calculoPerimetro(self):
        pass
```