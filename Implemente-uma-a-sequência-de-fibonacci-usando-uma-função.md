Crie uma função capaz de gerar a sequência de fibonacci até n digitos.

> Código:

``` 
def Fibo(n):
    if n <= 1:
        return n
    else:
        return Fibo(n-1) + Fibo(n-2)
n = int(input('Quantos números será mostrado? '))
n1 = 0
n2 = 1
cont = 3
print(f'-> {n1}')
print(f'-> {n2}')

while cont <= n:
        n3 = n1 + n2
        print(f'-> {n3}')
        n1 = n2
        n2 = n3
        cont += 1
resultado = Fibo(n)
print(resultado)
print('-> FIM')

```