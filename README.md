# ProjetoWikis

Projeto de avaliação de Wikis

## BookStack

Para criar os containers com o docker-compose e acessar a aplicação:

1. cd ProjetoWikis/bookstack
2. Criar volume de configurações do Bookstack: `docker volume create bookstack_config`
3. Criar volume de dados para o MariaDB: `docker volume create bookstackdb_data`
4. Criar a rede utilizada: `docker network create network-bookstack`
5. Criar os container em background: `docker-compose up -d`
6. Ver os logs: `docker-compose logs`
7. Acesso: `http://IP:porta` (Usuario: admin@admin.com / Senha: password)

## Wiki.js

Para criar os containers com o docker-compose e acessar a aplicação:

1. cd ProjetoWikis/wikijs
2. Criar volume de configurações do Wikijs: `docker volume create wikijs_config`
3. Criar volume de dados para o PostgreSQL: `docker volume create wikijsdb_data`
4. Criar a rede utilizada:  `docker network create network-wikijs`
5. Criar os container em background: `docker-compose up -d`
6. Ver os logs: `docker-compose logs`
7. Acesso: `http://IP:porta` (Usuario e senha criados no primeiro acesso)


## Xwiki

Para criar os containers com o docker-compose e acessar a aplicação:

1. cd ProjetoWikis/wikijs
2. Criar volume de configurações do Bookstack: `docker volume create xwiki_config`
3. Criar volume de dados para o MariaDB: `docker volume create xwikidb_data`
4. Criar a rede utilizada: `docker network create network-xwiki`
5. Na pasta do docker-compose.yml baixar: `wget https://raw.githubusercontent.com/xwiki-contrib/docker-xwiki/master/12/mysql-tomcat/mysql/xwiki.cnf`
6. Na pasta do docker-compose.yml baixar: `wget https://raw.githubusercontent.com/xwiki-contrib/docker-xwiki/master/12/mysql-tomcat/mysql/init.sql`
7. Criar os containers em background: `docker-compose up -d`
8. Ver os logs: `docker-compose logs`
9. Acesso: `http://IP:porta` (Usuario e senha criados durante a configuração)
