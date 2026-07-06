# Production Orders

## Overview

The Production Orders component manages manufacturing orders from release through completion. It converts production plans into executable manufacturing activities while coordinating materials, labor, machines, and routing.

Production Orders serve as the primary execution document within the Manufacturing Execution System (MES).

---

## Objectives

- Control manufacturing execution
- Allocate materials
- Reserve machine capacity
- Track production progress
- Monitor production costs
- Manage production status
- Ensure manufacturing traceability

---

## Production Order Lifecycle

Draft

↓

Planned

↓

Released

↓

In Progress

↓

Quality Inspection

↓

Completed

↓

Closed

↓

Archived

---

## Information

Each Production Order contains:

- Production Order Number
- Product
- Variant
- Configuration
- Quantity
- Unit of Measure
- Customer
- Due Date
- Priority
- Routing
- BOM Revision
- Engineering Revision
- Production Status

---

## Material Allocation

The system automatically reserves:

- Panels
- Hardware
- Accessories
- Packaging
- Consumables

Material shortages automatically generate procurement recommendations.

---

## Machine Assignment

Production Orders may be assigned to:

- CNC Router
- Edge Banding
- Drilling
- Sanding
- Assembly
- Painting
- Packaging

Capacity validation occurs before release.

---

## Status

- Draft
- Planned
- Approved
- Released
- In Progress
- On Hold
- Waiting Material
- Waiting Inspection
- Completed
- Closed
- Cancelled

---

## KPIs

- Orders Released
- Orders Completed
- Orders Delayed
- Manufacturing Lead Time
- Production Efficiency
- Schedule Adherence
- Material Availability
- Completion Rate

---

## Integrations

- Products
- BOM
- Routings
- Work Orders
- Shop Floor
- Inventory
- Purchasing
- Warehouse
- Quality
- Maintenance
- Analytics
