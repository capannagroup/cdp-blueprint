# Technology Stack

## Purpose

This document defines the official technology stack of the Capanna Digital Platform (CDP).

All applications, services and modules must comply with this standard unless an Architecture Decision Record (ADR) approves an exception.

---

# Frontend

| Layer | Technology |
|--------|------------|
| Web | React |
| Mobile | React Native |
| Desktop | Electron |
| UI Library | Material UI |
| State Management | Redux Toolkit |
| Charts | Apache ECharts |

---

# Backend

| Layer | Technology |
|--------|------------|
| Runtime | Node.js |
| Framework | NestJS |
| API | REST + GraphQL |
| Authentication | JWT + OAuth2 |
| Validation | Zod |

---

# Database

| Layer | Technology |
|--------|------------|
| Primary Database | PostgreSQL |
| Cache | Redis |
| Search | Elasticsearch |
| Object Storage | S3 Compatible |

---

# Messaging

| Service | Technology |
|----------|------------|
| Event Bus | RabbitMQ |
| Streaming | Kafka (Future) |

---

# Manufacturing

| Layer | Technology |
|--------|------------|
| PLC Integration | OPC-UA |
| CNC Integration | Custom Driver |
| Barcode | GS1 |
| RFID | EPC Gen2 |
| IoT Protocol | MQTT |

---

# AI

| Service | Technology |
|----------|------------|
| LLM | OpenAI |
| Embeddings | OpenAI |
| Vector Database | pgvector |
| OCR | Tesseract |

---

# DevOps

| Layer | Technology |
|--------|------------|
| Repository | GitHub |
| CI/CD | GitHub Actions |
| Containers | Docker |
| Orchestration | Kubernetes |
| Monitoring | Grafana |
| Logging | Loki |
| Metrics | Prometheus |

---

# Coding Standards

- TypeScript everywhere
- Clean Architecture
- Domain Driven Design
- Event Driven Architecture
- CQRS where appropriate
- SOLID Principles
- Semantic Versioning

---

# Supported Platforms

- Windows
- Linux
- Android
- iOS
- Web
