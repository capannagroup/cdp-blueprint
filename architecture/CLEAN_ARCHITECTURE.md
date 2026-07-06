# Clean Architecture

## Philosophy

The Capanna Digital Platform follows Uncle Bob's Clean Architecture.

The objective is to keep business logic independent from frameworks, databases and UI technologies.

---

## Layers

```
Presentation
        │
        ▼
Application
        │
        ▼
Domain
        │
        ▼
Infrastructure
```

---

## Responsibilities

### Presentation

- REST APIs
- Authentication
- Validation
- DTO Mapping

---

### Application

- Use Cases
- Commands
- Queries
- Event Handlers
- Business Workflows

---

### Domain

Contains:

- Entities
- Value Objects
- Aggregates
- Domain Events
- Domain Services
- Specifications
- Repository Interfaces

Contains NO:

- EF Core
- SQL
- HTTP
- JWT
- ASP.NET

---

### Infrastructure

Implements:

- Persistence
- Authentication
- Email
- Cache
- Logging
- File Storage
- AI Providers
- External APIs

---

## Dependency Rule

Presentation

↓

Application

↓

Domain

↑

Infrastructure implements interfaces defined by Domain and Application.

---

## Design Principles

- SOLID
- DDD
- CQRS
- MediatR
- Event Driven
- Repository Pattern
- Dependency Injection
- Open/Closed Principle
