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

## Xwiki
