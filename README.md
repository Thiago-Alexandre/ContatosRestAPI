# ContatosRestAPI
###Trabalho realizado para a disciplina de Programação 5, do Curso de Análise e Desenvolvimento de Sistemas, do Instituto Federal Catarinense- IFC.

Projeto de desenvolvimento de uma API Rest utilizando as seguintes tecnologias:

* linguagem Java;
* persistência de dados com JPA (Hibernate);
* banco de dados MariaDB;
* servidor Glassfish;
* para os testes foi utilizado o Postman.

A API tem como objetivo realizar um CRUD de Contatos através de Rest. Ela apresenta os Endpoint para listar todos os contatos, para pesquisar um contato específico, adicionar um novo contato, alterar um contato e excluir um contato. A exclusão pode ser realizada passando o id do contato como parâmetro ou passando o contato como Json.

Obs: A configuração do JPA foi definida para não modificar o banco de dados, sendo este definido e o JPA apenas realizando a persistência. O banco de dados apresenta o seguinte modelo:

```
CREATE DATABASE contatos CHARSET latin1 COLLATE latin1_general_cs;
USE contatos;

CREATE TABLE contato (
	id INTEGER PRIMARY KEY AUTO_INCREMENT,
	nome VARCHAR(50) NOT NULL,
	email VARCHAR(30) NOT NULL,
	fone VARCHAR(15contatos) NOT NULL
);
```
