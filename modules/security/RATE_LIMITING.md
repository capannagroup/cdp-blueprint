# Rate Limiting

## Purpose

This document defines how API rate limiting protects the Capanna Digital Platform against abuse, denial-of-service attacks, and excessive usage.

---

## Objectives

- Prevent API abuse
- Protect backend services
- Ensure fair usage
- Reduce bot traffic
- Improve platform stability

---

## Default Limits

| Endpoint Type | Limit |
|---------------|------:|
| Public API | 60 requests/minute |
| Authenticated API | 300 requests/minute |
| Login API | 5 attempts/minute |
| Password Reset | 3 attempts/hour |
| Admin API | 100 requests/minute |

---

## Rate Limit Strategy

The platform uses:

- Token Bucket Algorithm
- IP-based limiting
- User-based limiting
- API Key limiting

---

## Response

When a limit is exceeded:

HTTP Status

```
429 Too Many Requests
```

Headers returned:

```
Retry-After
X-RateLimit-Limit
X-RateLimit-Remaining
X-RateLimit-Reset
```

---

## Exemptions

The following are exempt:

- Internal services
- Health checks
- Monitoring systems

---

## Logging

Log:

- User ID
- IP Address
- Endpoint
- Timestamp
- Request Count

---

## Best Practices

- Use API Gateway
- Cache frequent requests
- Block abusive IPs
- Apply different limits per endpoint
- Monitor rate-limit events
