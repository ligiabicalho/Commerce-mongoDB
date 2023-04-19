# :sparkles: Projeto Commerce - MongoDB :hamburger:

Colocando em prática os aprendizados de MongoDB, com base nos dados do cardápio do McDonald's.

## Sumário

- [Sobre o projeto](#sobre-o-projeto)
  - [Contexto](#man_technologist-contexto)
- [Tecnologias utilizadas](#tecnologias-utilizadas)
  - [Banco de dados](#banco-de-dados)
- [Instalação](#instalando-localmente)
  - [Docker](#docker)
- [Status de desenvolvimento](#status-de-desenvolvimento)
- [Desenvolvedora](#desenvolvedora)
- [Agradecimentos](#agradecimentos)

<br>

# Sobre o projeto

## :man_technologist: Contexto

Esse projeto consiste em uma lista de desafios avaliativos para consolidar os conceitos relacionados ao banco de dados NoSQL, MongoDB.

Nesse projeto, trabalhei a partir do banco de dados `commerce`, que contém dados do cardápio do McDonald's, como ingredientes, valores nutricionais e dados fictícios de vendas.

<p align="right"><a href="#sparkles-projeto-commerce-MongoDB-hamburger">:top:</a></p>

# Tecnologias utilizadas

- Docker

### Banco de dados

- MongoDB

<p align="right"><a href="#sparkles-projeto-commerce-MongoDB-hamburger">:top:</a></p>

## Instalação

Caso deseje rodar o projeto na sua máquina, siga as orientações:

> ⚠️ Configurações mínimas para execução do projeto
>
> - Preferencialmente Sistema Operacional Distribuição Unix
> - Node versão 16
> - Docker
> - Docker-compose versão >=1.29.2

```bash
  # Clone o repositório
  git clone git@github.com:ligiabicalho/Commerce-mongoDB.git
  # Navegue até a pasta do repositório clonado
  cd Commerce-mongoDB
  # Instalar as dependências é necessário apenas para correção de Lint.
  npm install
```

### **Usando Docker**

```bash
  # No diretório raíz, crie um container com um volume apontando para a pasta do projeto
  # com o comando:
  docker run -d --name=mongodb -v "$PWD:/app" -p 27017:27017 mongo:5
  # Com o container em execução, acesse o terminal do container
  docker exec -it mongodb bash
  # No terminal do container, acesse o diretório /app mapeado no volume conforme o passo 1.
  cd app
```

1. :  
   `npm run compose:up`
2. Em seguida abra o terminal interativo do container:  
   `docker exec -it app_backend sh`
3. Instale as dependências dentro do container:  
   `npm install`

<p align="right"><a href="#sparkles-bem-vindo-ao-repositório-do-projeto-delivery-app">:top:</a></p>

## Requisitos do projeto

> _Clique na seta para ver a lista de requisitos que recebemos para desenvolver durante o processo avaliativo._

<p align="right"><a href="#sparkles-projeto-commerce-MongoDB-hamburger">:top:</a></p>

## Status de desenvolvimento

100% dos requisitos solicitados foram desenvolvidos.

## Desenvolvedora

<a href="https://github.com/ligiabicalho">
  <img src="https://avatars.githubusercontent.com/u/108960742" width="100px" alt="Ligia Bicalho"/>
  <a href="https://linkedin.com/in/ligiabicalho" target="_blank">
  <p>:information_source: Lígia Bicalho</p>
</a>

## Agradecimentos

A Trybe e seus instrutures pelos ensinamentos, elaboração do desafio e mentorias técnicas.
Aos colegas de turma pelas valiosas discussões, devidamente referenciadas nos comentários do código.

<p align="right"><a href="#sparkles-projeto-commerce-MongoDB-hamburger">:top:</a></p>
