# Multi-Factor Authentication (MFA)

## Purpose

Multi-Factor Authentication (MFA) adds an additional security layer beyond passwords.

---

## Supported Methods

- Authenticator App (TOTP)
- Email Verification
- SMS Verification
- Hardware Security Keys (FIDO2)
- Passkeys

---

## Authentication Flow

1. User enters username.
2. User enters password.
3. System validates credentials.
4. MFA challenge is generated.
5. User submits verification code.
6. Access token is issued.

---

## Recovery Methods

- Backup Codes
- Recovery Email
- Administrator Verification

---

## Security Policies

- MFA required for Administrators.
- MFA required for Finance users.
- MFA optional for Customers.
- Remember trusted devices for 30 days.

---

## Best Practices

- Prefer Authenticator Apps over SMS.
- Rotate backup codes annually.
- Log all MFA events.
- Detect suspicious login attempts.
