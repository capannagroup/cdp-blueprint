# Password Policy

## Purpose

This document defines the password standards for all Capanna Digital Platform users.

---

## Requirements

- Minimum length: 12 characters
- Uppercase letter required
- Lowercase letter required
- Number required
- Special character required

Example:

Password@2026

---

## Password Rules

✓ Minimum 12 characters

✓ Maximum 128 characters

✓ Cannot contain username

✓ Cannot reuse last 10 passwords

✓ Expire every 180 days (Administrators)

✓ Customers do not expire

---

## Storage

Passwords are never stored in plain text.

Algorithm:

- Argon2id
or
- BCrypt

---

## Login Protection

After five failed attempts:

- Lock account for 15 minutes
- Log security event
- Notify administrator if repeated

---

## Password Reset

Reset token expires after 15 minutes.

Single use only.

Encrypted.

---

## Best Practices

- Never send passwords by email.
- Never log passwords.
- Enforce HTTPS.
- Use password managers.
