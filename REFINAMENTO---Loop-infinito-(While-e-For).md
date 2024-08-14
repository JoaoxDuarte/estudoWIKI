# Loop Infinito (While e For)

<span dir="">A estrutura de repetição é um recurso das linguagens de programação responsável por executar um bloco de código repetidas vezes enquanto determinada condição é atendida. No </span>**Python**<span dir="">, possuímos dois tipos de estruturas de repetição: **for** e **while**.</span>

## While

<span dir="">O comando **while** faz com que um conjunto de instruções seja executado enquanto uma condição é atendida. Quando o resultado dessa condição passa a ser falso, a execução do loop é interrompida, como mostra o exemplo a seguir:</span>

```
contador = 0
while (contador < 5):
       print(contador)
       contador   = contador + 1
```

Neste código, enquanto a variável <span dir="">contador</span>, inicializada com 0, for menor do que 5, as instruções das **linhas 3** e **4** serão executadas. Observe que na **linha 4** incrementamos o valor da variável <span dir="">contador</span>, de forma que em algum momento seu valor igualará o número 5. Quando isso for verificado na **linha 2**, o laço será interrompido. Sem esse código, a condição de parada não será atingida, gerando o que é chamado de loop infinito.

## For

<span dir="">Diferente do while, o </span>for<span dir=""> executará um determinado bloco de código por um número definido de vezes. Esta estrutura é muito útil quando já sabemos a quantidade de vezes que precisamos executar determinado bloco de código. Diferente da maioria das linguagens, para criar um intervalo de vezes que o </span>for<span dir=""> será executado, precisamos utilizar a função </span>range<span dir=""> e definir o intervalo, como podemos ver abaixo:</span>

```
for i in range(1, 10):
    print(i)
```

<span dir="">O código acima irá executar o comando </span>print<span dir=""> enquanto o intervalo entre 1 e 10 não finalizar</span>.