# jsp
Projeto de cadastro de cliente


CREATE SCHEMA `cadastro` ;
use cadastro;

CREATE TABLE cliente (
  `id` INT NOT NULL AUTO_INCREMENT,
  `nome` VARCHAR(45) NULL,
  `sobrenome` VARCHAR(45) NULL,
  `login` VARCHAR(45) NULL,
  `senha` VARCHAR(45) NULL,
  `endereco` VARCHAR(45) NULL,
  `contato` VARCHAR(45) NULL,
  PRIMARY KEY (`id`));
  
  
INSERT INTO cliente(nome,sobrenome,login,senha,endereco,contato)
VALUES ('Michel','Osandon','osandon',md5('teste'),'teste','123456');

SELECT * FROM cliente;
