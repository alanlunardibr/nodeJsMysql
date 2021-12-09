# nodeJsMysql
Projeto NodeJs com Mysql

# Iniciar Arquivo Package.json
yarn init -y

# InstalarExpress
Gerenciador de Rotas
yarn add express

# instalar nodemon em modo de desenvolvimento
yarn global add nodemon
yarn add -D nodemon
Comando para rodar nodemon "nomearquivo.js"

# Criar o Banco de Dados
create database usuarios character set utf8mb4 collate utf8mb4_unicode_ci;

# Criar Tabela do Banco
CREATE TABLE `usuarios`.`users` (
  `id` INT NOT NULL AUTO_INCREMENT,
  `name` VARCHAR(220) CHARACTER SET 'utf8mb4' COLLATE 'utf8mb4_unicode_ci' NOT NULL,
  `email` VARCHAR(220) CHARACTER SET 'utf8mb4' COLLATE 'utf8mb4_unicode_ci' NOT NULL,
  PRIMARY KEY (`id`)
  )
ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE utf8mb4_unicode_ci;

# Conectar NodeJs com Mysql usando sequelize

yarn add sequelize

# Instalar Driver do Banco de Dados

yarn add mysql2