# Maintenance Management

## Overview

The Maintenance module manages preventive, predictive, corrective, and emergency maintenance activities for all manufacturing equipment.

Its objective is to maximize machine availability, reduce downtime, improve Overall Equipment Effectiveness (OEE), and extend equipment life.

---

# Maintenance Types

## Preventive Maintenance

Scheduled maintenance performed before failures occur.

Examples:

- Daily inspection
- Weekly lubrication
- Monthly calibration
- Quarterly service
- Annual overhaul

---

## Corrective Maintenance

Repairs performed after a machine failure.

Examples:

- Motor replacement
- Bearing replacement
- PLC repair
- Sensor replacement
- Air leak repair

---

## Predictive Maintenance

Maintenance based on machine condition.

Monitoring:

- Vibration
- Temperature
- Current
- Air Pressure
- Spindle Hours
- Cycle Count

---

## Emergency Maintenance

Immediate repair required to restore production.

Examples:

- CNC breakdown
- Compressor failure
- Dust collector shutdown
- Electrical failure

---

# Machine Information

Each machine stores:

- Machine ID
- Machine Name
- Manufacturer
- Model
- Serial Number
- Installation Date
- Department
- Work Center
- Status

---

# Maintenance Schedule

For every maintenance task:

- Task ID
- Machine
- Maintenance Type
- Frequency
- Responsible Technician
- Estimated Duration
- Checklist
- Required Spare Parts

---

# Work Orders

Maintenance work orders include:

- Work Order Number
- Machine
- Problem Description
- Priority
- Technician
- Start Time
- Finish Time
- Downtime
- Root Cause
- Resolution

---

# Spare Parts

Inventory includes:

- Part Number
- Description
- Supplier
- Quantity
- Minimum Stock
- Cost

---

# Downtime Analysis

Downtime reasons include:

- Mechanical Failure
- Electrical Failure
- Pneumatic Failure
- Software Failure
- Operator Error
- Scheduled Maintenance
- Material Shortage

---

# KPIs

- MTBF (Mean Time Between Failures)
- MTTR (Mean Time To Repair)
- Machine Availability
- Downtime
- Maintenance Cost
- Planned Maintenance %
- Emergency Maintenance %
- Spare Parts Consumption

---

# Dashboards

Maintenance Dashboard displays:

- Machine Status
- Active Work Orders
- Upcoming Maintenance
- Downtime Today
- MTBF
- MTTR
- OEE Impact
- Technician Workload

---

# Integrations

- Machines
- Production Orders
- Work Orders
- Scheduling
- Shop Floor
- Inventory
- Purchasing
- KPI_OEE
