## Shadow Variable

<span dir="">Uma Shadow Variable é definido como quando uma variável "esconde" outra variável com o mesmo nome, ou seja, ocorre quando um programador declara novamente uma variável em um escopo menor, tendo o mesmo nome que a variável do escopo maior. Assim, quando ocorre o sombreamento de variáveis, existem _duas ou mais_ variáveis ​​com o mesmo nome, e suas definições dependem de seu escopo.</span>

## Prática

```
estagiario = ['Victor', 'João', 'Gabriel', 
	   'Marcos', 'Kauan', 'Kassio'];

def mostra_estagiarios(estagiario):

  num = 6
  print(f"O número total de estagiários são {num}!")
  def estagiarios_manha():
    num = 3
    print(f"O número de estagiários de manhã é {num}!")
  estagiarios_manha()

mostra_estagiarios(estagiario)
```