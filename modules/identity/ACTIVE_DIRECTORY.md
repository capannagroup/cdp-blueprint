# Active Directory

---

# Overview

The Active Directory component provides enterprise integration between the Capanna Digital Platform (CDP) and Microsoft Active Directory Domain Services (AD DS).

While LDAP provides generic directory communication, this component delivers Microsoft-specific capabilities including Windows authentication, Kerberos, Group Policy awareness, domain trust management, and enterprise identity synchronization.

The component allows organizations to leverage their existing Active Directory infrastructure without duplicating identities inside CDP.

---

# Objectives

The Active Directory component provides:

- Windows authentication
- Domain integration
- Forest integration
- Organizational Unit synchronization
- Group synchronization
- Kerberos authentication
- NTLM compatibility
- Trust relationship management
- Security group mapping
- Enterprise identity management

---

# Business Requirements

The platform shall:

- Connect to one or more Active Directory domains
- Support multiple forests
- Support domain trusts
- Authenticate Windows users
- Import users automatically
- Synchronize security groups
- Synchronize Organizational Units
- Detect disabled accounts
- Detect expired accounts
- Detect password expiration
- Detect account lockout
- Synchronize computer objects
- Synchronize service accounts
- Support hybrid deployments

---

# Supported Versions

- Windows Server 2016
- Windows Server 2019
- Windows Server 2022
- Microsoft Entra Connect
- Hybrid Active Directory

---

# Architecture

```
Windows Domain
        │
        ▼
Domain Controller
        │
        ▼
Active Directory Connector
        │
        ▼
Identity Synchronization
        │
        ▼
CDP Identity Module
```

---

# Active Directory Objects

Supported objects include:

- Users
- Groups
- Computers
- Organizational Units
- Domains
- Forests
- Service Accounts
- Contacts
- Printers
- Shared Resources

---

# Authentication

Supported authentication methods:

- Kerberos
- NTLM
- LDAP Bind
- LDAPS
- Certificate Authentication
- Windows Integrated Authentication

---

# Domain Management

Each domain includes:

- Domain Name
- Forest
- NetBIOS Name
- Functional Level
- Domain Controllers
- Sites
- Trust Relationships
- DNS Configuration

---

# Organizational Units

The platform synchronizes:

- Departments
- Divisions
- Plants
- Warehouses
- Regional Offices
- Manufacturing Units
- Administrative Offices

---

# Group Types

Supported groups:

- Security Groups
- Distribution Groups
- Global Groups
- Universal Groups
- Domain Local Groups

---

# Synchronization

Synchronization supports:

- Initial Import
- Incremental Import
- Full Synchronization
- Scheduled Jobs
- Real-Time Detection

---

# Password Policies

Imported policies include:

- Password Complexity
- Password Length
- Expiration Policy
- Password History
- Lockout Threshold

---

# Account Status

Supported states:

- Active
- Disabled
- Locked
- Expired
- Password Expired
- Pending Activation

---

# Security

The component shall:

- Use LDAPS
- Support Kerberos encryption
- Validate domain certificates
- Protect service accounts
- Audit all authentication events
- Monitor failed logins

---

# Permissions

Administrators may:

- Register domains
- Configure synchronization
- Test connections
- View synchronization logs

Identity Operators may:

- Execute synchronization

Auditors may:

- View logs

---

# API Endpoints

GET /api/v1/ad/domains

POST /api/v1/ad/domains

PUT /api/v1/ad/domains/{id}

DELETE /api/v1/ad/domains/{id}

POST /api/v1/ad/test

POST /api/v1/ad/sync

GET /api/v1/ad/logs

GET /api/v1/ad/groups

GET /api/v1/ad/users

---

# Events

DomainRegistered

DomainUpdated

SynchronizationStarted

SynchronizationCompleted

SynchronizationFailed

UserImported

GroupImported

OUImported

ComputerImported

AuthenticationSucceeded

AuthenticationFailed

---

# Database Tables

ADDomains

ADForests

ADSites

ADSyncJobs

ADGroups

ADUsers

ADConnections

ADLogs

---

# Monitoring

Metrics include:

- Connected Domains
- Connected Controllers
- Imported Users
- Imported Groups
- Synchronization Duration
- Failed Logins
- Domain Availability

---

# Best Practices

- Use LDAPS
- Use dedicated service accounts
- Enable incremental synchronization
- Minimize imported attributes
- Synchronize only required Organizational Units
- Rotate service account passwords
- Monitor replication health

---

# Future Enhancements

- Microsoft Entra ID synchronization
- Hybrid identity
- Azure AD Connect integration
- Conditional Access synchronization
- Windows Hello support
- Passwordless authentication
- AI-powered identity health monitoring
