# Permissions

## Purpose

Permissions define exactly what actions a user can perform inside the Capanna Digital Platform.

---

## Permission Structure

Each permission belongs to:

- Module
- Resource
- Action

Example:

Production -> Work Orders -> Create

---

## Standard Actions

- View
- Create
- Update
- Delete
- Approve
- Reject
- Import
- Export
- Print
- Archive

---

## Permission Levels

### Read Only

User can only view information.

### Editor

User can create and update records.

### Manager

Can approve and reject operations.

### Administrator

Full control over the module.

---

## Permission Examples

| Module | Permission |
|---------|------------|
| Sales | sales.create |
| Sales | sales.update |
| Sales | sales.delete |
| Inventory | inventory.read |
| Inventory | inventory.export |
| Production | production.approve |
| HR | hr.manage |

---

## Best Practices

- Follow Least Privilege Principle.
- Never assign Administrator permissions unless necessary.
- Review permissions quarterly.
- Log all permission changes.
