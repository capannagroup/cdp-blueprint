# Dependency Rules

## Purpose

This document defines the allowed dependencies between layers and modules of the Capanna Digital Platform (CDP).

These rules are mandatory.

---

# Layer Dependencies

Presentation

↓

Application

↓

Domain

↓

Infrastructure

Dependencies always point downward.

Infrastructure never calls Presentation.

Domain never depends on Infrastructure.

---

# Module Dependencies

Allowed

Production

↓

Engineering

↓

Products

↓

Identity

Warehouse

↓

Products

↓

Identity

Sales

↓

CRM

↓

Identity

Purchasing

↓

Suppliers

↓

Identity

---

Forbidden

Production → Sales Database

Production → CRM Database

Engineering → Production Database

Warehouse → Production Database

Modules communicate only through APIs or Events.

---

# Database Rules

Each module owns its own schema.

No module writes into another module database.

Read operations use APIs.

Cross-module synchronization uses events.

---

# API Rules

REST

GraphQL

gRPC

are acceptable.

Direct SQL between modules is prohibited.

---

# Event Rules

Every business event must contain

Event ID

Timestamp

Module

Version

Payload

Correlation ID

---

# AI Rules

AI agents never bypass business services.

AI accesses only documented APIs.

AI never writes directly into databases.

---

# Security Rules

Authentication required.

Authorization required.

Audit required.

Encryption required.

---

# Future Compatibility

All new modules must comply with these dependency rules.

Exceptions require an approved Architecture Decision Record (ADR).
