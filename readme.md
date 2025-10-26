# Contact

[Share your message, suggestions, questions or comments](https://forms.gle/HLKt8TrLtZT3zQHJ8)

# Books

| [MICROSERVICES: ZERO TO HERO!](https://hotmart.com/product/microservices/X102617285D) | [MICROSSERVIÇOS: DO INÍCIO AO FIM!](https://hotmart.com/pt-br/marketplace/produtos/microservices/A102616752Q) |
| :----------------------------------------------------------------: | :---------------------------------------------------------------------: |
| [![MICROSERVICES: ZERO TO HERO!](https://hotmart.s3.amazonaws.com/product_pictures/01486abc-d26b-4125-a8ea-4b2a212e4a86/Cover.png)](https://hotmart.com/product/microservices/X102617285D) | [![MICROSSERVIÇOS: DO INÍCIO AO FIM!](https://hotmart.s3.amazonaws.com/product_pictures/a2a7cc7f-de97-49fe-9fdb-1d6de5fe21a1/Cover.png)](https://hotmart.com/pt-br/marketplace/produtos/microservices/A102616752Q) |

# [Architecture](https://github.com/rafaelfgx/Architecture)

<img src="https://img.shields.io/github/stars/rafaelfgx/Architecture" height="30" />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="https://img.shields.io/github/forks/rafaelfgx/Architecture" height="30" />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="https://github.com/rafaelfgx/Architecture/actions/workflows/build.yaml/badge.svg" height="30" />

### .NET 9, Angular 20, Clean Architecture, Clean Code, SOLID Principles, KISS Principle, DRY Principle, Fail Fast Principle, Common Closure Principle, Common Reuse Principle, Acyclic Dependencies Principle, Mediator Pattern, Result Pattern, Folder-by-Feature Structure, Separation of Concerns

# [DotNetCore](https://github.com/rafaelfgx/DotNetCore)

<img src="https://img.shields.io/github/stars/rafaelfgx/DotNetCore" height="30" />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="https://img.shields.io/github/forks/rafaelfgx/DotNetCore" height="30" />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="https://github.com/rafaelfgx/DotNetCore/actions/workflows/publish.yaml/badge.svg" height="30" />&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="https://img.shields.io/badge/⭐️🚀_7+_Million_🚀⭐️-Downloads-blue" height="30" />

### .NET 9 Nuget Packages

### https://www.nuget.org/profiles/rafaelfgx

# [Microservices](https://github.com/rafaelfgx/Microservices)

<img src="https://github.com/rafaelfgx/Microservices/actions/workflows/build.yaml/badge.svg" height="30" />

### Screaming Architecture, Clean Architecture, Event-Driven Architecture, Clean Code, Domain-Driven Design, SOLID Principles, Test Pyramid, Patterns (Ambassador, Circuit Breaker, Mediator, Outbox, Result, Retry, Strategy), Java, Spring Boot, Kong, Keycloak, Kafka, MongoDB, Redis, Elastic, Kibana, Swagger, Testcontainers, Docker

![](https://raw.githubusercontent.com/rafaelfgx/Microservices/refs/heads/main/.docs/systemdesign.svg)

![](https://raw.githubusercontent.com/rafaelfgx/Microservices/refs/heads/main/.docs/tools.png)

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

# [Java](https://github.com/rafaelfgx/Java)

<img src="https://github.com/rafaelfgx/Java/actions/workflows/build.yaml/badge.svg" height="30" />

### Java 25, Spring Boot 3, Docker, Testcontainers, PostgreSQL, MongoDB, Kafka, LocalStack, AWS (SQS, S3), JWT, Swagger, Patterns (Mediator, Observer, Outbox, Strategy)

# [Node](https://github.com/rafaelfgx/Node)

<img src="https://github.com/rafaelfgx/Node/actions/workflows/build.yaml/badge.svg" height="30" />

### Node, Express, TypeScript, MongoDB, Jest, Joi, Testcontainers, ESLint, Prettier, Folder-by-Feature Structure

# [Nest](https://github.com/rafaelfgx/Nest)

<img src="https://github.com/rafaelfgx/Nest/actions/workflows/build.yaml/badge.svg" height="30" />

### Nest, JWT Authentication and Authorization, Swagger, Folder-by-Feature Structure

# [Blockchain](https://github.com/rafaelfgx/Blockchain)

### Blockchain, Wallet, Smart Contracts, Token, NFT, SBT, Solidity

# [General](https://github.com/rafaelfgx/General)

### Programming Paradigms (Object Oriented Programming, Functional Programming), Best Practices (SOLID, Design Patterns), Software Design (System Design, Architecture, DDD), Distributed Systems (Distributed Computing, Docker, Kubernetes), Artificial Intelligence (Machine Learning, MCP Servers)
