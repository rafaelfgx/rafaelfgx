# [Microservices](https://github.com/rafaelfgx/Microservices)

**Clean Architecture, Event-Driven Architecture, Clean Code, SOLID Principles, Resilience, Idempotency, Folder-by-Feature, Patterns (Mediator, Result, Strategy, Outbox, Retry, Circuit Breaker), Java, Spring Boot, Kong, Keycloak, Kafka, MongoDB, Redis, Elastic, Kibana, Swagger, Docker.**

![System Design](https://raw.githubusercontent.com/rafaelfgx/Microservices/refs/heads/main/.docs/systemdesign.svg)

![Tools](https://raw.githubusercontent.com/rafaelfgx/Microservices/refs/heads/main/.docs/tools.png)

```mermaid
sequenceDiagram
    participant Client
    participant AuthService
    participant CustomerService
    participant ProductService
    participant OrderService
    participant PaymentService
    participant Kafka

    Client->>AuthService: POST /auth
    AuthService-->>Client: JWT

    Client->>CustomerService: POST /customers
    CustomerService-->>Client: Customer Created

    Client->>ProductService: POST /products
    ProductService-->>Client: Product Created

    Client->>OrderService: POST /orders
    OrderService-->>Client: Order Created
    OrderService->>Kafka: OrderEvent Published

    Kafka-->>PaymentService: OrderEvent Consumed
    Note right of PaymentService: Payment Created

    Client->>PaymentService: PUT /payments/order/{orderId}/status/{status}
    PaymentService-->>Client: Payment Status Updated
    PaymentService->>Kafka: PaymentEvent Published

    Kafka-->>OrderService: PaymentEvent Consumed
    Note right of OrderService: Status Updated
```

# [Architecture](https://github.com/rafaelfgx/Architecture)

![](https://img.shields.io/github/stars/rafaelfgx/Architecture)
![](https://img.shields.io/github/forks/rafaelfgx/Architecture)
![](https://github.com/rafaelfgx/Architecture/actions/workflows/build.yaml/badge.svg)

**.NET 9, Angular 20, Clean Architecture, Clean Code, SOLID Principles, KISS Principle, DRY Principle, Fail Fast Principle, Common Closure Principle, Common Reuse Principle, Acyclic Dependencies Principle, Mediator Pattern, Result Pattern, Folder-by-Feature Structure, Separation of Concerns.**

# [DotNetCore](https://github.com/rafaelfgx/DotNetCore)

![](https://img.shields.io/github/stars/rafaelfgx/DotNetCore)
![](https://img.shields.io/github/forks/rafaelfgx/DotNetCore)
![](https://github.com/rafaelfgx/DotNetCore/actions/workflows/publish.yaml/badge.svg)

 **.NET 9 Nuget Packages**
 
 **⭐️🚀 7+ Million Downloads! 🚀⭐️**
 
 **https://www.nuget.org/profiles/rafaelfgx**

# [Java](https://github.com/rafaelfgx/Java)

![](https://img.shields.io/github/stars/rafaelfgx/Java)
![](https://img.shields.io/github/forks/rafaelfgx/Java)
![](https://github.com/rafaelfgx/Java/actions/workflows/build.yaml/badge.svg)

**Java 24, Spring Boot 3, Docker, Testcontainers, PostgreSQL, MongoDB, Kafka, LocalStack, AWS (SQS, S3), JWT, Swagger, Patterns (Mediator, Observer, Outbox, Strategy).**

# [Node](https://github.com/rafaelfgx/Node)

![](https://img.shields.io/github/stars/rafaelfgx/Node)
![](https://img.shields.io/github/forks/rafaelfgx/Node)
![](https://github.com/rafaelfgx/Node/actions/workflows/build.yaml/badge.svg)

**Node, Express, TypeScript, MongoDB, Jest, Joi, Testcontainers, ESLint, Prettier, Folder-by-Feature Structure.**

# [Nest](https://github.com/rafaelfgx/Nest)

![](https://img.shields.io/github/stars/rafaelfgx/Nest)
![](https://img.shields.io/github/forks/rafaelfgx/Nest)
![](https://github.com/rafaelfgx/Nest/actions/workflows/build.yaml/badge.svg)

**Nest, JWT Authentication and Authorization, Swagger, Folder-by-Feature Structure.**

# [Blockchain](https://github.com/rafaelfgx/Blockchain)

![](https://img.shields.io/github/stars/rafaelfgx/Blockchain)
![](https://img.shields.io/github/forks/rafaelfgx/Blockchain)

**Blockchain, Wallet, Smart Contracts, Token, NFT, SBT, Solidity.**

# Programming Paradigms

- [Object Oriented Programming](https://github.com/rafaelfgx/Utils/blob/main/root/ObjectOrientedProgramming.md)

- [Functional Programming](https://github.com/rafaelfgx/Utils/blob/main/root/FunctionalProgramming.md)

# Best Practices

- [SOLID](https://github.com/rafaelfgx/Utils/blob/main/root/SOLID.md)

- [Design Patterns](https://github.com/rafaelfgx/Utils/tree/main/root/DesignPatterns)

# Software Design

- [System Design](https://github.com/rafaelfgx/Utils/blob/main/root/SystemDesign.md)

- [Architecture](https://github.com/rafaelfgx/Utils/blob/main/root/Architecture.md)

- [DDD](https://github.com/rafaelfgx/Utils/blob/main/root/DDD.md)

# Distributed Systems

- [Distributed Computing](https://github.com/rafaelfgx/Utils/blob/main/root/DistributedComputing.md)

- [Docker](https://github.com/rafaelfgx/Utils/tree/main/root/Docker)

- [Kubernetes](https://github.com/rafaelfgx/Utils/tree/main/root/Kubernetes)

# Machine Learning

- [Machine Learning](https://github.com/rafaelfgx/Utils/blob/main/root/MachineLearning.md)

# [YouTube](https://www.youtube.com/@rafaelfgx)

- **[Introduction to Software Development](https://www.youtube.com/watch?v=_pIgLsGGioE) | [Introdução ao Desenvolvimento de Software](https://www.youtube.com/watch?v=v8jmNJo8aLg)**
- **[Cryptocurrencies](https://www.youtube.com/watch?v=njGubDWdJxA) | [Criptomoedas](https://www.youtube.com/watch?v=uqbtaSaey78)**