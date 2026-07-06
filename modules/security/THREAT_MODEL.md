# Threat Model

## Purpose

The Threat Model identifies potential security threats to the Capanna Digital Platform and defines mitigation strategies to reduce risk.

---

## Security Objectives

- Confidentiality
- Integrity
- Availability
- Accountability
- Non-Repudiation

---

## Threat Categories

### Spoofing

- Fake user identity
- Stolen credentials
- Session hijacking

Mitigation

- MFA
- JWT validation
- OAuth2
- Secure Cookies

---

### Tampering

Examples

- API modification
- Request manipulation
- SQL Injection

Mitigation

- Input validation
- Parameterized queries
- HTTPS
- Encryption

---

### Repudiation

Examples

- User denies actions
- Missing audit records

Mitigation

- Audit Logging
- Immutable Logs
- Digital Signatures

---

### Information Disclosure

Examples

- Sensitive data exposure
- Token leakage
- Password leaks

Mitigation

- AES Encryption
- HTTPS
- Secrets Management
- RBAC

---

### Denial of Service

Examples

- API flooding
- Login attacks
- Resource exhaustion

Mitigation

- Rate Limiting
- WAF
- Auto Scaling
- CDN

---

### Elevation of Privilege

Examples

- Permission escalation
- Admin access abuse

Mitigation

- RBAC
- Least Privilege
- Permission Validation
- Authorization Middleware

---

## Threat Assessment

Each threat is evaluated using:

- Impact
- Likelihood
- Risk Score
- Mitigation Strategy

---

## Review Process

Threat model reviews occur:

- Before major releases
- Quarterly
- After security incidents
