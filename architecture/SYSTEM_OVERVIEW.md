# CDP System Overview

## High Level Architecture

```
                   ┌─────────────────────┐
                   │     Web Portal      │
                   └──────────┬──────────┘
                              │
                   ┌──────────▼──────────┐
                   │      API Gateway    │
                   └──────────┬──────────┘
                              │
      ┌───────────────────────┼────────────────────────┐
      │                       │                        │
┌─────▼─────┐         ┌───────▼──────┐        ┌────────▼────────┐
│ Security  │         │ Business     │        │ AI Services     │
│ Module    │         │ Modules      │        │                 │
└─────┬─────┘         └───────┬──────┘        └────────┬────────┘
      │                       │                        │
      └──────────────┬────────┴──────────────┬─────────┘
                     │                       │
             ┌───────▼────────┐      ┌──────▼───────┐
             │ PostgreSQL     │      │ Redis Cache  │
             └────────────────┘      └──────────────┘
```

---

## Layers

Presentation

↓

API

↓

Application

↓

Domain

↓

Infrastructure

↓

Database

---

## Principles

- Domain Driven Design
- Clean Architecture
- CQRS
- MediatR
- SOLID
- Event Driven
- Multi-Tenant
- API First
- AI First
