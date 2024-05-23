# Arquitetura_de_software

* Visão Geral

Essa aplicação em C# foi projetada para gerenciar o registro de livros. Ele inclui o cadastro de usuários, bem como a adição, busca, atualização e remoção de livros.
O registro dos livros pode ser feito com informações, tais como gênero, título e editora.

## Installation

Siga estas etapas para baixar e configurar a aplicação:

## Download from GitHub:

* Baixe o projeto do GitHub:
    - Clique no botão verde "Code".
    - Baixe o projeto.

* Versão do .Net:
    - Certifique-se de ter o .Net 8.0 instalado no seu dispositivo.

* Descompactação:
    - Descompacte o projeto.

* Abra na IDE:
    - Abra a pasta "src" no Visual Studio ou no Visual Studio Code.

## Como usar o projeto:

* Iniciar o projeto:
  - Após abrir o projeto na IDE escolhida, inicie o projeto. No navegador, uma interface do Swagger deve aparecer.

* Como é o projeto:
  - Nesta interface do Swagger, há os endpoints necessários para o projeto funcionar.
 
* Cadastro de usuários:
  - O cadastro de usuários é feito pelo método POST.
  - A busca de usuários é feita pelo método GET. É possível buscar todos os usuários juntamente, ou apenas um usuário, por meio do id dele.
  - A atualização de usuários é feita pelo método PUT.
  - A remoção de usuários é feita pelo método DELETE. A remoção é feita considerando o id do usuário.
 
* Cadastro de livros:
  - O cadastro de livros é feito pelo método POST.
  - A busca de livros é feita pelo método GET. É possível buscar livros por título, editora ou gênero.
  - A atualização de livros é feita pelo método PUT.
  - A remoção de livros é feita pelo método DELETE. A remoção é feita considerando o título do livro.
