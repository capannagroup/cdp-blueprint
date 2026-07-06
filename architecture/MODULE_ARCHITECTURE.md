# Module Architecture

## Philosophy

Each business capability is implemented as an independent module.

Modules own their own business logic and expose functionality through APIs and events.

---

## Standard Module Structure

```
Module

API

Application

Domain

Infrastructure
```

---

## Responsibilities

### API

- Controllers
- Requests
- Responses
- Middleware
- Routes

---

### Application

- Commands
- Queries
- Handlers
- DTOs
- Validators
- Behaviors

---

### Domain

- Entities
- Value Objects
- Events
- Services
- Specifications
- Repository Interfaces

---

### Infrastructure

- EF Core
- Persistence
- Authentication
- Email
- Cache
- Logging
- External Providers

---

## Rules

Modules never access another module's database.

Communication happens through:

- Events
- Interfaces
- APIs

Never by SQL.
