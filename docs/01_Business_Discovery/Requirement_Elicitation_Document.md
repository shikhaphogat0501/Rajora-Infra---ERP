Requirement Elicitation Document (RED)

Project Name: Rajora ERP – Enterprise Residential Construction Management System
Document ID: RED-001
Version: 1.0
Prepared By: Shikha Phogat – Business Analyst
Prepared For: Rajora Infra Homes Management
Date: July 2026
Document Status: Approved for Business Requirements Documentation (BRD)

Table of Contents

1.Purpose
2.Project Vision
3.Business Objectives
4.Requirement Gathering Approach
5.Stakeholders
6.Existing Business Process
7.Stakeholder Interviews
8.Functional Requirements
9.Non-Functional Requirements
10.Business Rules
11.Assumptions
12.Constraints
13.Risks
14.Requirement Prioritization
15.Open Items
16.Conclusion

1. Purpose

The purpose of this Requirement Elicitation Document is to capture, validate, and document the business needs of Rajora Infra Homes for the implementation of an integrated Enterprise Resource Planning (ERP) solution.

The document records information collected through stakeholder interviews, process observations, and analysis of existing operational documents. The requirements documented here will serve as the foundation for the Business Requirements Document (BRD), Functional Requirements Document (FRD), User Stories, and subsequent phases of the software development lifecycle.

2. Project Vision

Rajora Infra Homes currently manages its business operations through multiple Excel spreadsheets, manual registers, and isolated reporting practices. This approach has resulted in duplicate data, reporting delays, inconsistent records, and limited visibility across departments.

The proposed Rajora ERP aims to integrate all major business functions into a centralized platform that supports efficient operations, standardized processes, and real-time decision-making.

The ERP solution will cover the following business domains:

•Sales & CRM
•Customer Management
•Booking Management
•Loan Management
•Construction Management
•Labour Management
•Procurement
•Vendor Management
•Inventory Management
•Finance & Accounts
•Executive Reporting & Analytics

3. Business Objectives

The key objectives identified during stakeholder discussions are:

•Replace manual Excel-based operations with a centralized ERP.
•Improve collaboration between departments.
•Eliminate duplicate and inconsistent business records.
•Enable real-time tracking of sales, collections, construction progress, labour, and inventory.
•Improve management reporting through interactive dashboards.
•Automate approval workflows.
•Increase operational efficiency and data accuracy.
•Provide management with timely and reliable information for decision-making.
•Improve customer experience through better visibility of bookings and payments.

4. Requirement Gathering Approach

The following elicitation techniques were used to identify business requirements.

Technique                                	Purpose
Stakeholder Interviews	          Understand business goals, challenges, and expectations
Process Observation	              Analyze current operational workflows
Document Analysis	                Review Excel files, registers, reports, and business forms
Workshops	                        Validate cross-functional requirements
Brainstorming Sessions	          Identify opportunities for automation and process improvement

5. Stakeholders

Stakeholder                  	    Department	                                Primary Responsibility
Managing Director	                Executive Management	                      Strategic planning and decision-making
CEO                               Executive Management	                      Business objectives and ERP vision
Sales Manager                     Sales	                                      Lead generation and customer acquisition
CRM Executive                     Customer Relationship Management	          Customer communication and follow-ups
Finance Manager	                  Finance	                                    Payments, collections, accounting
Project Manager	                  Construction	                              Project planning and execution
Site Engineer	                    Construction	                              Daily site supervision
Labour Supervisor	                Operations	                                Labour attendance and deployment
Procurement Manager	              Procurement	                                Material purchasing
Store Manager	                    Inventory	                                  Inventory management
Customers	                        External	                                  Property purchase and payment
Vendors	                          External	                                  Material supply and services

6. Existing Business Process

The current operational workflow is summarized below.

Marketing Campaign

↓

Lead Generation

↓

Customer Enquiry

↓

Site Visit

↓

Property Selection

↓

Booking

↓

Customer KYC

↓

Bank Loan Processing

↓

Agreement Signing

↓

Construction

↓

Stage-wise Customer Payments

↓

Quality Inspection

↓

Registry

↓

Possession

Supporting activities such as procurement, labour attendance, inventory updates, and financial reporting are managed independently through Excel spreadsheets and manual registers.

7. Stakeholder Interviews

7.1 Executive Management

Objective
Understand organizational goals and strategic expectations from the ERP solution.

Questions Asked
1.What are the major operational challenges today?
2.Which departments require the highest level of automation?
3.What reports are reviewed during management meetings?
4.What information should be available in real time?
5.What business improvements are expected after ERP implementation?

Key Findings
•Departments maintain separate Excel files.
•Reports require manual consolidation.
•Real-time project visibility is unavailable.
•Decision-making is delayed due to scattered information.
•Executive dashboards are required for monitoring KPIs.

Requirements Identified
•Centralized ERP database
•Executive dashboard
•Real-time reporting
•Department integration
•Automated MIS reports

7.2 Sales Department

Objective
Understand lead management and booking operations.

Questions Asked
1.How are leads generated?
2.How are leads assigned?
3.What customer information is collected?
4.How are follow-ups managed?
5.How are bookings recorded?
6.Can customers reserve multiple units?
7.What reports are required daily?

Key Findings
•Leads originate from digital campaigns, referrals, and walk-ins.
•Follow-ups are maintained manually.
•Booking information is recorded in Excel.
•Sales reports require manual preparation.

Requirements Identified
•Lead Management Module
•Customer Master
•Follow-up Scheduler
•Booking Management
•Sales Dashboard

7.3 CRM Department

Objective
Understand customer communication and document management.

Questions Asked
1.How are customer interactions tracked?
2.How are reminders managed?
3.How are complaints handled?
4.Which customer documents are maintained?

Key Findings
•Customer communication history is not centralized.
•Reminder tracking is manual.
•Complaint resolution lacks visibility.
•Documents are stored in multiple locations.

Requirements Identified
•Customer Interaction History
•Reminder Management
•Complaint Tracking
•Document Repository

7.4 Finance Department

Objective
Understand financial operations and payment tracking.

Questions Asked
1.How are customer payments recorded?
2.How are outstanding balances monitored?
3.How are GST calculations performed?
4.How are refunds processed?
5.Which financial reports are required?

Key Findings
•Payments are maintained in Excel.
•Outstanding balances require manual calculation.
•GST is calculated using spreadsheet formulas.
•Financial reports are manually consolidated.

Requirements Identified
•Payment Management Module
•Automated GST Calculation
•Installment Tracking
•Receipt Generation
•Finance Dashboard
•Outstanding Payment Alerts

7.5 Construction Department

Objective
Understand project execution and progress monitoring.

Questions Asked
1.How is construction progress monitored?
2.Who updates project status?
3.How are delays identified?
4.Which reports are required?

Key Findings
•Progress updates are communicated manually.
•Delays are difficult to identify.
•No centralized construction tracking exists.

Requirements Identified
•Construction Management Module
•Stage-wise Progress Tracking
•Delay Monitoring
•Project Dashboard

7.6 Site Engineering Team

Objective
Understand site-level reporting activities.

Questions Asked
1.How is daily work recorded?
2.How are inspections documented?
3.How are issues escalated?

Key Findings
•Site updates rely on WhatsApp and Excel.
•Inspection records are paper-based.
•Issue tracking is inconsistent.

Requirements Identified
•Daily Progress Reporting
•Inspection Management
•Issue Tracking System

7.7 Labour Management

Objective
Understand workforce administration.

Questions Asked
1.How is attendance recorded?
2.How are wages calculated?
3.Can labour work on multiple projects?
5.Which reports are required?

Key Findings
•Attendance is maintained in manual registers.
•Wage calculations are manual.
•Labour deployment lacks centralized visibility.

Requirements Identified
•Digital Attendance
•Wage Calculation
•Labour Allocation
•Productivity Dashboard

7.8 Procurement Department

Objective
Understand purchasing operations.

Questions Asked
1.How are purchase requests initiated?
2.How are vendors selected?
3.Who approves purchases?
4.How are deliveries monitored?

Key Findings
•Material requests are communicated manually.
•Purchase approvals are paper-based.
•Vendor comparisons are maintained in Excel.

Requirements Identified
•Purchase Request Module
•Vendor Management
•Purchase Order Workflow
•Approval Workflow
•Delivery Tracking

7.9 Inventory Department

Objective
Understand inventory control.

Questions Asked
1.How is inventory maintained?
2.How are material issues recorded?
3.Which inventory reports are required?

Key Findings
•Inventory records are maintained in Excel.
•Material issues are recorded manually.
•Stock reconciliation is time-consuming.

Requirements Identified
•Inventory Management
•Material Issue Register
•Stock Alerts
•Inventory Dashboard

8. Functional Requirements (High-Level)

The following high-level functional requirements were identified.

Module	                                Functional Requirements
Sales	                                  Lead creation, assignment, follow-up, booking
Customer	                              Registration, KYC, agreements, communication history
Finance	                                Payment collection, receipts, GST, installments
Construction	                          Progress updates, milestones, inspections
Labour	                                Attendance, wages, deployment
Procurement                            	Purchase requests, approvals, purchase orders
Inventory                              	Material receipt, issue, transfers, stock monitoring
Vendor	                                Vendor registration, quotations, evaluations
Reporting	                              Executive dashboards, operational dashboards, KPI reports

9. Non-Functional Requirements

Category	                              Requirement
Security	                              Role-based access control
Availability	                          99.5% system availability
Performance	                            Dashboards should load within five seconds
Scalability	                            Support multiple residential projects
Backup	                                Daily automated backups
Audit	                                  Complete transaction audit trail
Compatibility	                          Support Chrome, Edge, Firefox
Usability	                              User-friendly interface with minimal training

10. Business Rules

The following business rules were identified.

1.Each customer shall have a unique Customer ID.
2.Each booking shall have a unique Booking Number.
3.Customer KYC must be completed before booking confirmation.
4.Construction shall begin only after required approvals.
5.Labour wages shall be calculated using approved attendance.
6.Inventory cannot issue materials exceeding available stock.
7.Purchase Orders exceeding predefined limits require management approval.
8.Payment receipts shall be generated automatically for every customer payment.
9.Construction progress shall be updated stage-wise.
10.Only authorized users may approve financial transactions.

11. Assumptions

•All departments will participate in ERP implementation.
•Existing operational data will be migrated into the new system.
•Users will receive adequate ERP training.
•Internet connectivity will be available across project locations.
•Stakeholders will validate documented requirements before design begins.

12. Constraints

•Existing data quality may require cleansing before migration.
•Initial implementation will be limited to one residential project.
•Project budget and implementation timeline are fixed.
•Users have varying levels of technical expertise.

13. Risks

Risk	                           Impact	                        Mitigation
Resistance to change	            High	                    User training and change management
Poor data quality	                High	                    Data cleansing before migration
Requirement changes	             Medium	                    Formal change management process
Delayed stakeholder feedback	   Medium                    	Weekly review meetings

14. Requirement Prioritization (MoSCoW)

Must Have
•Customer Management
•Sales CRM
•Booking Management
•Finance
•Inventory
•Labour
•Construction Tracking
•Executive Dashboard

Should Have
•Vendor Portal
•SMS Notifications
•Email Notifications
•Complaint Management

Could Have
•Customer Mobile Application
•QR-based Attendance
•GPS-enabled Site Tracking

Won't Have (Phase 1)
•AI-based Forecasting
•IoT Integration
•Predictive Analytics

15. Open Items

The following topics require further discussion during the Business Requirements phase.

•Should customers have access to an online self-service portal?
•Will mobile applications be provided to site engineers and supervisors?
•What approval hierarchy should be followed for procurement?
•Which reports must be available in real time?
•Will the ERP integrate with external accounting or banking systems?

16. Conclusion

The Requirement Elicitation phase identified the primary business needs of Rajora Infra Homes through structured stakeholder analysis, process observation, and review of existing operational practices. The findings confirm that the organization requires a centralized ERP solution to improve operational efficiency, reporting accuracy, collaboration, and decision-making.

The requirements documented in this report establish the baseline for preparing the Business Requirements Document (BRD), where each business need will be translated into detailed and traceable business requirements for implementation.

Document Approval

Role	                  Name	
Business Analyst    	Shikha Phogat	
Project Sponsor      	Managing Director	Vishutosh Singh
______	__________	__________
