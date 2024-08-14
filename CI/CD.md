**CI/CD**

CI/CD é um termo abrangente que cobre várias fases do DevOps. CI (Integração Contínua) é a prática de integrar alterações de código em um repositório várias vezes ao dia. CD tem dois significados: a entrega contínua automatiza as integrações de código, enquanto a implementação contínua libera automaticamente as compilações finais.
 
A importância do CI/CD é importante pois é uma prática recomendada de DevOps e um estágio no ciclo de vida de DevOps em que os desenvolvedores fazem check-in de código em seu repositório de código compartilhado, geralmente várias vezes ao dia. Idealmente, sempre que isso acontece, uma ferramenta de build automatizada verifica o check-in ou a ramificação para garantir que não haja erros e que esteja pronto para entrar em produção. O principal benefício é que os problemas geralmente são detectados cedo, antes que se transformem em problemas maiores. 

> CI (Continuous Integration)
- Detecta falhas rapidamente 
- Abre portas para entregas em produção automatizadas.
- Não necessita de alguém para manualmente executar os testes, validar o código e  gerar os artefatos necessários.
- Possibilita entregas de valor mais ágeis.

> CD (Continuous Delivery)
- Capacidade de obter alterações de todos os tipo, como:
- Novos recursos
- alterações de configuração
- Correções de bugs e experimentos, em produção ou na mão dos usuários, com segurança e rapidez de maneira sustentável.


> Código Declarativo 

Código Declarativo é a abordagem em que o objetivo da programação deve ser demonstrar o resultado esperado do código. para isso, a sintaxe deve contar com lógicas imutáveis, que apresentam sempre o mesmo resultado após a execução do software. 

>exemplo de aplicação que utiliza o CI/CD

O GitHub Actions é uma aplicação para criação de fluxos de software, onde estão incluídas as etapas que compõem o CI e o CD. Essa plataforma funciona como uma espécie de executor de ações (ou actions), que é definido através de código, permitindo que o desenvolvedor execute sua aplicação a partir de gatilhos configurados por ele.