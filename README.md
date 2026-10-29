# API REST com Spring Boot

API REST com dois recursos, produtos e filmes, construída com Spring Boot e banco em memória.

> Projeto desenvolvido no curso **Back End Java da Ada Tech em parceria com o Mercado Livre**.

## Endpoints

| Recurso | Rota base | Operações |
|---|---|---|
| Produtos | `/api/produtos` | `GET` listar, `POST` criar, `PUT /{id}` atualizar, `DELETE /{id}` remover |
| Filmes | `/api/filmes` | `GET` listar, `POST` criar, `PUT` atualizar, `DELETE /{id}` remover |

## Arquitetura

Camadas separadas por responsabilidade:

- **Controller:** recebe as requisições HTTP e devolve as respostas
- **Service:** concentra a regra de negócio
- **Model:** entidades `Produto`, `FilmeModel` e o objeto de busca `Busca`

## Stack

`Java` `Spring Boot` `Spring Web` `H2` `Lombok` `Maven`

## Como executar

```bash
mvn spring-boot:run
```

A API sobe em `http://localhost:8080`.
