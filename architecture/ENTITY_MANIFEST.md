# Entity Manifest

## Purpose

The Entity Manifest is the master registry of all business entities used throughout the Capanna Digital Platform (CDP).

Each entity must have:

- Business Owner
- Primary Module
- Database Table
- API
- Relationships
- Version

---

# Entity Registry

| Entity | Module | Owner | Status |
|---------|---------|--------|----------|
| User | Identity | Platform | Approved |
| Role | Identity | Platform | Approved |
| Permission | Identity | Platform | Approved |
| Product | Products | Engineering | Approved |
| Product Variant | Products | Engineering | Approved |
| Material | Products | Engineering | Approved |
| BOM | Engineering | Engineering | Approved |
| BOM Item | Engineering | Engineering | Approved |
| Routing | Engineering | Engineering | Approved |
| Routing Operation | Engineering | Engineering | Approved |
| Production Order | Production | Production | Approved |
| Work Order | Production | Production | Approved |
| Machine | Production | Maintenance | Approved |
| Work Center | Production | Production | Approved |
| Operator | Production | HR | Approved |
| Shift | Production | HR | Approved |
| Quality Inspection | Quality | Quality | Approved |
| NCR | Quality | Quality | Planned |
| Maintenance Order | Maintenance | Maintenance | Planned |
| Inventory Item | Inventory | Warehouse | Planned |
| Warehouse | Inventory | Warehouse | Planned |
| Purchase Order | Purchasing | Purchasing | Planned |
| Supplier | Purchasing | Purchasing | Planned |
| Customer | Sales | Sales | Planned |
| Sales Order | Sales | Sales | Planned |

---

# Entity Rules

Every entity shall define:

- Primary Key
- Business Identifier
- Status
- Audit Fields
- Relationships
- Events

---

# Standard Audit Fields

Every entity shall contain:

- Created By
- Created Date
- Modified By
- Modified Date
- Version
- Active
