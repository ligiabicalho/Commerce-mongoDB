# :sparkles: Projeto Commerce - MongoDB :hamburger:

Colocando em prática os aprendizados de MongoDB, com base em informações do cardápio do McDonald's.

## Sumário

- [Sobre o projeto](#sobre-o-projeto)
  - [Contexto](#man_technologist-contexto)
  - [Habilidades](#habilidades)
- [Tecnologias utilizadas](#tecnologias-utilizadas)
  - [Banco de dados](#banco-de-dados)
- [Instalação](#instalando-localmente)
  - [Docker](#docker)
- [Status de desenvolvimento](#status-de-desenvolvimento)
- [Desenvolvedora](#desenvolvedora)
- [Agradecimentos](#agradecimentos)

## Sobre o projeto

### :man_technologist: Contexto

Esse projeto consiste em uma lista de desafios avaliativos para consolidar os conceitos relacionados ao banco de dados NoSQL, MongoDB.

Nesse projeto, trabalhei a partir do banco de dados `commerce`, que contém informações do cardápio do McDonald's, como ingredientes, valores nutricionais e dados fictícios de vendas.  
Minha responsabilidade foi escrever as _queries_ necessárias para pesquisar e atualizar os dados para atender ao que era solicitado em cada requisito.

### Habilidades

- Pesquisar documentos no banco de dados usando o find();
- Especificar os dados retornados do documento com _projection_.
- Filtrar resultado das pesquisas, usando _operadores lógicos_ e de _comparação_:
  - `$and, $or, $not, $nor, $exists.`
  - `$lt, $lte, $gt, $gte, $eq, $ne, $in, $nin.`
- Limitar, pular, ordenar os documentos retornados, com os métodos:
  - `limit(), skip(), sort()`;
- Utilizar operadores de consulta em array:
  - ` $all, $elementMatch, $size, $expr, $regex, $mod`.
- Fazer atualizações nos documentos utilizando os operadores:
  - `$set, $mul, $inc, $min, $max e $currentDate`.
- Renomear campos com `$rename` e remover com `$unset`.
- Incorporar dados aos documentos através de arrays utilizando os operadores:
  - `$pop, $pull, $push, $addToSet, $each, $slice e $sort`.

## Tecnologias utilizadas

- Docker

### Banco de dados

- MongoDB

<p align="right"><a href="#sparkles-projeto-commerce---mongodb-hamburger">:top:</a></p>

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
  # Neste caso, instalar as dependências é necessário apenas para correção de Lint.
  npm install
```

### **Usando o MongoDB com Docker**

```bash
  # No diretório raíz, crie um container com um volume apontando para a pasta do projeto
  # com o comando:
  docker run -d --name=mongodb -v "$PWD:/app" -p 27017:27017 mongo:5
  # Com o container em execução, acesse o terminal do container
  docker exec -it mongodb bash
  # No terminal do container, acesse o diretório /app mapeado no volume conforme o passo 1.
  cd app
```

<p align="right"><a href="#sparkles-bem-vindo-ao-repositório-do-projeto-delivery-app">:top:</a></p>

## Requisitos do projeto

Esse projeto consistiu em 32 desafios/requisitos, onde para cada um tivemos que escrever uma ou mais _querys_ para pesquisar e/ou atualizar os dados e alcançar o resultado requerido.  
Os commits foram nomeados com cada uma das solicitações.

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
Aos colegas de turma pelas valiosas discussões, importantes para o aprimoramento das habilidades.

<p align="right"><a href="#sparkles-projeto-commerce---mongodb-hamburger">:top:</a></p>
