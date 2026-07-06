# Session Management

## Purpose

This document defines how user sessions are created, maintained, refreshed, and terminated within the Capanna Digital Platform.

---

## Session Types

### Web Session

- Secure HTTP Only Cookie
- SameSite=Strict
- Secure=True
- Idle timeout: 30 minutes

---

### Mobile Session

- JWT Access Token
- Refresh Token
- Device Binding

---

## Session Lifetime

| Session | Duration |
|----------|----------|
| Access Token | 15 Minutes |
| Refresh Token | 30 Days |
| Web Session | 30 Minutes Idle |

---

## Refresh Process

1. Access token expires
2. Refresh token validated
3. New access token issued
4. Old access token revoked

---

## Logout

Logout performs:

- Token Revocation
- Cookie Deletion
- Session Invalidation
- Audit Log Entry

---

## Session Security

- Device fingerprint validation
- IP anomaly detection
- Session timeout
- Concurrent session limits

---

## Best Practices

- Never store JWT in Local Storage
- Use Secure Cookies where possible
- Rotate Refresh Tokens
- Detect stolen sessions
- Log suspicious activity
