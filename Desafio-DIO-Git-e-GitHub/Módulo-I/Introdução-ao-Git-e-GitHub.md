# Introdução ao Git e GitHub :cat:

### 1 - Introdução ao Git

* Entendendo o que é o Git e sua importância
  * O Git é um software de versionamento de código, criado por Linus Torvald enquanto trabalhava no desenvolvimento do sistema operacional Linux. Foi a partir do Git que programadores do mundo inteiro contribuíram com esse processo. 
  * O GitHub, por outro lado, se apresenta como uma plataforma que guarda seus códigos em repositórios, no servidor remoto, permitindo o acesso criptografado por programadores do mundo. 
  * Benefícios do uso dessas ferramentas:
    * Controle de versão;
    * Armazenamento em nuvem;
    * Trabalho em equipe;
    * Melhora seu código;
    * Reconhecimento.



### 2 - Navegação via command line interface e instalação 

* Comandos básicos para um bom desempenho no terminal

  * Digite cmd no buscador da área de trabalho e abra o Prompt de controle.

  | Funções                 | Windows   | Linux |
  | ----------------------- | --------- | ----- |
  | Mudar de pastas         | cd        | cd    |
  | Listar pastas           | dir       | ls    |
  | Criar pastas/arquivos   | mkdir     | mkdir |
  | Deletar pastas/arquivos | del/rmdir | em-rf |
  | Limpar tela             | cla       | clear |

  

### 3 - Entendendo como o Git funciona por baixo dos panos

* Tópicos fundamentais para entender o funcionamento do Git:
  * SHA1
    * openless sha1 nome-do-arquivo > ENTER
    * A sigla SHA significa Secure Hash Algorithm (Algoritmo de Hash Seguro).
    * Conjunto de funções Hash criptográficas projetadas pela NSA (Agência de Segurança Nacional dos EUA).
    * Embaralha seu arquivo de uma forma específica. A criptação gera conjunto de caracteres identificador de 40 dígitos, combinação única. Caso haja alteração de uma vírgula no arquivo, a criptação muda. A vírgula sendo removida, a criptação volta a ser como antes. Dessa forma, é fácil acompanhar as alterações de um código.
    * Forma curta de representar o arquivo.
  * Objetos fundamentais
  * Sistema distribuído
  * Segurança



* Objetos internos do Git
  * Tipos:
    * Blobs
      * Armazena metadados do Git (tamanho do objeto etc);
      * Guarda o sha1 do arquivo;
      * Bloco básico de complemento.
    * Trees
      * Armazena/aponta para blobs com os respectivos nomes dos arquivos;
      * Sha1 da árvore.
    * Commits
      * Dá sentido à estrutura;
      * Guarda todas as informações dos objetos;
      * Condição para passar para um servidor remoto;
      * O SHA1 do commit é o hash de toda a informação;
      * Função hash -object --stdin : SHA1.



* Chave SSH e Token
  * Chave SSH
    * Conexão segura e encriptada entre duas máquinas;
    * Configura nossa máquina local como "confiável" para o GitHub;
    * São geradas 2 chaves: uma privada e uma pública (.pub). A pública deve ser logada no GitHub para que a máquina local seja reconhecida;
    * Comandos:
      * Conferir possíveis chaves existentes: **ls -al ~/ .ssh**
      * Gerar chave ed25519 : **ssh -keygen -t ed25519 -C "email"**
      * Gerar chave rsa: **ssh -keygen -t rsa -b 4096 -C "email"**



### 4 - Primeiros comandos com o Git

* Iniciando o Git e criando um commit
  * Iniciar o Git;
  * Iniciar o versionamento;
  * Criar um commit.
* Comandos no Git Bash:
  * Git init 
    * Inicia um repositório - pasta oculta (.git) gerenciamento e versionamento - mostrar: **ls -a**
  * Git Add
  * Git commit
* Criando um repositório...
  * Git init
    * Configurar: git config --global user.mail "email"
      git config --global user.name "Nome"
    * Incluir todas as alterações no commit: git add *
      git commit -m "commit inicial"



### 5 - Ciclo de vida dos arquivos no Git

* Passo a passo do ciclo de vida

  * Tracked ou untracked

    ![](C:\Users\debor\OneDrive\Imagens\ciclo de vida.png)

    * Conhecendo os conceitos:

      * Untracked (não rastreável). Estado em que se encontram arquivos recém criados. O Git ainda não reconhece esse arquivo.
      * Tracked (rastreável). Quer dizer que o arquivo passou por comandos específicos e foi reconhecido pelo Git, podendo estar nos seguintes campos:
        * Inmodified: não foi modificado desde seu reconhecimento pelo Git;
        * Modified: arquivo modificado pós reconhecimento do Git;
        * Staged: arquivo modificado ou  não, aguardando por trás das cortinas para agir. Aguardando para ser commitado!

    * Sempre que um arquivo é criado, no Git, ele fica como Untracked (não rastreável). Isso quer dizer que o Git ainda não o reconhece;

    * Com o comando Git Add, o arquivo é movido automaticamente para Staged;

    * Um arquivo já reconhecido pelo Git, quando sofre uma primeira alteração, passa de Unmodified para Modified (e fica no staged, aguardando);

    * Se um arquivo é deletado, este volta a ser Untracked;

    * Uma vez que é dado o comando para criação do Commit, o arquivo volta para Unmodified e recomeça o ciclo.

      

  * Entendo o que os repositórios significam...

    * O ambiente de desenvolvimento, compreendido como nossa área de trabalho local (em nossa máquina), é dividido entre WORKING DIRECTORY, STAGING AREA e LOCAL REPOSITORY;
    * No processo do arquivo ser criado, reconhecido e sofrer possíveis modificações, esse arquivo fica passeando entre os ambientes WORKING DIRECTORY e STAGING AREA;
    * Uma vez que o Commit é criado, o arquivo se encontra no LOCAL REPOSITORY, ainda em nossa máquina local;
    * Após isso, o passo final é colocar o nosso arquivo pro servidor, em um Remote Repository (repositório remoto), como o GitHub. 



### 6 - Trabalhando com o GitHub e criando repositório remoto

* Arquivo de codificação Commitado, é hora de criarmos um repositório remoto para desenvolvedores do mundo inteiro terem acesso a ele e contribuir para a melhoria do código!

  * Criando um novo repositório no GitHub

    * Abra o github.com no navegador e crie sua conta;

    * Entre na opção Your repositories > New;

    * Dê nome ao seu repositório, uma breve descrição, decida se seu repositório será público ou privado e se quer adicionar a capa README ou não, caso tenha feito um arquivo manual que cumpre essa função.

      OBS1: caso você queira que seu código fique disponível para outros programadores versionarem, não esqueça de marcar a opção que deixa seu repositório público!

      OBS2: É interessante que na configuração do seu Git, seu email e o seu nome sejam iguais aos dados da sua conta do GitHub para evitar possíveis problemas no reconhecimento.

    * Ao criar um novo repositório no GitHub, o programa já sugere que seu repositório está vazio. É hora de apontar o repositório para o repositório local, no Git.

