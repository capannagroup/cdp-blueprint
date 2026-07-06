# Organizations

---

# Overview

The Organization component represents a legal or operational business entity within the Capanna Digital Platform (CDP).

Every user belongs to one or more organizations, and nearly all business data is scoped to an organization.

Organizations provide the highest business boundary inside the Identity module and are responsible for ownership of:

- Users
- Teams
- Departments
- Roles
- Assets
- Projects
- Manufacturing Plants
- Warehouses
- Financial Records
- CRM Data
- AI Models
- Documents

---

# Objectives

The Organization component enables:

- Multi-company architecture
- Business ownership separation
- Secure data isolation
- Cross-module integration
- Enterprise scalability
- Organization-level administration
- Compliance boundaries

---

# Responsibilities

The Organization component is responsible for:

- Organization lifecycle
- Organization hierarchy
- Organization settings
- Organization branding
- Organization ownership
- Organization administrators
- Business metadata
- Default configuration
- Organization policies

---

# Organization Types

| Type | Description |
|------|-------------|
| Enterprise | Large corporation |
| Manufacturing | Factory or production company |
| Retail | Retail company |
| Distributor | Distribution business |
| Service | Service provider |
| Government | Government organization |
| Educational | Educational institution |
| Non-Profit | Non-profit organization |

---

# Organization Hierarchy

```text
Organization
│
├── Business Units
├── Departments
├── Teams
├── Users
├── Projects
├── Warehouses
├── Manufacturing Plants
├── Assets
└── AI Services
```

---

# Core Properties

| Property | Description |
|-----------|-------------|
| Organization ID | Unique identifier |
| Organization Code | Short business code |
| Name | Display name |
| Legal Name | Registered company name |
| Tax Number | Tax registration |
| Country | Country |
| Region | State /Province |
| City | City |
| Address | Headquarters |
| Time Zone | Default timezone |
| Currency | Base currency |
| Language | Default language |
| Logo | Organization logo |
| Status | Current state |
| Created At | Creation date |
| Updated At | Last update |

---

# Lifecycle

```text
Created
    │
Configured
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

# Organization States

| State | Description |
|--------|-------------|
| Draft | Initial configuration |
| Active | Fully operational |
| Suspended | Temporarily disabled |
| Locked | Compliance restriction |
| Archived | Historical record |
| Deleted | Soft deleted |

---

# Ownership Model

Each organization contains:

- Owner
- Administrators
- Managers
- Members
- Guests

---

# Business Units

Example:

- Sales
- Manufacturing
- Engineering
- Procurement
- Marketing
- Finance
- Human Resources
- Information Technology

---

# Departments

Example departments include:

- Design
- Production
- CNC Operations
- Finishing
- Painting
- Packaging
- Warehouse
- Logistics
- Accounting
- Customer Service

---

# Relationships

An Organization owns:

- Users
- Roles
- Teams
- Groups
- Warehouses
- Assets
- Projects
- Documents

An Organization belongs to exactly one Tenant.

---

# Database Schema

**Primary Table**

```text
organizations
```

Important fields:

- organization_id
- tenant_id
- code
- name
- legal_name
- parent_organization_id
- owner_user_id
- tax_number
- country
- timezone
- currency
- language
- logo
- status
- created_at
- updated_at

---

# REST API

## Retrieve organizations

GET /organizations

## Retrieve organization

GET /organizations/{organizationId}

## Create organization

POST /organizations

## Update organization

PUT /organizations/{organizationId}

## Archive organization

DELETE /organizations/{organizationId}

## Organization users

GET /organizations/{organizationId}/users

## Organization teams

GET /organizations/{organizationId}/teams

## Organization roles

GET /organizations/{organizationId}/roles

---

# Events

The Organization module publishes:

- OrganizationCreated
- OrganizationUpdated
- OrganizationActivated
- OrganizationSuspended
- OrganizationArchived
- OrganizationDeleted

---

# Permissions

| Permission | Description |
|------------|-------------|
| Organization.View | View organization |
| Organization.Create | Create organization |
| Organization.Update | Modify organization |
| Organization.Delete | Archive organization |
| Organization.Settings | Manage settings |
| Organization.ManageUsers | Manage users |
| Organization.ManageTeams | Manage teams |
| Organization.ManageRoles | Manage roles |

---

# Validation Rules

Organization Name

- Required
- Unique inside Tenant

Organization Code

- Required
- Uppercase
- Immutable
- Unique

Country

- ISO-3166

Currency

- ISO-4217

Language

- ISO Language Code

---

# Security

Every organization is isolated.

Cross-organization access requires explicit authorization.

Administrative actions require Organization Administrator permission.

Sensitive changes are audited.

---

# Audit Logging

The following actions are logged:

- Organization creation
- Updates
- Ownership transfer
- Status changes
- Policy modifications
- Administrator assignment
- Archive operations

---

# Best Practices

- Never hard delete organizations.
- Use immutable organization codes.
- Separate production and testing organizations.
- Enable auditing.
- Enable organization policies.
- Minimize cross-organization permissions.

---

# Future Enhancements

- Organization templates
- Organization cloning
- Billing integration
- AI organization profile
- Health dashboard
- Compliance scoring
- Analytics
- Organization insights
