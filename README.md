# ProjetoWikis

Projeto de avaliação de Wikis

## BookStack

Para criar os containers com o docker-compose e acessar a aplicação:

1. Criar volume de configurações do Bookstack: `docker volume create bookstack_config`
2. Criar volume de dados para o MariaDB: `docker volume create bookstackdb_data`
3. Criar a rede utilizada: `docker network create network-bookstack`
4. Criar os container em background: `docker-compose up -d`
5. Ver os logs: `docker-compose logs`
6. Acesso: `http://IP:porta` (Usuario: admin@admin.com / Senha: password)

## Wiki.js

Para criar os containers com o docker-compose e acessar a aplicação:

1. Criar volume de configurações do Wikijs: `docker volume create wikijs_config`
2. Criar volume de dados para o PostgreSQL: `docker volume create wikijsdb_data`
3. Criar a rede utilizada:  `docker network create network-wikijs`
4. Criar os container em background: `docker-compose up -d`
5. Ver os logs: `docker-compose logs`
6. Acesso: `http://IP:porta` (Usuario e senha criados no primeiro acesso)


## Xwiki

Para criar os containers com o docker-compose e acessar a aplicação:

1. Criar volume de configurações do Bookstack: `docker volume create xwiki_config`
2. Criar volume de dados para o MariaDB: `docker volume create xwikidb_data`
3. Criar a rede utilizada: `docker network create network-xwiki`
4. Na pasta do docker-compose.yml baixar: `wget https://raw.githubusercontent.com/xwiki-contrib/docker-xwiki/master/12/mysql-tomcat/mysql/xwiki.cnf`
5. Na pasta do docker-compose.yml baixar: `wget https://raw.githubusercontent.com/xwiki-contrib/docker-xwiki/master/12/mysql-tomcat/mysql/init.sql`
6. Criar os containers em background: `docker-compose up -d`
7. Ver os logs: `docker-compose logs`
8. Acesso: `http://IP:porta` (Usuario e senha criados durante a configuração)
