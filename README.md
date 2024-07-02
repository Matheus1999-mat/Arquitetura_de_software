# Arquitetura_de_software

* Visão Geral

Essa aplicação em C# foi projetada para gerenciar uma livraria. Ele inclui o cadastro de usuários, bem como o registro de informações sobre os livros adquiridos por tais usuários.
O cadastro de usuários é feito com o nome e email. A busca por um usuário específico pode ser feita com o id dele.
O registro dos livros pode ser feito com o titulo, gênero, editora, preço, entrega a domicilio, telefone do cliente, e data da compra.
A busca de dados específicos sobre os livros pode ser feita com editora, titulo, genero, preço, se é entrega a domicilio e o método de pagamento.

## Instalação:

Siga estas etapas para baixar, configurar e usar a aplicação:

### Download e configuração do Mysql:

Esse projeto foi feito com o banco de dados MySQL Server. O banco de dados usado é dbAPI.
*Download:
    - Baixe o MySQL Server. Isso pode ser feito no link https://dev.mysql.com/downloads/installer/
    - Após baixar, siga as instruções de instalação.
    - Após baixar e instalar, digite e execute o seguinte código, para criar o banco de dados e a tabela a serem utilizados:
        create database dbAPI;
        use  dbAPI;
        create table User(
        id char (36), Nome varchar(50),
        Email varchar (60),
        Editora varchar (100),
        Genero varchar (50),
        Titulo varchar (100),
        EnderecoCliente varchar(100),
        TelefoneCliente varchar(20),
        PrecoLivro varchar(7),
        MetodoPagamento varchar (30),
        EntregaDomicilio varchar (10),
        DataCompra datetime, 
        createAt datetime,
        updateAt datetime);

### Download from GitHub:

* Baixe o projeto do GitHub:
    - Clique no botão verde "Code".
    - Baixe o projeto.

* Versão do .Net:
    - Certifique-se de ter o .Net 8.0 instalado no seu dispositivo.

* Descompactação:
    - Descompacte o projeto.

* Abra na IDE:
    - Abra a pasta "src" no  Visual Studio Code.

### Como usar o projeto:

* Compilar o projeto:
  - Após abrir o projeto na IDE escolhida, inicie um novo terminal. Isso pode ser feito, no Visual Studio Code, com o atalho Ctrl+Shift+'
  - Nele, navegue até a pasta src. Após isso, escreva o comando "dotnet build", sem aspas, e pressione o botão enter.

* Iniciar o projeto:
  - Após compilar o projeto , inicie o projeto. Na pasta src, escreva o comando, sem aspas, "dotnet run --project .\Api.Apllication\Application.csproj"
  - Uma outra maneira é, na pasta src, escrever, sem aspas, "cd Api.Apllication". Após isso, novamente sem aspas, escrever "dotnet run"

* Acessar o projeto:
  - No terminal do Visual Studio Code, após iniciar o projeto, http://localhost:5284 deve aparecer. No navegador, escreva http://localhost:5284/swagger 
 
* Cadastro de usuários:
  - O cadastro de usuários é feito pelo método POST.
  - A busca de usuários é feita pelo método GET. É possível buscar todos os usuários juntamente, ou apenas um usuário, por meio do id dele.
  - A atualização de usuários é feita pelo método PUT.
  - A remoção de usuários é feita pelo método DELETE. A remoção é feita considerando o id do usuário.
 
* Cadastro de livros:
  - O cadastro de dados sobre os livros adquiridos é feito pelo método POST.
  - A busca de livros é feita pelo método POST. Isso ocorre em virtude da possibilidade de buscar dados específicos, sendo possível passar um argumento.
  - A atualização de livros é feita pelo método PUT.
  - A remoção de livros é feita pelo método DELETE. A remoção é feita considerando o título do livro.
