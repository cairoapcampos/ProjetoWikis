# ProjetoWikis

Projeto de avaliação de Wikis usando containers Docker.

## BookStack

Para criar os containers com o docker-compose e acessar a aplicação:

1. Entrar no diretório: `cd ProjetoWikis/bookstack`
2. Criar volume de configurações do Bookstack: `docker volume create bookstack_config`
3. Criar volume de dados para o MariaDB: `docker volume create bookstackdb_data`
4. Criar a rede utilizada: `docker network create network-bookstack`
5. Criar os container em background: `docker-compose up -d`
6. Ver os logs: `docker-compose logs`
7. Acesso: `http://IP:8081` (Usuario: admin@admin.com / Senha: password)

## Wiki.js

Para criar os containers com o docker-compose e acessar a aplicação:

1. Entrar no diretório: `cd ProjetoWikis/wikijs`
2. Criar volume de configurações do Wikijs: `docker volume create wikijs_config`
3. Criar volume de dados para o PostgreSQL: `docker volume create wikijsdb_data`
4. Criar a rede utilizada:  `docker network create network-wikijs`
5. Criar os container em background: `docker-compose up -d`
6. Ver os logs: `docker-compose logs`
7. Acesso: `http://IP:8082` (Usuario e senha criados no primeiro acesso)


## Xwiki

Para criar os containers com o docker-compose e acessar a aplicação:

1. Entrar no diretório: `cd ProjetoWikis/xwiki`
2. Criar volume de configurações do Bookstack: `docker volume create xwiki_config`
3. Criar volume de dados para o MariaDB: `docker volume create xwikidb_data`
4. Criar a rede utilizada: `docker network create network-xwiki`
5. Criar os containers em background: `docker-compose up -d`
6. Ver os logs: `docker-compose logs`
7. Acesso: `http://IP:8080` (Usuario e senha criados durante a configuração)
