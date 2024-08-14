## Prática

```
class Grafo:
  def __init__(self, vertices):
    self.vertices = vertices
    self.grafo = [[] for i in range(self.vertices)]  # criação da quantidade linhas/

  def adiciona_aresta(self, u, v):
    # Grafo direcionado, se for não direcionado self.grafo[v-1].append(u)
    self.grafo[u-1].append(v) # u-1 por que no python uma lista sempre começa pelo 0

  def mostra_lista(self):
    for i in range(self.vertices):
      print(f"{i+1}:", end='  ')
      for j in self.grafo[i]:
        print(f"{j} ->", end='  ')
      print("")

v = int(input("Digite a quantidade de vértices: "))

g = Grafo(v)

a = int(input("Digite a quantidade de arestas: "))
for i in range(a):
  
  u = int(input("De qual vértice parte esta aresta: "))
  v = int(input("Para qual vértice chega esta aresta: "))
  
  g.adiciona_aresta(u, v)
 
g.mostra_lista()
```