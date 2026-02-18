# 📘 Conceitos Básicos de GraphQL

## 🔹 Input
Representa dados de entrada utilizados em mutations ou queries.  
Normalmente define a estrutura esperada para criação ou atualização de dados.

> Equivalente a um DTO de request.

---

## 🔹 Type
Define o modelo/estrutura de dados retornado pela API.

> Equivalente a uma classe de resposta ou entidade exposta no schema.

Exemplo:

```graphql
type Category {
  id: ID!
  name: String!
  description: String
}
```
---

## 🔹 Mutation
Responsável por criar, atualizar ou remover dados.

Qualquer operação que altere o estado da aplicação deve ser feita via mutation.

> Equivalente a POST, PUT, PATCH ou DELETE no REST.

Exemplo:

```graphql
mutation {
  createCategory(input: {
    name: "Nova Categoria",
    description: "Descrição"
  }) {
    id
    name
  }
}
```
---

## 🔹 Query
Utilizada para consultar dados.

Toda operação que apenas busca informações deve ser feita via query.

> Equivalente a GET no REST.

---

## 🚀 Comandos com gqlgen (Go)
Inicializar projeto GraphQL

```bash
go run github.com/99designs/gqlgen init
```

Gerar/Atualizar código após alterações no schema

```bash
go run github.com/99designs/gqlgen generate
```
