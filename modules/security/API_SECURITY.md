# API Security

## Purpose

This document defines how APIs are secured across the Capanna Digital Platform.

---

## Authentication

All APIs require authentication unless explicitly marked as Public.

Supported methods:

- JWT Bearer Token
- OAuth2
- API Keys (Internal Services)

---

## Authorization

Authorization is enforced using:

- RBAC
- Permissions
- Claims
- Resource Ownership

---

## API Gateway

Responsibilities:

- Authentication
- Authorization
- Rate Limiting
- Request Validation
- Logging
- API Versioning

---

## Request Validation

Every request validates:

- Content Type
- JSON Schema
- Required Fields
- Maximum Payload Size

---

## HTTPS

All APIs require HTTPS.

TLS 1.3 preferred.

HTTP requests are redirected.

---

## CORS

Allowed Origins:

- app.capanna.com
- admin.capanna.com

Credentials allowed.

---

## Security Headers

- Strict-Transport-Security
- X-Content-Type-Options
- X-Frame-Options
- Referrer-Policy

---

## API Versioning

Example:

/api/v1/customers

/api/v2/customers

---

## Logging

Every API request logs:

- User ID
- Endpoint
- Timestamp
- IP Address
- Response Code

---

## Best Practices

- Never expose stack traces
- Validate every request
- Use HTTPS
- Use JWT
- Apply least privilege
