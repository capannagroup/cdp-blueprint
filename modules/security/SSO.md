# Single Sign-On (SSO)

## Purpose

Single Sign-On (SSO) allows users to authenticate once and securely access all Capanna Digital Platform services without signing in multiple times.

---

## Benefits

- One login
- Improved security
- Better user experience
- Centralized identity management
- Reduced password fatigue

---

## Supported Providers

- Microsoft Entra ID
- Google Workspace
- Okta
- Auth0
- Keycloak

---

## Authentication Flow

1. User requests application
2. Redirect to Identity Provider
3. User authenticates
4. Identity Provider issues token
5. Backend validates token
6. User session created

---

## Token Validation

Validate:

- Signature
- Expiration
- Audience
- Issuer
- Nonce

---

## Session Management

- Automatic session creation
- Logout propagation
- Session timeout
- Token refresh

---

## Security

- HTTPS only
- PKCE support
- MFA compatible
- Token encryption
- Secure cookies

---

## Best Practices

- Centralized identity provider
- Short-lived tokens
- MFA enforcement
- Logout everywhere
- Session monitoring
