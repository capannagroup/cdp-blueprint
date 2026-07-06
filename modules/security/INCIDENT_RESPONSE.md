# Incident Response

## Purpose

The Incident Response Plan defines the process for detecting, responding to, recovering from, and preventing cybersecurity incidents within the Capanna Digital Platform.

---

## Incident Lifecycle

### 1. Preparation

- Security monitoring
- Backup strategy
- Employee awareness
- Incident response team

---

### 2. Detection

Examples:

- Unauthorized login
- API attacks
- Malware
- Data breach
- Service outage

Detection Sources

- SIEM
- Audit Logs
- IDS/IPS
- Monitoring Systems
- User Reports

---

### 3. Analysis

Determine:

- Severity
- Impact
- Affected Systems
- Root Cause

Severity Levels

| Level | Description |
|-------|-------------|
| Critical | Production outage or data breach |
| High | Major service disruption |
| Medium | Limited impact |
| Low | Minor issue |

---

### 4. Containment

Immediate Actions

- Disable accounts
- Block IPs
- Revoke JWT tokens
- Isolate affected servers
- Enable emergency firewall rules

---

### 5. Eradication

- Remove malware
- Patch vulnerabilities
- Rotate secrets
- Update passwords
- Remove unauthorized access

---

### 6. Recovery

- Restore backups
- Verify system integrity
- Resume production
- Monitor closely

---

### 7. Lessons Learned

Create a post-incident report including:

- Timeline
- Root Cause
- Impact
- Recovery Actions
- Preventive Measures

---

## Incident Response Team

- Security Lead
- Infrastructure Team
- Development Team
- Management
- Legal (if required)

---

## Review

The Incident Response Plan is tested annually and reviewed after every major incident.
