# Estruturas de repetição 

### Teoria

- O código deve funcionar
- O texto deve explicar o que são loops infinitos
- O texto deve citar diferença entre loops e recursão
- O texto deve explicar o que é unrolling de loops
- O texto deve responder se loops causam branching ou não


### O que são Loops Infinitos ?

Loops infinitos são aqueles em que a condição é sempre verdadeira

### Qual a diferença entre loops e recursão?

A principal diferença entre recursão e loop é que recursão é um mecanismo para chamar uma função dentro da mesma função, enquanto loop é uma estrutura de controle que ajuda a executar um conjunto de instruções repetidas vezes até que a condição dada seja verdadeira.

### Oque é unrolling de loops ?

Loop unrolling é uma técnica de transformação de loop que ajuda a otimizar o tempo de execução de um programa




### Pratica
``` 
n = int(input("Digite o valor de n: "))

soma = 0
i = 1

while (i <= n):
    soma = soma + i
    i = i + 1

print ("Sum(1, {}) = {}". format(n, soma))
``` 

No caso aqui quando o usuário digitar um número armazenamos ele em uma variável e logo depois definimos duas variáveis 
soma e i definimos que vão começar o loop como 0 e 1 respectivamente 

então enquanto o i for menor ou igual ao numero que o usuário digitou a váriavel soma vai receber ela mesma + i 
e o i recebe ele mesmo + 1

e assim sucessivamente até o momento que i for maior a variável n 


