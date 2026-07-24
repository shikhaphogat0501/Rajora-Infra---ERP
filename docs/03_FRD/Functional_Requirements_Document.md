# Functional Requirements Document (FRD)

> **Project:** Rajora ERP – Enterprise Residential Construction Management System  
> **Company:** Rajora Infra Homes  
> **Document ID:** FRD-001  
> **Version:** 1.0  
> **Prepared By:** Shikha Phogat – Business Analyst  
> **Prepared For:** Rajora Infra Homes Management  
> **Date:** July 2026  
> **Document Status:** Final

---

# Document Overview

This Functional Requirements Document (FRD) describes how the Rajora ERP system will fulfill the business requirements defined in the Business Requirements Document (BRD).

The document translates business needs into functional system behavior by defining user interactions, workflows, validations, business rules, and expected outputs for each ERP module.

The FRD serves as the primary reference for developers, testers, and business users during solution development, system testing, and User Acceptance Testing (UAT).

---

# Version History

| Version | Date | Author | Description |
|----------|------|--------|-------------|
| 0.1 | July 2026 | Shikha Phogat | Initial Draft |
| 1.0 | July 2026 | Shikha Phogat | Final Version |

---

# Table of Contents

- [1. Purpose](#1-purpose)
- [2. Functional Scope](#2-functional-scope)
- [3. System Users](#3-system-users)
- [4. General Functional Requirements](#4-general-functional-requirements)
- [5. CRM Module](#5-crm-module)
- [6. Sales Module](#6-sales-module)
- [7. Finance Module](#7-finance-module)
- [8. Construction Module](#8-construction-module)
- [9. Labour Module](#9-labour-module)
- [10. Procurement Module](#10-procurement-module)
- [11. Inventory Module](#11-inventory-module)
- [12. Dashboard & Reporting](#12-dashboard--reporting)
- [13. Administration & Security](#13-administration--security)
- [14. Error Handling & Validations](#14-error-handling--validations)
- [15. Assumptions & Constraints](#15-assumptions--constraints)
- [16. Acceptance Criteria](#16-acceptance-criteria)
- [17. Document Approval](#17-document-approval)

---

# 1. Purpose

The purpose of this Functional Requirements Document is to define how the Rajora ERP system will function to meet the approved business requirements.

The document provides detailed functional specifications for each ERP module, ensuring that developers, testers, and business stakeholders share a common understanding of the expected system behavior.

This document complements the Business Requirements Document (BRD) by focusing on **how the system will operate**, rather than **what the business requires**.

---

## Objectives

- Define the functional behavior of each ERP module.
- Describe user interactions with the system.
- Document validations and business rules.
- Define expected system outputs.
- Provide a reference for development and testing.

> **Business Analyst Note**
>
> The FRD focuses on system functionality and user interactions. Technical implementation details such as database design, application architecture, and source code are documented separately.

---

# 2. Functional Scope

The Rajora ERP system will include the following functional modules.

| Module | Primary Function |
|----------|-----------------|
| CRM | Lead and customer management |
| Sales | Booking and agreement management |
| Finance | Payments, collections and financial records |
| Construction | Project and milestone tracking |
| Labour | Attendance and wage management |
| Procurement | Purchase Requests and Purchase Orders |
| Inventory | Material receipt, issue and stock management |
| Dashboard & MIS | Business reporting and KPI dashboards |
| Administration | User management and system security |

---

# 3. System Users

The following users will interact with the ERP system.

| User Role | Primary Responsibility |
|------------|------------------------|
| Managing Director | View executive dashboards and approve major transactions |
| CEO | Monitor business performance |
| Sales Executive | Manage leads, bookings and customers |
| Finance Manager | Record payments and manage financial records |
| Project Manager | Monitor construction activities |
| Site Engineer | Update daily project progress |
| Procurement Manager | Manage purchasing activities |
| Store Manager | Manage inventory transactions |
| HR Executive | Record labour attendance |
| System Administrator | Manage users, permissions and system configuration |

---

# 4. General Functional Requirements

The ERP system shall provide the following common functionality across all modules.

| ID | Functional Requirement |
|----|------------------------|
| FR-001 | Secure user login. |
| FR-002 | Role-based access control. |
| FR-003 | Create, edit and delete records based on user permissions. |
| FR-004 | Search and filter records. |
| FR-005 | Export reports to Excel and PDF. |
| FR-006 | Maintain audit logs for critical transactions. |
| FR-007 | Record date and time of business transactions. |
| FR-008 | Display dashboards based on user roles. |

---

# 5. CRM Module

## Module Purpose

The CRM module manages customer enquiries, lead tracking, follow-ups and customer records throughout the sales lifecycle.

---

## Functional Features

| ID | Function |
|----|----------|
| CRM-FR-001 | Create Lead |
| CRM-FR-002 | Assign Lead |
| CRM-FR-003 | Update Lead Status |
| CRM-FR-004 | Record Customer Follow-up |
| CRM-FR-005 | Maintain Customer Master |
| CRM-FR-006 | Upload Customer Documents |
| CRM-FR-007 | Record Customer Complaints |
| CRM-FR-008 | CRM Dashboard |

---

### Lead Creation

**Description**

The system shall allow sales executives to create new customer leads.

**Input Fields**

- Customer Name
- Mobile Number
- Email
- Project
- Lead Source
- Budget
- Assigned Executive

**Validation Rules**

- Customer Name is mandatory.
- Mobile Number is mandatory.
- Duplicate mobile numbers shall not be allowed.
- Lead Source must be selected.

**Output**

- Lead ID generated automatically.
- Lead status set to **New**.

---

### Lead Assignment

The system shall allow managers to assign leads to sales executives.

**Business Rules**

- One lead can be assigned to only one executive.
- Assignment history shall be maintained.
- Reassignment shall be logged.

---

### Customer Follow-up

The system shall allow users to record customer interactions.

Information recorded includes:

- Follow-up Date
- Discussion Summary
- Next Follow-up Date
- Lead Status

---

### CRM Dashboard

The dashboard shall display:

- Total Leads
- New Leads
- Follow-ups Due
- Converted Customers
- Lost Leads
- Lead Conversion Rate

> **Business Analyst Observation**
>
> The CRM module is designed to centralize customer information, reduce duplicate records, and ensure timely follow-ups through a structured lead management process.

---

# 6. Sales Module

## Module Purpose

The Sales module manages unit availability, bookings, agreements, cancellations and installment planning.

---

## Functional Features

| ID | Function |
|----|----------|
| SALES-FR-001 | Unit Availability |
| SALES-FR-002 | Booking Management |
| SALES-FR-003 | Booking Approval |
| SALES-FR-004 | Agreement Generation |
| SALES-FR-005 | Installment Planning |
| SALES-FR-006 | Booking Cancellation |
| SALES-FR-007 | Sales Dashboard |

---

### Unit Availability

The system shall display available, booked and reserved units in real time.

**Validation**

- Booked units shall not be available for new bookings.

---

### Booking Management

The system shall allow authorized users to create customer bookings.

**Mandatory Fields**

- Customer
- Project
- Unit Number
- Booking Date
- Booking Amount

**System Output**

- Booking ID generated.
- Unit status updated to **Booked**.

---

### Agreement Generation

The system shall generate customer agreements using predefined templates after booking approval.

---

### Sales Dashboard

The dashboard shall display:

- Total Bookings
- Booking Value
- Sales by Project
- Sales by Executive
- Pending Agreements
- Monthly Sales Trend

---

# 7. Finance Module

## Module Purpose

The Finance module manages customer payments, receipts, outstanding balances, and financial records related to property bookings.

---

## Functional Features

| ID | Function |
|----|----------|
| FIN-FR-001 | Record Customer Payments |
| FIN-FR-002 | Generate Payment Receipts |
| FIN-FR-003 | Maintain Customer Ledger |
| FIN-FR-004 | Track Outstanding Payments |
| FIN-FR-005 | GST Calculation |
| FIN-FR-006 | Finance Dashboard |

---

### Customer Payment

The system shall allow finance users to record payments received from customers.

**Mandatory Fields**

- Customer Name
- Booking ID
- Payment Date
- Payment Amount
- Payment Mode

**Validation Rules**

- Booking ID must exist.
- Payment amount cannot exceed the outstanding balance.
- Payment date cannot be a future date.

**System Output**

- Receipt generated automatically.
- Customer ledger updated.
- Outstanding balance recalculated.

---

### Customer Ledger

The system shall maintain complete payment history for every customer.

The ledger shall display:

- Booking Amount
- Total Payments Received
- Outstanding Balance
- Payment History

---

### Finance Dashboard

The dashboard shall display:

- Total Collections
- Outstanding Amount
- Monthly Collections
- Payment Status
- Collection Trend

> **Business Analyst Observation**
>
> The Finance module provides a centralized view of customer collections while reducing manual calculation of outstanding balances.

---

# 8. Construction Module

## Module Purpose

The Construction module enables monitoring of project progress, milestones, and daily site activities.

---

## Functional Features

| ID | Function |
|----|----------|
| CON-FR-001 | Project Master |
| CON-FR-002 | Milestone Tracking |
| CON-FR-003 | Daily Progress Update |
| CON-FR-004 | Delay Monitoring |
| CON-FR-005 | Construction Dashboard |

---

### Project Master

The system shall maintain project information including:

- Project Name
- Location
- Start Date
- Expected Completion Date
- Current Status

---

### Milestone Tracking

The system shall allow project managers to update milestone completion status.

Example milestones include:

- Foundation
- Structure
- Brickwork
- Plumbing
- Electrical
- Finishing
- Handover

---

### Daily Progress

Site engineers shall record daily progress.

**Input**

- Project
- Date
- Work Completed
- Remarks
- Percentage Completed

---

### Construction Dashboard

The dashboard shall display:

- Active Projects
- Completed Projects
- Delayed Projects
- Overall Progress
- Upcoming Milestones

> **Business Analyst Observation**
>
> This module improves project visibility and enables management to monitor construction progress across all ongoing projects.

---

# 9. Labour Module

## Module Purpose

The Labour module manages labour records, attendance, and wage calculations.

---

## Functional Features

| ID | Function |
|----|----------|
| LAB-FR-001 | Labour Registration |
| LAB-FR-002 | Attendance Management |
| LAB-FR-003 | Wage Calculation |
| LAB-FR-004 | Labour Dashboard |

---

### Labour Registration

The system shall maintain labour details including:

- Labour ID
- Name
- Trade
- Daily Wage
- Contact Number

---

### Attendance Management

Attendance shall be recorded daily.

**Validation Rules**

- Attendance cannot be marked for future dates.
- Labour ID must exist.

---

### Wage Calculation

The system shall calculate wages based on:

- Attendance
- Daily Wage Rate

---

### Labour Dashboard

The dashboard shall display:

- Total Labour
- Present Labour
- Absent Labour
- Total Wages
- Attendance Percentage

---

# 10. Procurement Module

## Module Purpose

The Procurement module manages vendor information, purchase requests, and purchase orders.

---

## Functional Features

| ID | Function |
|----|----------|
| PROC-FR-001 | Vendor Management |
| PROC-FR-002 | Purchase Request |
| PROC-FR-003 | Purchase Order |
| PROC-FR-004 | Approval Workflow |
| PROC-FR-005 | Procurement Dashboard |

---

### Vendor Management

The system shall maintain vendor details including:

- Vendor Name
- Contact Information
- Material Category
- GST Number

---

### Purchase Request

Authorized users shall create Purchase Requests for required materials.

**Mandatory Fields**

- Material
- Quantity
- Required Date
- Requestor

---

### Purchase Order

Approved Purchase Requests shall generate Purchase Orders.

Each Purchase Order shall include:

- Vendor
- Material Details
- Quantity
- Rate
- Expected Delivery Date

---

### Procurement Dashboard

The dashboard shall display:

- Pending Purchase Requests
- Approved Purchase Orders
- Vendor Performance
- Material Procurement Status

---

# 11. Inventory Module

## Module Purpose

The Inventory module manages material receipts, issues, and stock availability.

---

## Functional Features

| ID | Function |
|----|----------|
| INV-FR-001 | Material Master |
| INV-FR-002 | Material Receipt |
| INV-FR-003 | Material Issue |
| INV-FR-004 | Stock Monitoring |
| INV-FR-005 | Inventory Dashboard |

---

### Material Receipt

The system shall record all incoming materials.

**Input**

- Material Name
- Vendor
- Quantity
- Receipt Date

---

### Material Issue

Materials shall be issued against approved project requirements.

**Validation**

- Quantity issued cannot exceed available stock.

---

### Stock Monitoring

The system shall automatically update stock balances after every receipt or issue transaction.

Low-stock items shall be highlighted for procurement.

---

### Inventory Dashboard

The dashboard shall display:

- Current Stock
- Low Stock Items
- Material Consumption
- Recent Material Receipts
- Material Issues

---

# 12. Dashboard & Reporting

## Module Purpose

The Dashboard & Reporting module provides management with real-time business insights through interactive reports and KPIs.

---

## Functional Features

| ID | Function |
|----|----------|
| RPT-FR-001 | Executive Dashboard |
| RPT-FR-002 | Sales Dashboard |
| RPT-FR-003 | Finance Dashboard |
| RPT-FR-004 | Construction Dashboard |
| RPT-FR-005 | Labour Dashboard |
| RPT-FR-006 | Procurement Dashboard |
| RPT-FR-007 | Inventory Dashboard |
| RPT-FR-008 | Export Reports |

---

### Dashboard Features

All dashboards shall support:

- Search
- Filters
- Date Selection
- Excel Export
- PDF Export

---

### Standard Reports

The ERP shall generate:

- Daily Sales Report
- Customer Outstanding Report
- Labour Attendance Report
- Project Progress Report
- Procurement Status Report
- Inventory Stock Report

> **Business Analyst Observation**
>
> Dashboards and MIS reports provide management with timely, accurate information for operational monitoring and business decision-making.

---

# 13. Administration & Security

## Module Purpose

The Administration module enables system administrators to manage users, roles, permissions, and basic system settings while ensuring secure access to the ERP application.

---

## Functional Features

| ID | Function |
|----|----------|
| ADM-FR-001 | User Management |
| ADM-FR-002 | Role-Based Access Control |
| ADM-FR-003 | Password Management |
| ADM-FR-004 | Audit Log |
| ADM-FR-005 | User Activity Monitoring |

---

### User Management

The system shall allow the administrator to:

- Create new users.
- Edit user information.
- Activate or deactivate user accounts.
- Reset user passwords.

---

### Role-Based Access Control (RBAC)

The system shall provide predefined roles such as:

| Role | Access |
|------|--------|
| Managing Director | View all dashboards and reports |
| CEO | Executive dashboards and reports |
| Sales Executive | CRM and Sales modules |
| Finance Manager | Finance module |
| Project Manager | Construction module |
| Procurement Manager | Procurement module |
| Store Manager | Inventory module |
| HR Executive | Labour module |
| System Administrator | Full system access |

---

### Audit Log

The system shall maintain audit records for important business transactions including:

- Login history
- Record creation
- Record modification
- Record deletion
- User account changes

---

# 14. Error Handling & Validations

The ERP system shall display meaningful validation messages to users whenever invalid data is entered.

| Scenario | Validation Message |
|----------|--------------------|
| Duplicate Customer | Customer already exists. |
| Duplicate Booking | Selected unit has already been booked. |
| Invalid Login | Invalid username or password. |
| Missing Mandatory Field | Please complete all mandatory fields. |
| Invalid Payment | Payment amount exceeds outstanding balance. |
| Stock Shortage | Insufficient stock available. |
| Future Attendance | Attendance cannot be recorded for future dates. |

---

# 15. Assumptions

The following assumptions have been considered while preparing this Functional Requirements Document.

- Users have basic computer knowledge.
- All departments will use the ERP system for daily operations.
- Master data will be available before implementation.
- Business users will participate in User Acceptance Testing (UAT).
- Required infrastructure will be available before Go-Live.

---

# 16. Constraints

The implementation is subject to the following constraints.

| Constraint | Description |
|------------|-------------|
| Budget | Implementation shall remain within the approved project budget. |
| Timeline | Phase 1 shall be completed within the planned schedule. |
| Resources | Business users will continue operational work during implementation. |
| Infrastructure | Existing IT infrastructure will be utilized where possible. |

---

# 17. Acceptance Criteria

The ERP solution shall be considered acceptable when the following conditions are met.

| Module | Acceptance Criteria |
|---------|---------------------|
| CRM | Users can successfully create and manage customer leads. |
| Sales | Bookings and agreements are generated successfully. |
| Finance | Payments and receipts are recorded accurately. |
| Construction | Project progress can be updated and monitored. |
| Labour | Attendance and wage calculations function correctly. |
| Procurement | Purchase Requests and Purchase Orders follow the approval workflow. |
| Inventory | Material receipts and issues update stock correctly. |
| Dashboards | KPI dashboards display accurate business information. |
| Security | Users can access only authorized modules. |

> **Business Analyst Observation**
>
> Successful User Acceptance Testing (UAT) confirms that the implemented ERP solution satisfies the approved business and functional requirements documented in the BRD and FRD.

---

# 18. Requirement Traceability

The following table illustrates how business requirements are translated into functional requirements.

| Business Requirement | Functional Requirement |
|----------------------|------------------------|
| Lead Management | CRM Module |
| Customer Booking | Sales Module |
| Payment Management | Finance Module |
| Project Monitoring | Construction Module |
| Labour Attendance | Labour Module |
| Procurement Process | Procurement Module |
| Inventory Tracking | Inventory Module |
| MIS Reporting | Dashboard & Reporting Module |
| User Access Control | Administration Module |

> **Business Analyst Note**
>
> Detailed testing and User Acceptance Testing (UAT) documents will validate each functional requirement during the testing phase.

---

# 19. Document Approval

The following stakeholders approve this Functional Requirements Document.

| Role | Name | Status |
|------|------|--------|
| Managing Director | Vishutosh Singh | Pending |
| Business Analyst | Shikha Phogat | Approved |

---

# Conclusion

The Functional Requirements Document defines how the Rajora ERP system will operate to meet the business requirements identified during the Business Discovery and Business Requirements Analysis phases.

It provides a clear description of the expected functionality for each ERP module, establishes system behavior, documents validation rules, and serves as the primary reference for development, testing, and User Acceptance Testing (UAT).

Together with the Business Requirements Document (BRD), this document forms the foundation for the successful implementation of the Rajora ERP – Enterprise Residential Construction Management System.

---

## Related Documents

| Document | Purpose |
|----------|---------|
| Business Discovery | Understand business processes and objectives |
| Business Requirements Document (BRD) | Define business needs and scope |
| Functional Requirements Document (FRD) | Define system functionality |
| User Stories | Describe functional requirements from the user's perspective |
| Process Models | Visualize business workflows |
| Database Design | Define database structure |
| Testing & UAT | Validate system functionality |
| Power BI Dashboards | Provide business insights and reporting |

---

**Document Status:** Final

**Version:** 1.0

**Prepared By:** Shikha Phogat – Business Analyst

**Project:** Rajora ERP – Enterprise Residential Construction Management System

---
