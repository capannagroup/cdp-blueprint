# Production Workflow

## Overview

The Production Workflow defines the complete manufacturing execution process within the Capanna Digital Platform (CDP), beginning with a customer order and ending with finished goods being transferred to inventory.

This document serves as the master process map for all Production module components.

---

# Workflow Overview

```text
Customer Order
      │
      ▼
Sales Order
      │
      ▼
Production Planning
      │
      ▼
Material Availability Check
      │
      ▼
Production Scheduling
      │
      ▼
Production Order
      │
      ▼
Work Orders
      │
      ▼
Machine Assignment
      │
      ▼
Operator Assignment
      │
      ▼
Material Issue
      │
      ▼
Machine Setup
      │
      ▼
Production Execution
      │
      ▼
Shop Floor Monitoring
      │
      ▼
Quality Inspection
      │
      ▼
Production Tracking
      │
      ▼
Traceability Recording
      │
      ▼
Finished Goods
      │
      ▼
Warehouse Transfer
      │
      ▼
Production Reports
      │
      ▼
Production Dashboard
```

---

# Stage 1 – Sales Order

Input:

- Customer Order
- Product Configuration
- Delivery Date

Output:

- Approved Sales Order

---

# Stage 2 – Production Planning

Responsible:

Production Planner

Activities:

- Capacity Planning
- Material Planning
- Resource Planning
- Delivery Planning

Output:

- Production Plan

---

# Stage 3 – Material Verification

Checks:

- Raw Material Availability
- Hardware
- Accessories
- Glue
- Packaging

If materials are unavailable:

→ Purchasing Request

---

# Stage 4 – Scheduling

Activities:

- Machine Scheduling
- Operator Scheduling
- Shift Planning
- Priority Sequencing

Output:

- Production Schedule

---

# Stage 5 – Production Order

Creates the master manufacturing document.

Contains:

- Product
- Quantity
- Due Date
- Routing
- BOM
- Priority

Generates:

- Work Orders

---

# Stage 6 – Work Orders

Each routing operation becomes one Work Order.

Example:

Production Order

↓

WO-001 Cutting

↓

WO-002 CNC

↓

WO-003 Edge Banding

↓

WO-004 Drilling

↓

WO-005 Assembly

↓

WO-006 Sanding

↓

WO-007 Painting

↓

WO-008 Packing

---

# Stage 7 – Machine Assignment

Assigns each Work Order to:

- Machine
- Work Center
- Production Line

---

# Stage 8 – Operator Assignment

Assigns:

- Operator
- Team Leader
- Shift

---

# Stage 9 – Material Issue

Inventory issues:

- MDF
- Plywood
- Hardware
- Glue
- Edge Banding
- Packaging

Inventory is updated automatically.

---

# Stage 10 – Machine Setup

Activities:

- Load CNC Program
- Tool Verification
- Material Verification
- Safety Check
- Setup Approval

---

# Stage 11 – Production Execution

Machine status:

- Running
- Idle
- Setup
- Maintenance
- Alarm
- Completed

Captured automatically:

- Cycle Time
- Production Count
- Scrap
- Downtime

---

# Stage 12 – Shop Floor Monitoring

Real-time monitoring includes:

- Machine Status
- Operator Status
- Work Order Progress
- OEE
- Alarms
- Downtime

---

# Stage 13 – Quality Control

Inspection Types:

- Incoming
- First Piece
- In Process
- Final Inspection

Possible Results:

- Pass
- Rework
- Reject

---

# Stage 14 – Production Tracking

Records:

- Quantity Produced
- Scrap
- Time
- Operator
- Machine
- Shift

---

# Stage 15 – Traceability

Records:

- Material Batch
- Machine
- Tool
- Operator
- Shift
- Production Order
- Work Order
- Inspection Results

---

# Stage 16 – Finished Goods

Completed products are transferred to Finished Goods Inventory.

Inventory Status:

- Available
- Reserved
- Ready for Shipment

---

# Stage 17 – Reporting

Reports Generated:

- Production Report
- OEE Report
- Downtime Report
- Machine Report
- Operator Report
- Scrap Report
- Quality Report

---

# Stage 18 – Dashboards

Management dashboards display:

- Live Production
- Machine Status
- OEE
- Downtime
- Production Progress
- Schedule Adherence
- Quality Performance
- Labor Efficiency

---

# Integrated Modules

This workflow integrates with:

- Products
- Engineering
- Inventory
- Warehouse
- Purchasing
- Sales
- Quality
- Maintenance
- Dashboards
- Reports
- Traceability
- KPI/OEE
- Andon
- Alarms

---

# Success Metrics

Production workflow performance is measured using:

- OEE
- Production Output
- First Pass Yield
- Downtime
- Machine Utilization
- Labor Productivity
- Schedule Adherence
- On-Time Delivery
- Scrap Rate
- Cycle Time

---

# End-to-End Process Summary

Customer Order
→ Sales
→ Planning
→ Scheduling
→ Production Order
→ Work Orders
→ Machines
→ Operators
→ Material Issue
→ Production
→ Quality
→ Traceability
→ Finished Goods
→ Warehouse
→ Reports
→ Dashboard
