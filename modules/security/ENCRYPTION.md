# Encryption

## Purpose

Encryption protects sensitive data stored and transmitted within the Capanna Digital Platform.

---

## Encryption Types

### Data in Transit

- HTTPS
- TLS 1.3
- Secure API Communication

---

### Data at Rest

- AES-256 Encryption
- Database Encryption
- File Encryption
- Backup Encryption

---

## Password Encryption

Passwords are never stored in plain text.

Recommended algorithms:

- Argon2id
- bcrypt

---

## Secret Management

Secrets must never be hardcoded.

Use:

- Environment Variables
- Secret Vault
- GitHub Secrets

---

## Encryption Keys

- Rotate keys regularly.
- Store separately from encrypted data.
- Restrict access.

---

## Best Practices

- Encrypt all sensitive information.
- Use strong cryptographic libraries.
- Rotate certificates before expiration.
- Never expose encryption keys.
