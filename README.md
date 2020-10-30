# TCC-Projeto-EAD_backend
Trabalho de conclusão do curso sistemas de informação

## Preparando ambiente para executar projeto
### Requirements
- Node.js
- Yarn 
- Uma instancia do PostgreSQL

Obs: Recomendado docker

  ##  Getting started
  #### 1° - Executar comando para clonar o repositorio:
  $ git clone "https://github.com/zagob/TCC-Projeto-EAD_backend.git"
  #### 2° - Executar comando para instalar todas as dependêcias que o projeto necessita
  $ git yarn
  #### 3° - Para o projeto estar funcionando, voçê deve instalar uma ferrameta chamado docker, segue abaixo o link para download
  - Disponível em https://docs.docker.com/docker-for-windows/install/
  #### 4° - Após a instalção, executar comando abaixo para criar uma instância do Postgres
  $ docker run --name postgres -e POSTGRES_USER=docker -e POSTGRES_DB=proffy -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres
  #### 5° - Comando para executar as migrations e criar as tabelas
  $ yarn typeorm migration:run
  #### 6° - Executar projeto
  $ yarn dev
