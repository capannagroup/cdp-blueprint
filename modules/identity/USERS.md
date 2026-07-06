# Users

## Overview

The Users component is the central identity entity within the Capanna Digital Platform (CDP). Every authenticated person or machine interacting with the platform is represented as a User.

The module manages the complete user lifecycle, identity attributes, authentication integration, authorization assignments, auditing, and compliance across all CDP modules.

---

## Objectives

The Users component provides:

- Centralized user management
- Identity lifecycle management
- Multi-tenant support
- Organization-aware user assignments
- Authentication integration
- Authorization integration
- User profile management
- Account security
- Audit logging
- Regulatory compliance

---

# User Types

| Type | Description |
|------|-------------|
| Platform Administrator | Full platform control |
| Organization Administrator | Manages an organization |
| Department Manager | Manages departments |
| Team Leader | Manages team members |
| Employee | Internal employee |
| Customer | External customer |
| Supplier | Vendor account |
| Contractor | Temporary workforce |
| Guest | Limited access |
| API User | Machine account |
| Service Account | Background services |

---

# User Lifecycle

```
Draft
   │
   ▼
Invited
   │
   ▼
Registered
   │
   ▼
Email Verified
   │
   ▼
Active
   │
   ├─────────────► Suspended
   │                    │
   │                    ▼
   │                 Reactivated
   │
   ├─────────────► Locked
   │                    │
   │                    ▼
   │                 Unlocked
   │
   ▼
Archived
   │
   ▼
Deleted (Soft Delete)
```

---

# User Status

Supported statuses:

- Pending
- Invited
- Registered
- Active
- Suspended
- Locked
- Disabled
- Archived
- Deleted

---

# User Profile

Each user stores:

- User ID
- Username
- Email
- Phone Number
- Full Name
- Display Name
- Avatar
- Preferred Language
- Time Zone
- Job Title
- Employee Number
- Department
- Organization
- Tenant
- Account Status
- Created Date
- Last Login

---

# Authentication

Supported methods:

- Username / Password
- Email Login
- Mobile Login
- OAuth2
- OpenID Connect
- SAML 2.0
- Single Sign-On (SSO)
- Multi-Factor Authentication (MFA)
- Passkeys
- API Tokens

---

# Authorization

Permissions are inherited through:

- Roles
- Groups
- Policies
- Organizations
- Teams

---

# Relationships

A user may belong to:

- Multiple Organizations
- Multiple Teams
- Multiple Departments
- Multiple Projects
- Multiple Applications

---

# Security

Security controls include:

- Password Policies
- MFA Enforcement
- Login Monitoring
- Session Management
- Device Registration
- Geo Restrictions
- IP Restrictions
- Risk Detection
- Account Lockout

---

# Audit Logging

Every important action is recorded.

Examples:

- Login
- Logout
- Failed Login
- Password Change
- Email Change
- MFA Enabled
- MFA Disabled
- Role Assignment
- Permission Change
- Profile Update
- User Lock
- User Unlock
- User Archive
- User Delete

---

# REST API

## User Management

```
GET    /users
GET    /users/{id}
POST   /users
PUT    /users/{id}
DELETE /users/{id}
```

## Lifecycle

```
POST /users/invite
POST /users/activate
POST /users/suspend
POST /users/unlock
POST /users/archive
POST /users/reset-password
```

---

# Database Tables

Core tables:

- Users
- UserProfiles
- UserRoles
- UserOrganizations
- UserTeams
- UserGroups
- UserSessions
- UserDevices
- UserTokens
- UserAuditLogs

---

# Events

The module publishes domain events.

- UserCreated
- UserInvited
- UserActivated
- UserUpdated
- UserSuspended
- UserLocked
- UserUnlocked
- PasswordChanged
- RoleAssigned
- UserArchived
- UserDeleted

---

# Best Practices

- Never hard delete users.
- Prefer soft deletion.
- Enable MFA for privileged users.
- Follow least privilege.
- Encrypt sensitive information.
- Log every security-sensitive action.
- Require verified email addresses.
- Review inactive accounts regularly.

---

# Future Roadmap

Future capabilities include:

- Passwordless Authentication
- Decentralized Identity (DID)
- Verifiable Credentials
- Identity Wallet
- AI Risk Scoring
- Behavioral Authentication
- Continuous Authentication
- Zero Trust Identity
