# Security Headers

## Purpose

This document defines the HTTP security headers used across the Capanna Digital Platform.

---

## Required Headers

### Strict-Transport-Security

```
Strict-Transport-Security: max-age=31536000; includeSubDomains
```

Forces HTTPS.

---

### X-Content-Type-Options

```
X-Content-Type-Options: nosniff
```

Prevents MIME type sniffing.

---

### X-Frame-Options

```
X-Frame-Options: DENY
```

Protects against Clickjacking.

---

### Referrer-Policy

```
Referrer-Policy: strict-origin-when-cross-origin
```

Limits referrer leakage.

---

### Content-Security-Policy (CSP)

Example:

```
default-src 'self';
script-src 'self';
style-src 'self';
img-src 'self' https:;
font-src 'self';
connect-src 'self';
```

---

### Permissions-Policy

Disable unnecessary browser features.

Example:

```
camera=()
microphone=()
geolocation=()
payment=()
```

---

## Cookies

All authentication cookies must use:

- HttpOnly
- Secure
- SameSite=Strict

---

## Cache Headers

Sensitive responses:

```
Cache-Control: no-store
Pragma: no-cache
Expires: 0
```

---

## Best Practices

- Always use HTTPS
- Enable HSTS
- Use CSP
- Deny iframe embedding
- Disable browser sniffing
- Protect cookies
