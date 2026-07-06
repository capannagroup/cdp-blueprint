# JWT (JSON Web Token)

## Purpose

The Capanna Digital Platform uses JSON Web Tokens (JWT) for stateless authentication between clients and backend services.

---

## Token Types

### Access Token

Used to access protected APIs.

Default lifetime:

- 15 Minutes

---

### Refresh Token

Used to generate a new Access Token.

Default lifetime:

- 30 Days

---

## JWT Payload

Contains:

- User ID
- Username
- Roles
- Permissions
- Tenant ID
- Token Version
- Expiration Date

---

## Security

- RS256 Signing
- HTTPS Only
- Short Expiration
- Refresh Token Rotation
- Revocation Support

---

## Validation Flow

1. Client sends JWT.
2. Gateway validates signature.
3. Expiration is checked.
4. Roles are extracted.
5. Permissions are evaluated.
6. Request proceeds.

---

## Future Improvements

- Token Blacklist
- Device Binding
- Session Revocation
- Geo-location Validation
