# aula_mysql

CREATE TABLE produto (id_produto VARCHAR(20), nome VARCHAR(20), preco VARCHAR(20), codigo VARCHAR(20)); //Criar tabela com id_produto,nome,preco,codigo

INSERT INTO produto(id_produto,nome,preco,codigo) VALUES("10","abacaxi","9,90","143"); //Adicionar produto

SELECT *FROM produto; //Mostrar tabela criada

UPDATE produto SET precoo = "11,00" WHERE preco = "10,00"; //Alterar produto

DELETE FROM produto WHERE id_produto = "10"; //Deletar registro
