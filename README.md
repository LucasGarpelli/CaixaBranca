Caixa-Branca
Descrição
Este projeto consiste em duas classes principais:

User.java: Contém métodos para estabelecer conexão com o banco de dados e verificar se um usuário existe.
Teste.java: Classe de teste para verificar o funcionamento dos métodos da classe User.
Como Executar
Passo 1: Criar o Banco de Dados
Execute os seguintes comandos SQL para configurar o banco de dados:

Criação do Banco de Dados
CREATE DATABASE teste;
    
Criação da Tabela usuarios
CREATE TABLE usuarios (
    id INT AUTO_INCREMENT PRIMARY KEY,
    login VARCHAR(50) NOT NULL,
    senha VARCHAR(50) NOT NULL,
    nome VARCHAR(100) NOT NULL
);
    
Passo 2: Inserir Dados no Banco de Dados
Adicione os seguintes dados ao banco de dados:

INSERT INTO usuarios (login, senha, nome) VALUES ('Zhefiroth', '1234', 'Matheus');
    
Passo 3: Configurar a URL de Conexão
Atualize a URL no código para apontar para o seu banco de dados:

"jdbc:mysql://127.0.0.1/Nome_do_seu_Banco_de_Dados?user=Seu_usuario_do_MYSQL&password=Sua_senha"
    
Passo 4: Baixar o Driver MySQL
Faça o download do driver JDBC MySQL no site:

https://dev.mysql.com/downloads/connector/j/
Selecione a opção Platform Independent e faça o download do arquivo Platform Independent (Architecture Independent), ZIP Archive.

Extraia o arquivo ZIP, localize o JAR mysql-connector-j-9.1.0.jar e adicione-o ao seu projeto.

Passo 5: Executar o Projeto
Após seguir os passos acima, o projeto estará funcionando corretamente.