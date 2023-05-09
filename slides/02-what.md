# What?

## An RPC framework

Made by Facebook in 2015

## Basics

- Single endpoint (POST)
- Aggregates "leaf nodes"
    - SQL
    - NoSQL
    - External APIs
- Unique Query Syntax

## Features: Type System

strings, numbers, and IDs

```graphql
type Query {
  currentUser: User
}

type User {
  id: ID!
  name: String!
}
```

## Features: Queries

```graphql
query CurrentUser {
  currentUser {
    name
  }
}
```

## Features: Mutations

```graphql
mutation CreateUser($name: String!, $age: Int!) {
  createUser(userName: $name, age: $age) {
    name
    age
  }
}
```

## Features: Subscriptions

In spec but Client/Server implementation specific

```
subscription {
  newPerson {
    name
    age
  }
}
```
