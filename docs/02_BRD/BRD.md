# Business Requirements Document (BRD)

**Project:** Rajora ERP – Enterprise Resource Planning System  
**Company:** Rajora Infra Homes  
**Document ID:** BRD-001  
**Version:** 1.0  
**Prepared By:** Shikha Phogat – Business Analyst  
**Status:** Final  

---

# Version History

| Version | Date | Author | Description |
|---------|------|--------|-------------|
| 0.1 | July 2026 | Shikha Phogat | Initial Draft |
| 1.0 | July 2026 | Shikha Phogat | Final Version |

# 1. Purpose

The purpose of this Business Requirements Document (BRD) is to define the business needs, objectives, scope, and high-level requirements for implementing the Rajora ERP solution. It serves as the baseline for Functional Requirements, User Stories, Solution Design, Development, Testing, and User Acceptance Testing.

# 2. Business Problem

Rajora Infra Homes currently manages operations using spreadsheets and manual processes, resulting in duplicate data, delayed reporting, limited visibility, and inefficient approvals.

# 3. Project Background

Rajora ERP will integrate CRM, Sales, Finance, Construction, Labour, Procurement, Inventory, and Reporting into a centralized ERP platform.

# 4. Business Objectives

- Standardize business processes
- Improve operational efficiency
- Digitize approvals
- Enable real-time reporting
- Improve customer management
- Improve project monitoring
- Improve financial visibility
- Improve inventory accuracy

# 5. Project Scope

## CRM
- Lead Management
- Customer Master
- Follow-up Management
- Complaint Management

## Sales
- Unit Availability
- Booking Management
- Agreement Management
- Installment Planning

## Finance
- Collections
- Receipts
- GST
- Outstanding Tracking

## Construction
- Project Tracking
- Milestones
- Progress Updates
- Delay Monitoring

## Labour
- Registration
- Attendance
- Wage Calculation
- Productivity

## Procurement
- Purchase Requests
- Purchase Orders
- Vendor Management

## Inventory
- Material Receipt
- Material Issue
- Stock Management

## Dashboards
- Executive Dashboard
- Department Dashboards
- MIS Reporting

## Administration
- Users
- Roles
- Audit Logs

# 6. Out of Scope

- Payroll
- Mobile App
- AI Forecasting
- IoT Integration
- Customer Portal

# 7. Stakeholders

| Stakeholder | Role |
|-------------|------|
| Managing Director | Sponsor |
| CEO | Executive Stakeholder |
| Business Analyst | Requirements |
| Sales Manager | Sales Owner |
| Finance Manager | Finance Owner |
| Project Manager | Construction Owner |
| Procurement Manager | Procurement Owner |
| Store Manager | Inventory Owner |
| HR Executive | Labour Owner |

# 8. Business Requirements

## CRM
| ID | Requirement | Priority |
|---|---|---|
|BR-CRM-001|Lead Creation|High|
|BR-CRM-002|Lead Assignment|High|
|BR-CRM-003|Lead Tracking|High|
|BR-CRM-004|Follow-up Management|High|
|BR-CRM-005|Duplicate Detection|High|
|BR-CRM-006|Customer Master|High|
|BR-CRM-007|Document Upload|Medium|
|BR-CRM-008|Communication History|Medium|
|BR-CRM-009|Complaint Management|Medium|
|BR-CRM-010|CRM Dashboard|High|

## Sales
| ID | Requirement |
|---|---|
|BR-SALES-001|Unit Availability|
|BR-SALES-002|Booking Management|
|BR-SALES-003|Booking Approval|
|BR-SALES-004|Agreement Generation|
|BR-SALES-005|Installment Schedule|
|BR-SALES-006|Cancellation|
|BR-SALES-007|Sales Performance|
|BR-SALES-008|Discount Approval|
|BR-SALES-009|Target Tracking|
|BR-SALES-010|Sales Dashboard|

## Finance
- BR-FIN-001 Payment Recording
- BR-FIN-002 Receipt Generation
- BR-FIN-003 Outstanding Tracking
- BR-FIN-004 GST Calculation
- BR-FIN-005 Customer Ledger
- BR-FIN-006 Installment Management
- BR-FIN-007 Bank Reconciliation
- BR-FIN-008 Audit Trail
- BR-FIN-009 Financial MIS
- BR-FIN-010 Finance Dashboard

## Construction
- Project Master
- Milestones
- Daily Progress
- Delay Monitoring
- Budget Monitoring
- Quality Inspection
- Construction Dashboard

## Labour
- Labour Registration
- Attendance
- Wage Calculation
- Productivity
- Labour Dashboard

## Procurement
- Purchase Requests
- Vendor Management
- Purchase Orders
- Approval Workflow
- Procurement Dashboard

## Inventory
- Material Master
- Material Receipt
- Material Issue
- Low Stock Alerts
- Inventory Dashboard

## Dashboard & Reporting
- Executive Dashboard
- Sales Dashboard
- Finance Dashboard
- Construction Dashboard
- Labour Dashboard
- Procurement Dashboard
- Inventory Dashboard
- Scheduled MIS Reports

## Administration & Security
- User Management
- RBAC
- Password Policy
- Audit Logs
- Backup & Recovery

# 9. Functional Requirements

The system shall:
- Authenticate users.
- Manage leads and customers.
- Manage bookings.
- Record payments.
- Track construction progress.
- Capture labour attendance.
- Manage procurement.
- Maintain inventory.
- Generate dashboards.
- Export reports.

# 10. Non-Functional Requirements

- 99.5% availability
- Secure authentication
- Audit logging
- Daily backup
- Responsive UI
- Role-based security
- Encrypted data
- Scalable architecture

# 11. Business Rules

- One unit can only be booked once.
- Duplicate customers are not allowed.
- Attendance cannot be entered for future dates.
- Purchase approvals follow approval matrix.
- Material cannot be issued beyond available stock.

# 12. Reporting Requirements

- Daily MIS
- Weekly MIS
- Monthly MIS
- Executive Reports
- Sales Reports
- Finance Reports
- Construction Reports
- Labour Reports
- Procurement Reports
- Inventory Reports

# 13. Acceptance Criteria

- Approved requirements implemented.
- Successful UAT.
- Accurate dashboards.
- Successful data migration.
- Secure role-based access.
- No critical production defects.

# 14. Risks

| Risk | Mitigation |
|------|------------|
|Data quality|Data cleansing|
|User resistance|Training|
|Scope creep|Change control|
|Approval delays|Governance|

# 15. Sign-off

| Role | Status |
|------|--------|
|Managing Director|Pending|
|CEO|Pending|
|Project Manager|Pending|
|Business Analyst|Approved|

---

**End of Document**
