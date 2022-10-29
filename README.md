# aula_mysql

CREATE TABLE produto (id_produto VARCHAR(20), nome VARCHAR(20), preco VARCHAR(20), codigo VARCHAR(20)); //Criar tabela com id_produto,nome,preco,codigo

INSERT INTO produto(id_produto,nome,preco,codigo) VALUES("10","abacaxi","9,90","143"); //Adicionar produto

SELECT *FROM produto; //Mostrar tabela criada

UPDATE produto SET precoo = "11,00" WHERE preco = "10,00"; //Alterar produto

DELETE FROM produto WHERE id_produto = "10"; //Deletar registro

#AND
SELECT *FROM produto WHERE 
produto.id_produto= 1049 AND produto.codigo = "13881"

#OR (CASO NÃO ENCONTRAR UMA INFORMAÇÃO SERA TRAZIDA OUTRA)
SELECT *FROM produto WHERE 
produto.id_produto = 10989 OR produto.codigo= '13890200'

#IN (TRAZER INFORMAÇÃO ESPECIFICA)
SELECT *FROM produto WHERE
produto.id_produto IN (1029,5,10,7,29)

#NOT IN (INFORMAÇÃO QUE NÃO QUERO QUE SEJA TRAZIDA)
SELECT *FROM produto WHERE 
produto.id_produto NOT IN (1029,5,10,7,29)

#ORDER BY (ORGANIZAR OS RESULTADOS)
SELECT *FROM produto ORDER BY id_produto DESC 
SELECT *FROM produto ORDER BY preco ASC 
SELECT *FROM produto ORDER BY preco DESC

#LIMIT (LIMITAR INFORMAÇOES)
SELECT *FROM produto LIMIT 5;

#LIKE (PROUCURAR INFORMAÇÕES ESPECIFICAS)
SELECT *FROM produto WHERE nome LIKE '%FECHO MAGNETICO ABERT AUT BRANCO%'
SELECT *FROM produto WHERE nome LIKE '%BRANCO'#PALAVRA NO FINAL
SELECT *FROM produto WHERE nome LIKE 'FECHO%' #PALAVRA NO COMEÇO
