# Estruturas de controle de fluxo

<span dir=""> Ao introduzir estruturas de controle de fluxo, nosso programa deixa de ser uma mera sequência linear de instruções ineficientes para se tornar um programa capaz de tomar decisões em função do valor das variáveis ​​com que está lidando, por isso são chamadas de "inteligentes".
O controle de fluxo determina como um software ou uma aplicação responderá diante de certas condições e parâmetros, ou seja, consiste no processo básico de tomada de decisão das máquinas.</span>




## Bloco de comandos



<span dir=""> No JavaScript, o bloco de comandos é uma estrutura para agrupar outros comandos.
O bloco de comando começa pelo abre chave { e finaliza com o fecha chave }, o ultimo elemento não necessáriamente necessita de finalizar com ponto e virgula ; mas se terminar não terá problemas, este ultimo ponto e virgula é opcional:</span>

```
{
    comando;
    comando;
    ...
    comando
}
```


## Comando If

<span dir=""> Talvez um dos comandos mais utilizados em todas as linguagens de programação, o if é um comando utilizado para tomar a decisão de executar o próximo comando baseado numa expressão lógica, se esta expressão for verdadeira o próximo comando é executado, caso contrário ele é ignorado:</span>


```

var hora = new Date().getHours();
if (hora < 12){
    alert("bom dia");
}else{
    alert("boa tarde");
}

```

## Comando While

<span dir=""> Executa bloco enquanto condição resultar em verdadeiro.</span>

```
while (condição) { bloco; }

```

<span dir="">Igual ao anterior, porém o bloco é executado pelo menos uma vez, mesmo que a condição seja falsa.</span>

```
do { bloco; } while (condição);

```


## Comando Switch


<span dir="">Se o conteúdo da variável for igual a constante1 ou constante2 será executado o comando1; se for igual a constante3 será executado o comando2; caso contrário será executado o comando3; note que o comando break força o fluxo sair fora do comando switch.</span>

```
switch(variável) {
case constante1:
case constante2:
    comando1;
    break;
case constante3:
    comando2;
    break;
default:
    comando3;
}

```


## Branching (Ramificação)

<span dir="">Branching ou Ramificação é quando o tempo de execução pode escolher se segue um caminho ou outro, é usado para alterar o fluxo normal da execução de um código, com base em alguma condição</span>

## <span dir="">U</span>nreachable Code (Código Inacessível)

<span dir=""> O aviso de JavaScript "código inacessível após a instrução de retorno" ocorre ao usar uma expressão que não pode ser executada, por não ter jeito do controle de fluxo alcançar esse código ou sequência, erros de programação, códigos desnecessários, controles de fluxo complexos, pode ocorrer, por exemplo,  ao usar uma expressão após uma instrução de retorno, ou ao usar uma instrução return sem ponto e vírgula, mas incluindo uma expressão logo após:


```
function f() {
  let x = 3;
  x += 4;
  return x;   // return sai da função imediatamente
  x -= 3;     // então esta linha nunca será executada; é inacessível
}

function g() {
  return     // isso é tratado como `return;`
    3 + 4;   // então a função retorna e essa linha nunca é alcançada,
}

```


## Prática


<span dir="">O Código abaixo em Javascript retorna  B quando a condição for A e retorna X em qualquer outro caso </span>

```

var input = 'A';
if(input == 'A'){
 console.log('B'); 
} else {
  console.log('X');
}

```