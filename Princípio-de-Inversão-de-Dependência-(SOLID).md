# Teoria
Este é o quinto e último princípio da S.O.L.I.D e, diz que módulos de alto nível não devem depender de módulos de baixo nível; ambos devem depender de abstrações ("High level modules should not depend on low level modules; both should depend on abstractions”) tal qual abstrações não devem depender de detalhes. Detalhes devem depender de abstrações (“Abstractions should not depend on details. Details should depend upon abstractions”). Isso significa que um módulo não deve depender de detalhes de implementação de outro módulo diretamente, havendo a necessidade de uma abstração (interface) entre as duas, reduzindo assim, a dependência de um módulo de alto nível no módulo de baixo nível.

- Módulo/classe de alto nível: é qualquer módulo que depende de outros módulos e que execute uma tarefa com uma ferramenta.
> Exemplo: uma consulta em um BD.

- Módulo/classe de baixo nível: ajuda os módulos de alto nível a executar uma tarefa. Ele é a ferramenta para executar a tarefa.
> Exemplo: utilizaria o resultado e faria alguma operação sobre ela.

- Abstração: interface que conecta as/os duas/dois Classes/Módulos.

# RESUMINDO:

Este princípio diz que um módulo (ou uma classe) não deve ser misturado com a ferramenta que ele usa para executar uma ação. Em vez disso, ele deve ser usado em conjunto com interface que permitirá que a ferramenta se conecte ao módulo. E não menos importante, tanto o módulo quanto a interface não devem saber como a ferramenta funciona. No entanto, a ferramenta precisa atender a “especificação” da interface.