# 📘 Conceitos Básicos de GraphQL

## 🔹 input
Representa dados de entrada utilizados em mutations ou queries.  
Normalmente define a estrutura esperada para criação ou atualização de dados.

> Equivalente a um DTO de request.

---

## 🔹 type
Define o modelo/estrutura de dados retornado pela API.

> Equivalente a uma classe de resposta ou entidade exposta no schema.

Exemplo:

```graphql
type Category {
  id: ID!
  name: String!
  description: String
}
