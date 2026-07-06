# Work Orders

## Overview

Work Orders represent executable manufacturing tasks derived from a Production Order. Each Work Order is assigned to a specific work center, machine, or operator and contains the detailed instructions required to complete one manufacturing operation.

A Production Order may generate multiple Work Orders based on the product routing.

---

## Objectives

- Execute production operations
- Control manufacturing activities
- Track shop floor progress
- Record labor and machine time
- Monitor operation status
- Ensure production traceability

---

## Work Order Structure

Each Work Order includes:

- Work Order Number
- Parent Production Order
- Product
- Operation
- Routing Step
- Work Center
- Machine
- Operator
- Planned Quantity
- Completed Quantity
- Scrap Quantity
- Due Date
- Priority
- Status

---

## Typical Operations

- Panel Cutting
- CNC Machining
- Edge Banding
- Drilling
- Sanding
- Assembly
- Painting
- Packaging

---

## Lifecycle

Created

↓

Released

↓

Assigned

↓

Started

↓

Paused

↓

Completed

↓

Verified

↓

Closed

---

## Execution Data

The system records:

- Start Time
- End Time
- Machine Runtime
- Operator Time
- Cycle Time
- Setup Time
- Downtime
- Rejects
- Rework
- Quality Checks

---

## Status

- Created
- Released
- Assigned
- Running
- Paused
- Waiting Material
- Waiting Quality
- Completed
- Closed
- Cancelled

---

## KPIs

- Work Order Completion Rate
- Average Cycle Time
- Operator Productivity
- Machine Utilization
- First Pass Yield
- Scrap Rate
- Schedule Compliance

---

## Integrations

- Production Orders
- Routings
- BOM
- Machines
- Operators
- Inventory
- Quality
- Maintenance
- Analytics
