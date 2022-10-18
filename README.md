# aula_mysql

CREATE TABLE produto (id_produto VARCHAR(20), nome VARCHAR(20), preco VARCHAR(20), codigo VARCHAR(20)); //Criar tabela com id_produto,nome,preco,codigo

INSERT INTO produto(id_produto) VALUES(""); //Adicionar produto

SELECT *FROM produto; //Mostrar tabela criada

UPDATE produto SET id_produto = "amora" WHERE id_produto = "limão"; //Alterar produto

DELETE FROM produto WHERE id_produto = "uva"; //Deletar um registro
