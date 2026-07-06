# Authentication

## Purpose

The Authentication component verifies the identity of every user accessing the Capanna Digital Platform.

---

## Supported Authentication Methods

- Username & Password
- JWT Token
- Refresh Token
- Multi-Factor Authentication (MFA)
- OAuth2 (Future)
- Microsoft Entra ID (Future)

---

## Authentication Flow

1. User submits credentials.
2. Credentials are validated.
3. JWT Access Token is issued.
4. Refresh Token is stored securely.
5. Client accesses protected APIs.
6. Token expiration is monitored.
7. Refresh Token generates a new Access Token.

---

## Components

- Login API
- Logout API
- Refresh Token API
- Password Hashing
- Session Management

---

## Security Standards

- HTTPS Only
- BCrypt Password Hashing
- JWT RS256 Signing
- Rate Limiting
- Account Lockout
- Password Complexity Policy

---

## Future Enhancements

- Single Sign-On (SSO)
- Biometric Authentication
- Passkeys (FIDO2)
