# OAuth 2.0

## Purpose

This document defines how OAuth 2.0 is implemented within the Capanna Digital Platform for secure delegated authorization.

---

## Supported Grant Types

- Authorization Code + PKCE
- Client Credentials
- Refresh Token

Not Supported:

- Implicit Flow
- Password Grant

---

## Authorization Flow

1. User requests login
2. Identity Provider authenticates user
3. Authorization Code issued
4. Backend exchanges code for tokens
5. Access Token returned
6. Refresh Token stored securely

---

## Token Types

### Access Token

- JWT
- 15-minute lifetime
- Used for API access

### Refresh Token

- 30-day lifetime
- Rotated after each use
- Revoked on logout

---

## Scopes

Examples:

- profile
- email
- orders.read
- orders.write
- inventory.read
- inventory.write
- admin

---

## Supported Identity Providers

- Microsoft Entra ID
- Google
- Apple
- GitHub
- Internal Identity Provider

---

## Token Validation

Every request validates:

- Signature
- Expiration
- Issuer
- Audience
- Scopes

---

## Security

- HTTPS only
- PKCE required
- Refresh token rotation
- Short-lived access tokens
- Token revocation supported

---

## Best Practices

- Never expose client secrets
- Use Authorization Code Flow
- Require PKCE
- Rotate refresh tokens
- Validate all claims
