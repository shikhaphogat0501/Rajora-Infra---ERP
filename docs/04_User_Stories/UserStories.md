# Functional Requirements Document (FRD)

## Overview

This folder contains the **Functional Requirements Document (FRD)** for the **Rajora ERP – Enterprise Residential Construction Management System** project.

The FRD translates the approved business requirements into detailed functional specifications by defining how the ERP system should behave, how users interact with each module, and how business processes are executed within the application.

It serves as the primary reference for developers, testers, and business stakeholders during system development, testing, and User Acceptance Testing (UAT).

---

# Project Information

| Item | Details |
|------|---------|
| **Project** | Rajora ERP – Enterprise Residential Construction Management System |
| **Organization** | Rajora Infra Homes |
| **Phase** | Functional Analysis & Solution Design |
| **Document** | Functional Requirements Document (FRD) |
| **Document ID** | FRD-001 |
| **Version** | 1.0 |
| **Prepared By** | Shikha Phogat |
| **Role** | Business Analyst |
| **Status** | Final |

---

# Objectives

The Functional Requirements Document aims to:

- Define how each ERP module will function.
- Translate approved business requirements into system behavior.
- Document user interactions and workflows.
- Define business rules and validation logic.
- Support development, testing, and User Acceptance Testing (UAT).
- Ensure all stakeholders have a common understanding of the expected system functionality.

---

# Document Highlights

The FRD includes:

- Functional Scope
- System Users
- General Functional Requirements
- CRM Module Specifications
- Sales Module Specifications
- Finance Module Specifications
- Construction Module Specifications
- Labour Management Specifications
- Procurement Module Specifications
- Inventory Management Specifications
- Dashboard & Reporting Requirements
- Administration & Security
- Error Handling & Validations
- Assumptions & Constraints
- Acceptance Criteria
- Requirement Traceability
- Document Approval

---

# ERP Modules Covered

The Functional Requirements Document defines system functionality for the following modules:

- CRM
- Sales
- Finance
- Construction
- Labour Management
- Procurement
- Inventory Management
- Dashboard & MIS Reporting
- Administration & Security

---

# Repository Structure

```text
03_FRD/
│
├── README.md
└── Functional_Requirements_Document.md
```

---

# Document Flow

The Functional Requirements Document builds upon the Business Requirements Document and serves as the foundation for solution development.

```text
Business Discovery
        │
        ▼
Business Requirements Document (BRD)
        │
        ▼
Functional Requirements Document (FRD)
        │
        ▼
User Stories
        │
        ▼
Wireframes
        │
        ▼
Database Design
        │
        ▼
SQL Development
        │
        ▼
System Testing
        │
        ▼
User Acceptance Testing (UAT)
        │
        ▼
Power BI Dashboards
```

---

# Related Repository Documents

| Folder | Purpose |
|--------|---------|
| **01_Business_Discovery** | Business Discovery, Requirement Elicitation, Stakeholder Analysis, AS-IS & TO-BE Process Analysis |
| **02_BRD** | Business Requirements Document |
| **03_FRD** | Functional Requirements Document |
| **04_User_Stories** | Agile User Stories & Acceptance Criteria |
| **05_Process_Models** | Business Process Models & Workflow Diagrams |
| **06_Wireframes** | Screen Mockups & UI Designs |
| **07_Database** | ER Diagram & Database Design |
| **08_SQL** | SQL Scripts & Database Objects |
| **09_Testing** | Test Cases & User Acceptance Testing |
| **10_Dashboards** | Power BI Dashboards & KPI Reports |

---

# Key Deliverables

The FRD documents the following functional deliverables:

- Functional Scope
- Module-wise Functional Requirements
- User Workflows
- Input & Output Specifications
- Business Rules
- Validation Rules
- Dashboard Requirements
- Error Handling
- Security Requirements
- Acceptance Criteria
- Requirement Traceability

---

# Business Value

The Functional Requirements Document provides a clear blueprint for how the Rajora ERP system will operate by converting business needs into detailed functional specifications.

It establishes a common understanding between business stakeholders, developers, and testers, ensuring that every approved business requirement is implemented consistently and validated during testing before deployment.

---

# Author

**Shikha Phogat**  
**Role:** Business Analyst

---

# License

This repository has been created for **educational and portfolio purposes** to demonstrate end-to-end Business Analysis documentation for an ERP implementation project.

The project represents a realistic ERP implementation case study for a small-to-medium construction company and showcases requirement analysis, functional specification, solution documentation, and Software Development Life Cycle (SDLC) deliverables. It does not contain confidential or proprietary client information.

---

# 6. Finance Module

## Epic: Financial Management

---

### User Story: US-013

| Field | Details |
|------|---------|
| Story ID | US-013 |
| Module | Finance |
| Title | Record Customer Payment |
| Priority | High |

**User Story**

As a **Finance Manager**, I want to record customer payments so that financial transactions are accurately maintained.

**Acceptance Criteria**

- Booking ID must exist.
- Payment amount is mandatory.
- Payment date cannot be a future date.
- Receipt is generated automatically.

---

### User Story: US-014

| Field | Details |
|------|---------|
| Story ID | US-014 |
| Module | Finance |
| Title | Generate Payment Receipt |
| Priority | High |

**User Story**

As a **Finance Executive**, I want to generate payment receipts so that customers receive proof of payment.

**Acceptance Criteria**

- Receipt Number is generated automatically.
- Receipt includes customer and booking details.
- Receipt can be downloaded as PDF.

---

### User Story: US-015

| Field | Details |
|------|---------|
| Story ID | US-015 |
| Module | Finance |
| Title | View Customer Ledger |
| Priority | High |

**User Story**

As a **Finance Manager**, I want to view customer payment history so that I can monitor outstanding balances.

**Acceptance Criteria**

- Complete payment history is displayed.
- Outstanding balance is calculated automatically.
- Ledger can be exported.

---

### User Story: US-016

| Field | Details |
|------|---------|
| Story ID | US-016 |
| Module | Finance |
| Title | Track Outstanding Payments |
| Priority | High |

**User Story**

As a **Finance Manager**, I want to monitor outstanding customer payments so that collections can be planned.

**Acceptance Criteria**

- Outstanding balance is updated automatically.
- Customers with pending payments are highlighted.
- Outstanding report is available for export.

---

### User Story: US-017

| Field | Details |
|------|---------|
| Story ID | US-017 |
| Module | Finance |
| Title | View Finance Dashboard |
| Priority | Medium |

**User Story**

As a **Finance Manager**, I want to view financial dashboards so that I can monitor collections and pending payments.

**Acceptance Criteria**

- Dashboard displays total collections.
- Dashboard displays outstanding amount.
- Monthly collection trend is available.

---

# 7. Construction Module

## Epic: Construction Management

---

### User Story: US-018

| Field | Details |
|------|---------|
| Story ID | US-018 |
| Module | Construction |
| Title | Create Project |
| Priority | High |

**User Story**

As a **Project Manager**, I want to create construction projects so that project information is centrally managed.

**Acceptance Criteria**

- Project Name is mandatory.
- Start Date is mandatory.
- Project ID is generated automatically.

---

### User Story: US-019

| Field | Details |
|------|---------|
| Story ID | US-019 |
| Module | Construction |
| Title | Update Project Progress |
| Priority | High |

**User Story**

As a **Site Engineer**, I want to update daily project progress so that management can monitor construction activities.

**Acceptance Criteria**

- Project selection is mandatory.
- Progress percentage is recorded.
- Update date is automatically stored.

---

### User Story: US-020

| Field | Details |
|------|---------|
| Story ID | US-020 |
| Module | Construction |
| Title | Track Project Milestones |
| Priority | High |

**User Story**

As a **Project Manager**, I want to monitor milestone completion so that project timelines are maintained.

**Acceptance Criteria**

- Milestones can be updated.
- Completed milestones are highlighted.
- Delay status is visible.

---

### User Story: US-021

| Field | Details |
|------|---------|
| Story ID | US-021 |
| Module | Construction |
| Title | View Construction Dashboard |
| Priority | Medium |

**User Story**

As a **Project Manager**, I want to view project dashboards so that construction performance is monitored.

**Acceptance Criteria**

- Dashboard displays active projects.
- Dashboard displays delayed projects.
- Dashboard displays overall completion percentage.

---

# 8. Labour Module

## Epic: Labour Management

---

### User Story: US-022

| Field | Details |
|------|---------|
| Story ID | US-022 |
| Module | Labour |
| Title | Register Labour |
| Priority | High |

**User Story**

As an **HR Executive**, I want to register labour records so that workforce information is maintained.

**Acceptance Criteria**

- Labour ID is generated automatically.
- Name and daily wage are mandatory.
- Duplicate records are not allowed.

---

### User Story: US-023

| Field | Details |
|------|---------|
| Story ID | US-023 |
| Module | Labour |
| Title | Record Attendance |
| Priority | High |

**User Story**

As an **HR Executive**, I want to record labour attendance so that wages can be calculated accurately.

**Acceptance Criteria**

- Attendance date cannot be a future date.
- Labour ID must exist.
- Attendance status is saved successfully.

---

### User Story: US-024

| Field | Details |
|------|---------|
| Story ID | US-024 |
| Module | Labour |
| Title | Calculate Wages |
| Priority | High |

**User Story**

As an **HR Executive**, I want the system to calculate labour wages automatically so that manual calculations are reduced.

**Acceptance Criteria**

- Wage calculation is based on attendance.
- Daily wage rate is considered.
- Total wages are displayed correctly.

---

### User Story: US-025

| Field | Details |
|------|---------|
| Story ID | US-025 |
| Module | Labour |
| Title | View Labour Dashboard |
| Priority | Medium |

**User Story**

As an **HR Executive**, I want to monitor labour statistics through dashboards so that workforce information is easily accessible.

**Acceptance Criteria**

- Dashboard displays total labour.
- Dashboard displays attendance percentage.
- Dashboard displays wage summary.

---

# 9. Procurement Module

## Epic: Procurement Management

---

### User Story: US-026

| Field | Details |
|------|---------|
| Story ID | US-026 |
| Module | Procurement |
| Title | Create Purchase Request |
| Priority | High |

**User Story**

As a **Procurement Executive**, I want to create Purchase Requests so that material requirements are recorded.

**Acceptance Criteria**

- Material selection is mandatory.
- Quantity is mandatory.
- Purchase Request Number is generated automatically.

---

### User Story: US-027

| Field | Details |
|------|---------|
| Story ID | US-027 |
| Module | Procurement |
| Title | Generate Purchase Order |
| Priority | High |

**User Story**

As a **Procurement Manager**, I want to generate Purchase Orders so that materials can be procured from vendors.

**Acceptance Criteria**

- Approved Purchase Request is required.
- Vendor must be selected.
- Purchase Order Number is generated automatically.

---

### User Story: US-028

| Field | Details |
|------|---------|
| Story ID | US-028 |
| Module | Procurement |
| Title | Manage Vendor Information |
| Priority | Medium |

**User Story**

As a **Procurement Manager**, I want to maintain vendor records so that procurement activities are organized.

**Acceptance Criteria**

- Vendor details can be created and updated.
- Duplicate vendor records are prevented.
- Vendor list is searchable.

---

### User Story: US-029

| Field | Details |
|------|---------|
| Story ID | US-029 |
| Module | Procurement |
| Title | View Procurement Dashboard |
| Priority | Medium |

**User Story**

As a **Procurement Manager**, I want to monitor procurement activities through dashboards so that pending requests and purchase orders are visible.

**Acceptance Criteria**

- Dashboard displays pending Purchase Requests.
- Dashboard displays approved Purchase Orders.
- Vendor performance summary is available.

---

# 10. Inventory Module

## Epic: Inventory Management

---

### User Story: US-030

| Field | Details |
|------|---------|
| Story ID | US-030 |
| Module | Inventory |
| Title | Record Material Receipt |
| Priority | High |

**User Story**

As a **Store Manager**, I want to record material receipts so that inventory stock is updated accurately.

**Acceptance Criteria**

- Material Name is mandatory.
- Quantity is mandatory.
- Stock is updated automatically.

---

### User Story: US-031

| Field | Details |
|------|---------|
| Story ID | US-031 |
| Module | Inventory |
| Title | Issue Material |
| Priority | High |

**User Story**

As a **Store Manager**, I want to issue materials against approved project requirements so that inventory remains accurate.

**Acceptance Criteria**

- Quantity issued cannot exceed available stock.
- Stock balance updates automatically.
- Issue transaction is recorded.

---

### User Story: US-032

| Field | Details |
|------|---------|
| Story ID | US-032 |
| Module | Inventory |
| Title | Monitor Stock Levels |
| Priority | Medium |

**User Story**

As a **Store Manager**, I want to monitor stock levels so that material shortages are avoided.

**Acceptance Criteria**

- Current stock is displayed.
- Low-stock items are highlighted.
- Stock report can be exported.

---

### User Story: US-033

| Field | Details |
|------|---------|
| Story ID | US-033 |
| Module | Inventory |
| Title | View Inventory Dashboard |
| Priority | Medium |

**User Story**

As a **Store Manager**, I want to view inventory dashboards so that stock movements can be monitored efficiently.

**Acceptance Criteria**

- Dashboard displays current stock.
- Dashboard displays material receipts.
- Dashboard displays material issues.
- Dashboard displays low-stock alerts.

---

> **Business Analyst Observation**
>
> The Finance, Construction, Labour, Procurement, and Inventory modules support the core operational processes of Rajora ERP. These user stories provide clear, testable requirements that help development and QA teams implement functionality consistently while ensuring each business process can be validated during User Acceptance Testing (UAT).

---

# 11. Dashboard & Reporting

## Epic: Dashboard & MIS Reporting

---

### User Story: US-034

| Field | Details |
|------|---------|
| Story ID | US-034 |
| Module | Dashboard |
| Title | View Executive Dashboard |
| Priority | High |

**User Story**

As a **Managing Director**, I want to view an executive dashboard so that I can monitor the overall business performance from a single screen.

**Acceptance Criteria**

- Dashboard displays business KPIs.
- Dashboard displays project summary.
- Dashboard displays sales and collection summary.
- Dashboard loads successfully after login.

---

### User Story: US-035

| Field | Details |
|------|---------|
| Story ID | US-035 |
| Module | Dashboard |
| Title | Export Reports |
| Priority | Medium |

**User Story**

As a **Department Manager**, I want to export reports so that I can share business information with stakeholders.

**Acceptance Criteria**

- Reports can be exported to Excel.
- Reports can be exported to PDF.
- Applied filters are retained in exported reports.

---

### User Story: US-036

| Field | Details |
|------|---------|
| Story ID | US-036 |
| Module | Dashboard |
| Title | Filter Dashboard Data |
| Priority | Medium |

**User Story**

As a **Business User**, I want to filter dashboard information so that I can analyze specific projects or time periods.

**Acceptance Criteria**

- Dashboard supports date filters.
- Dashboard supports project filters.
- Dashboard refreshes automatically after filters are applied.

---

# 12. Administration & Security

## Epic: System Administration

---

### User Story: US-037

| Field | Details |
|------|---------|
| Story ID | US-037 |
| Module | Administration |
| Title | Manage Users |
| Priority | High |

**User Story**

As a **System Administrator**, I want to create and manage user accounts so that employees can securely access the ERP system.

**Acceptance Criteria**

- Administrator can create users.
- Administrator can edit users.
- Administrator can deactivate users.
- Username must be unique.

---

### User Story: US-038

| Field | Details |
|------|---------|
| Story ID | US-038 |
| Module | Administration |
| Title | Assign User Roles |
| Priority | High |

**User Story**

As a **System Administrator**, I want to assign roles to users so that they can access only the modules required for their job.

**Acceptance Criteria**

- One role can be assigned to each user.
- Users can only access authorized modules.
- Changes are effective immediately after saving.

---

### User Story: US-039

| Field | Details |
|------|---------|
| Story ID | US-039 |
| Module | Administration |
| Title | View Audit Log |
| Priority | Medium |

**User Story**

As a **System Administrator**, I want to review audit logs so that important system activities can be monitored.

**Acceptance Criteria**

- Login history is recorded.
- Record updates are logged.
- User account changes are logged.
- Audit logs are searchable by date.

---

# 13. Story Summary

The following table summarizes the user stories documented for each ERP module.

| Module | Number of User Stories |
|---------|-----------------------:|
| CRM | 6 |
| Sales | 6 |
| Finance | 5 |
| Construction | 4 |
| Labour | 4 |
| Procurement | 4 |
| Inventory | 4 |
| Dashboard & Reporting | 3 |
| Administration & Security | 3 |
| **Total** | **39** |

---

# 14. Requirement Traceability

The following table maps the Functional Requirements (FRD) to the corresponding User Stories.

| Functional Area | User Story IDs |
|-----------------|----------------|
| CRM | US-001 to US-006 |
| Sales | US-007 to US-012 |
| Finance | US-013 to US-017 |
| Construction | US-018 to US-021 |
| Labour | US-022 to US-025 |
| Procurement | US-026 to US-029 |
| Inventory | US-030 to US-033 |
| Dashboard & Reporting | US-034 to US-036 |
| Administration & Security | US-037 to US-039 |

> **Business Analyst Note**
>
> Each user story in this document is derived from the approved Functional Requirements Document (FRD). These stories form the product backlog for the Rajora ERP implementation and provide a clear basis for development, testing, and User Acceptance Testing (UAT).

---

# 15. Document Approval

The following stakeholders approve the User Stories document.

| Role | Name | Status |
|------|------|--------|
| Managing Director | Vishutosh Singh | Pending |
| CEO | — | Pending |
| Business Analyst | Shikha Phogat | Approved |

---

# Conclusion

The User Stories document converts the approved functional requirements into user-focused development requirements for the Rajora ERP implementation.

Each story clearly defines the user's objective, business value, priority, and acceptance criteria, ensuring that the development team understands the expected system behavior and that the testing team has measurable criteria for validation.

Together with the Business Requirements Document (BRD) and Functional Requirements Document (FRD), these User Stories provide a complete and traceable foundation for the successful delivery of the Rajora ERP – Enterprise Residential Construction Management System.

---

## Related Documents

| Document | Purpose |
|----------|---------|
| Business Discovery | Business understanding and stakeholder analysis |
| Business Requirements Document (BRD) | Business objectives and requirements |
| Functional Requirements Document (FRD) | Functional system specifications |
| User Stories | Agile development requirements |
| Process Models | Business workflows |
| Wireframes | User interface designs |
| Database Design | Data model and relationships |
| Testing & UAT | Functional validation |
| Power BI Dashboards | Reporting and analytics |

---

**Document Status:** Final

**Version:** 1.0

**Prepared By:** Shikha Phogat – Business Analyst

**Project:** Rajora ERP – Enterprise Residential Construction Management System

---
