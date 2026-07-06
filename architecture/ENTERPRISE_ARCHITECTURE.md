# Capanna Digital Platform (CDP)

# Enterprise Architecture

**Version:** 1.0

**Status:** Approved Architecture

---

# 1. Mission

The Capanna Digital Platform (CDP) is a cloud-native SaaS platform designed specifically for the furniture manufacturing industry.

Its mission is to connect every business process, department, employee, customer, supplier, machine, and AI service into one intelligent digital ecosystem.

---

# 2. Vision

To become the world's leading digital operating system for furniture manufacturers.

CDP is designed to scale from a single factory to thousands of companies worldwide without changing the core architecture.

---

# 3. Core Principles

The platform follows these architectural principles.

- SaaS First
- Cloud Native
- API First
- AI First
- Security by Design
- Domain Driven Design (DDD)
- Clean Architecture
- Event Driven Architecture
- Modular Monolith evolving into Microservices
- Automation First

---

# 4. Multi-Tenant Architecture

The platform is designed as a multi-tenant SaaS application.

```
Platform
    │
    ├── Tenant
    │      │
    │      ├── Company
    │      │      │
    │      │      ├── Branch
    │      │      │
    │      │      ├── Department
    │      │      │
    │      │      ├── Users
    │      │      │
    │      │      └── Roles
```

Every tenant owns its own data while sharing the same platform.

---

# 5. Business Domains

CDP is organized around business domains.

## Platform

- Identity
- Security
- Administration
- Notifications
- Audit
- AI Platform

## Commercial

- CRM
- Sales
- Marketing
- Customer Service

## Operations

- Purchasing
- Inventory
- Warehouse
- Manufacturing
- Production Planning
- Logistics

## Enterprise

- Finance
- HR
- Projects
- Reporting
- Analytics

---

# 6. User Hierarchy

Platform Administrator

↓

Company Owner

↓

Executive Management

↓

Department Managers

↓

Supervisors

↓

Employees

↓

External Users

---

# 7. Data Ownership

Every business record belongs to:

- Tenant
- Company
- Branch
- Department

No data may cross tenant boundaries.

---

# 8. Security Model

Authentication

- JWT
- OAuth2

Authorization

- Role Based Access Control (RBAC)
- Policy Based Authorization

Security Features

- MFA Ready
- Audit Logging
- Encryption
- HTTPS
- Zero Trust Principles

---

# 9. AI Strategy

Artificial Intelligence is considered a core platform service.

Every module must expose AI capabilities.

Examples:

Inventory

- Demand prediction

Production

- Scheduling optimization

Quality

- Defect prediction

CRM

- Customer recommendations

Finance

- Cash-flow forecasting

Executive Dashboard

- Business insights

---

# 10. Integration Strategy

The platform integrates through APIs and Events.

Supported integrations include:

- ERP Systems
- Accounting Software
- Payment Providers
- IoT Devices
- CNC Machines
- PLC Controllers
- Barcode Scanners
- Mobile Applications

---

# 11. Scalability

The platform must support:

- Single factory deployment
- Multi-company deployment
- Regional deployment
- Global SaaS deployment

---

# 12. Technology Direction

Frontend

- React
- TypeScript

Backend

- ASP.NET Core

Database

- PostgreSQL

Messaging

- RabbitMQ

Caching

- Redis

Storage

- S3 Compatible Storage

Containers

- Docker

Orchestration

- Kubernetes

CI/CD

- GitHub Actions

---

# 13. Future Vision

The long-term goal is to create a Digital Factory Operating System capable of managing the complete lifecycle of furniture manufacturing through automation, AI, and cloud technologies.

---

# End of Document
