# Grafos

<span dir="">Simplificadamente, um grafo é uma coleção de vértices (V) e uma coleção de arcos (E) constituídos por pares de vértices. Em uma analogia simples, os vértices seriam como ‘locais’, com o conjunto de vértices sendo um conjunto de todos os possíveis locais. Os arcos (ou arestas) representam o caminho entre estes locais. Utilizar grafos é de grande utilidade na representação de problemas da vida real.</span> Alguns exemplos:

<span dir="">1. Mapas de rotas / redes de estrada;</span>

<span dir="">2. Diagramas de pré-requisitos;</span>

<span dir="">3. Relações de amizade no ORKUT;</span>

<span dir="">4. Goal Oriented Action Planning (GOAP);</span>

<span dir="">5. Circuitos elétricos;</span>

<span dir="">6. e milhares de outros.</span>

<span dir="">A representação gráfica é normalmente da seguinte forma:</span>

![download](uploads/4e911c4b55979fddb0faaf62da8cc463/download.png)

<span dir="">Vértices são pontos ou círculos; arcos são linhas entre eles.</span>

<span dir="">_V = {1, 2, 3, 4, 5, 6}_ e _E = {(1,3), (1,6), (2,5), (3,4), (3,6)}_.</span>

<span dir="">O grafo adapta-se as nossas necessidades, assim, existindo vários tipos diferentes deles, e junto disso, alguns termos comumente usados para descreve-los. Alguns exemplos:</span>

**<span dir="">Vértice isolado</span>**

<span dir="">Um vértice é considerado isolado se não possuir nenhuma ligação a outro vértice.</span>

**<span dir="">Laço (ou loop/self-loop)</span>**

<span dir="">Um arco é um laço se em ambas as extremidades estiver o mesmo vértice.</span>

**<span dir="">Grafo simples</span>**

<span dir="">Um grafo é simples se não contiver laços nem arcos repetidos em _E_.</span>

**<span dir="">Vértices adjacentes</span>**

<span dir="">Dois vértices (_u_ e _v_) são adjacentes se existir um arco que possui uma extremidade em _u_ e outra em _v_. Os vizinhos de um vértice são todos os vértices adjacentes a ele.</span>

**<span dir="">Grafo pesado (ou grafo de arcos pesados)</span>**

<span dir="">A cada aresta está associado um valor. Pode ser uma distância, um custo, seja o que for.</span>

**<span dir="">Grafo direcionado</span>**

<span dir="">Cada arco tem um nó de origem e um nó de chegada. O exemplo típico é o das redes de estradas, uma vez que existem estradas só com um sentido seria o caos se um GPS não soubesse distingui-las.</span>

**<span dir="">Grau de um vértice (ou valência)</span>**

<span dir="">O grau de um vértice é o número de arcos que lhe são incidentes. Um arco _(u,v)_ é incidente tanto no vértice _u_ como no vértice _v_. Pode-se distinguir grau de entrada e grau de saída em grafos direcionados.</span>

<span dir="">Existem diversas formas de representa-las e armazena-las, e duas das principais são a **Matriz de adjacência** e **Lista de adjacência**.</span>

## Métodos de pesquisas no Grafo (BFS e DFS)

**BFS** ou **<span dir="">Breadth First Search</span>** <span dir="">é uma técnica baseada para armazenar em fila os vértices visitados, assim encontrando o caminho mais curto no grafo. Um vértice é selecionado no momento em que é visitado e marcado, então seus adjacentes são visitados e armazenados na fila sequencialmente.</span>

**DFS** ou **<span dir="">Depth First Search</span>** <span dir="">é uma técnica baseada para armazenar em pilha (stack) os vértices visitados, onde o vértice mais profundo do grafo é selecionado, visitado e marcado para depois visitar seus adjacentes.</span>

## Goal Oriented Action Planning (GOAP)

<span dir="">É uma arquitetura de planejamento projetada com foco no controle de comportamento de personagens autônomos em jogos</span>, ou seja, é um <span dir="">sistema de IA que dará facilmente aos seus agentes opções e ferramentas para tomar decisões inteligentes</span>. Essencialmente, esse modelo trabalha com uma abstração de grafos, sendo utilizado como um meio de construção de uma sequência de ações que satisfaz um dado objetivo através do Algoritmo **Pathfinding A\***.

![image](uploads/18cf8564423a9f5bfb76dd39fd2f7496/image.png)