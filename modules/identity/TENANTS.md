# Tenants

---

# Overview

The Tenant component represents the highest logical isolation boundary within the Capanna Digital Platform (CDP).

A Tenant owns all platform resources including organizations, users, applications, data, configurations, security policies, integrations, and AI services.

No data may cross tenant boundaries unless explicitly configured through trusted federation or approved cross-tenant collaboration mechanisms.

The Tenant architecture enables secure multi-tenancy while maintaining complete data isolation, scalability, compliance, and operational independence.

---

# Objectives

The Tenant component provides:

- Multi-tenant architecture
- Complete data isolation
- Independent administration
- Independent security policies
- Independent branding
- Independent integrations
- Independent AI services
- Independent billing
- Independent licensing

---

# Responsibilities

The Tenant component manages:

- Tenant lifecycle
- Tenant configuration
- Subscription
- Licensing
- Organizations
- Security policies
- Identity providers
- AI configuration
- Regional settings
- Billing information
- Compliance settings

---

# Tenant Architecture

```text
Capanna Digital Platform
│
├── Tenant A
│     ├── Organizations
│     ├── Users
│     ├── ERP
│     ├── CRM
│     ├── Manufacturing
│     ├── Finance
│     └── AI
│
├── Tenant B
│     ├── Organizations
│     ├── Users
│     ├── ERP
│     ├── CRM
│     ├── Manufacturing
│     └── AI
│
└── Tenant C
      └── ...
```

---

# Tenant Types

| Type | Description |
|------|-------------|
| Enterprise | Large company |
| SMB | Small and Medium Business |
| Manufacturing | Industrial customer |
| Government | Government entity |
| Education | Educational institution |
| Partner | Business partner |
| Internal | Capanna internal tenant |
| Development | Testing environment |

---

# Core Properties

| Property | Description |
|-----------|-------------|
| Tenant ID | Unique identifier |
| Tenant Code | Unique code |
| Name | Display name |
| Display Name | Public name |
| Owner | Primary administrator |
| Subscription | Current subscription |
| License | License information |
| Region | Hosting region |
| Time Zone | Default timezone |
| Currency | Default currency |
| Language | Default language |
| Status | Operational state |
| Created At | Creation date |
| Updated At | Last modification |

---

# Tenant Lifecycle

```text
Provisioned
      │
Configured
      │
Licensed
      │
Activated
      │
Operational
      │
Suspended
      │
Archived
```

---

# Tenant States

| State | Description |
|--------|-------------|
| Draft | Newly created |
| Active | Operational |
| Suspended | Temporarily disabled |
| Locked | Compliance restriction |
| Expired | License expired |
| Archived | Historical |
| Deleted | Soft deleted |

---

# Tenant Isolation

Every Tenant has isolated:

- Database records
- Users
- Organizations
- Files
- Documents
- APIs
- AI Models
- Manufacturing Data
- Financial Data
- CRM Data
- Audit Logs

No resource may be shared unless explicitly enabled.

---

# Tenant Hierarchy

```text
Tenant
│
├── Organizations
│      ├── Teams
│      ├── Departments
│      ├── Users
│      └── Assets
│
├── Applications
│
├── Security
│
├── Integrations
│
└── AI Services
```

---

# Subscription Plans

Supported plans:

- Community
- Starter
- Professional
- Enterprise
- Manufacturing Enterprise
- Government

---

# Resource Limits

Tenant limits may include:

- Users
- Organizations
- Storage
- API requests
- AI tokens
- Manufacturing machines
- Warehouses
- Projects
- Documents

---

# Database Schema

Primary table

```text
tenants
```

Important fields

- tenant_id
- tenant_code
- name
- owner_user_id
- subscription
- license_key
- region
- timezone
- currency
- language
- status
- created_at
- updated_at

---

# Relationships

A Tenant owns:

- Organizations
- Users
- Roles
- Groups
- Applications
- API Keys
- AI Models
- Documents

A Tenant may contain multiple Organizations.

---

# REST API

## List tenants

GET /tenants

## Get tenant

GET /tenants/{tenantId}

## Create tenant

POST /tenants

## Update tenant

PUT /tenants/{tenantId}

## Suspend tenant

POST /tenants/{tenantId}/suspend

## Activate tenant

POST /tenants/{tenantId}/activate

## Archive tenant

DELETE /tenants/{tenantId}

---

# Events

The Tenant module publishes:

- TenantCreated
- TenantUpdated
- TenantActivated
- TenantSuspended
- TenantArchived
- TenantDeleted
- SubscriptionChanged
- LicenseExpired

---

# Permissions

| Permission | Description |
|------------|-------------|
| Tenant.View | View tenant |
| Tenant.Create | Create tenant |
| Tenant.Update | Modify tenant |
| Tenant.Delete | Archive tenant |
| Tenant.Security | Manage security |
| Tenant.Settings | Manage configuration |
| Tenant.Subscription | Manage licensing |
| Tenant.Administration | Full administration |

---

# Validation Rules

Tenant Name

- Required
- Unique

Tenant Code

- Required
- Immutable
- Uppercase
- Globally unique

Region

- Supported hosting region

Language

- ISO language code

Currency

- ISO-4217

---

# Security

Tenant isolation is mandatory.

Cross-tenant authentication is disabled by default.

Every API request must contain Tenant Context.

Every database query must include Tenant ID filtering.

Administrative operations require Tenant Administrator privileges.

---

# Audit Logging

The following actions are audited:

- Tenant creation
- Configuration changes
- Subscription updates
- License changes
- Security policy updates
- Administrator assignment
- Region changes
- Suspension
- Activation
- Archive

---

# Best Practices

- Never hard delete tenants.
- Enforce tenant isolation at every layer.
- Keep tenant codes immutable.
- Encrypt tenant secrets.
- Maintain separate encryption keys per tenant.
- Enable audit logging by default.
- Apply least privilege principles.

---

# Future Enhancements

- Multi-region replication
- Cross-region failover
- Tenant cloning
- Automated provisioning
- Self-service onboarding
- AI tenant optimization
- Usage analytics
- Billing automation
- Compliance dashboards
- Disaster recovery orchestration
