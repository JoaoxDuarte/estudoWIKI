# Estruturas de controle de fluxo

<span dir="">Uma Estrutura de Controle é um bloco de programação que analisa variáveis e escolhe uma direção para seguir</span>, e junto dela, vem o termo Controle de Fluxo, sendo nada mais nada menos que o processo básico de tomada de decisão das máquinas, onde o controle de fluxo determina como um software ou uma aplicação responderá diante de certas condições e parâmetros. <span dir="">Existem dois tipos de estruturas de controles: Estruturas de controle Condicionais e Estruturas de repetição. Abordarei como principal as condicionais nessa teoria.</span>

## Estrutura de controle condicionais

<span dir="">Em Python, nas estruturas condicionais, é usado if, elif (else if), else. As condicionais nos permitem selecionar certos blocos de código que serão ou não executados dependendo de certas condições, pela forma:</span>

1. <span dir=""> A condição é verdadeira?</span>
2. <span dir=""> Se sim, execute um trecho de código.</span>
3. <span dir="">Senão, execute outro trecho de código.</span>

<span dir="">Exemplos:</span>

```
condicao_1 = False 
condicao_2 = False 
if condicao_1:      # é a mesma coisa de if condicao_1 == True:
   print("A condicao_1 é verdadeira.")
elif condicao_2:    # if condicao_2 == True:
   print("A condicao_2 é verdadeira.") 
else: 
   print("As condições condicao_1 e condicao_2 são falsas.")

"As condições condicao_1 e condicao_2 são falsas."
```

<span dir="">Os blocos de código em Python são delimitados por sua indentação (delimitação dos blocos de códigos), como podemos ver pelos comandos </span>`print`<span dir=""> , que estão alinhados mais à direita do bloco.</span>

## Branching (Ramificação)

<span dir="">Em Python, Branching ou Ramificação, é usado para alterar o fluxo normal da execução de um código, com base em alguma condição, onde um programa decide se deve fazer algo ou não.</span>

## <span dir="">U</span>nreachable Code (Código Inacessível)

<span dir="">É um código ou uma sequência de códigos que não pode ser executado, por não ter jeito do controle de fluxo alcançar esse código ou sequência. Alguns motivos para isso acontecer seria erros de programação ao desenvolver branches condicionais complexas, testes de unidades incompleto devido ao qual o código inacessível não foi detectado, códigos desnecessários que o desenvolvedor esqueceu de excluir, etc.</span>

## Prática

```
print("Em Python, blocos de código são delimitados por sua indentação.")  
usuario = int(input("Digite 1 para verdadeiro e 2 para falso: "))  

if usuario == False:  # Condição A False
  print("É verdadeiro!!!")
else:                 # Condição B True
  print("É falso!!!!")

# Vai retornar sempre "É falso!!!!" pela regra determinada: será executado a condição que for True
```