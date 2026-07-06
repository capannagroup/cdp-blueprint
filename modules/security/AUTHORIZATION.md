# Authorization

## Purpose

Authorization determines what an authenticated user is allowed to access and perform within the Capanna Digital Platform.

---

## Authorization Model

The platform implements Role-Based Access Control (RBAC) with policy-based authorization.

---

## Roles

- System Administrator
- Factory Manager
- Production Manager
- Sales Manager
- Purchasing Manager
- Warehouse Manager
- Finance Manager
- HR Manager
- Customer
- Supplier

---

## Permission Categories

- Read
- Create
- Update
- Delete
- Approve
- Export
- Configure
- Manage Users

---

## Authorization Flow

1. User is authenticated.
2. JWT Token is validated.
3. User role is identified.
4. Permissions are loaded.
5. Access policy is evaluated.
6. Resource access is granted or denied.

---

## Security Principles

- Least Privilege
- Separation of Duties
- Policy-Based Authorization
- Centralized Permission Management
- Audit Logging

---

## Future Enhancements

- Attribute-Based Access Control (ABAC)
- Dynamic Policies
- Tenant-Level Permissions
