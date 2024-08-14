

# Sejam bem-vindos ao controle de versão, galera: 

> O que é controle de versão: 

O controle de versão é uma forma de rastrear e gerenciar as alterações em um código de software. 

Exemplificando de forma objetiva o controle de versão para o mundo do Git:

Sempre que alguém fizer uma alteração no Git isso será registrado, assim será possível analisar o código posteriormente. 

> Diferença entre Git e GitLab/GitHub:

- Git: É um sistema de controle de versão em código aberto. É por esse sistema que será encontrado o histórico de alterações. 

- Já o GitLab/GitHub são plataformas de hospedagem. 

Os dois são similares, porém o GitLab permite que os desenvolvedores armazenem o código em seu próprio servidor, enquanto o GitHub trabalha em servidores de terceiros. 

# Prática: 

> Tutorial de como clonar esse projeto: 

Fala, galera!

1. Você precisará de um programa chamado **GITBASH** em sua máquina.

2. Chave pública: 
Você deverá saber se possui uma chave pública. 
Para isso use esse comando: 

```cat ~/.ssh/id_rsa.pub```

Se você não possuir a chave utilize esse outro comando:

```ssh-keygen```

3. Dê o comando Public Key ``cat ~/.ssh/id_rsa.pub`` e copie o conteúdo. 

4. Acesse o site do GitLab aqui da sedes ``https://gitlab.sedes.df.gov.br/``

5. Clique sobre o seu avatar e clique em "edit profile" e posteriormente em SSH KEYS, ou então cole o seguinte link abaixo em seu navegador:
``https://gitlab.sedes.df.gov.br/-/profile/keys``

6. Lembra do conteúdo da sua public key que você adquiriu com o comando cat ~/.ssh/id_rsa.pub. 
Cole este conteúdo da sua chave pública no campo KEY.

7. Clique no botão ADD KEY. PRONTO! A sua chave SSH está adicionada. 

Agora faça o seguinte: 

-  Clique em "Menu" 
-  Selecione "Projects"
-  Clique sobre o projeto desejado (Estudo de python e logica de programação). 
-  Depois disso clique no botão "Clone". 
-  Clique no botão clone para copiar a URL.
-  Copie esse conteúdo. 

Vá agora para o terminal do GITBASH e faça o seguinte: 

execute o seguinte comando ``git clone`` + A URL que você copiou no GITLAB. 

Dessa forma: 

``git clone git@gitlab.sedes.df.gov.br:igor.costa/estudo-de-python-e-logica-de-programacao.git``

DÊ ENTER e espere! 

Feito isso você terá o projeto clonado no seu computador! 

 Será gerado uma pasta com o nome do projeto "automacao-de-insercao-no-siads". 
E dentro um arquivo REDME.MD

# Configurar a chave SSH no Gitlab: 


- Abra o GITBASH e execute esse comando: 

``cd .ssh/``

- Pressione ENTER e digite posteriormente: 

``ls``

- Pressione ENTER e então execute o comando: 

``code config``

- Você então será direcionado ao Visual Studio: 

Jogue essas linhas de código para executar a configuração:

``Host gitlab.sedes.df.gov.br
    HostName gitlab.sedes.df.gov.br
    Port 2222``
