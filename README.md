🎓 Placement Drive Management — ServiceNow Scoped App

A custom end-to-end scoped application built on ServiceNow App Engine to digitally transform and automate the campus placement process.

🚀 Key Features & Architecture
1. Relational Data Model

Engineered a custom relational schema within a dedicated ServiceNow scope (x_snc_placement) featuring interconnected tables for:

Companies
Students
Job Postings
Applications
2. Advanced Security (ACLs)

Implemented strict Role-Based Access Control (RBAC) using custom roles and Scripted Row-Level ACLs with gs.getUser().getEmail() to ensure data privacy and prevent unauthorized access to student application records.

3. Service Catalog & UX

Designed a frictionless frontend intake form using platform session data (caller_id) for dynamic identity resolution, eliminating the need for manual student information entry.

4. Flow Designer Automation

Built a zero-code backend automation pipeline triggered upon catalog submission. The flow dynamically cross-references user records and automatically generates the required Application junction records.

5. Platform Analytics

Configured real-time executive dashboards using:

Pie Charts
Bar Charts
Donut Charts
KPI Score Widgets

These dashboards provide insights into placement pipelines, application status, and company-wise recruitment metrics.

🔐 Security & Access Control (RBAC)

The application implements role-based permissions to ensure that each user can access only the data required for their responsibilities.

👨‍💼 Placement Officer
Company: Full CRUD access
Job Posting: Full CRUD access
Student: Full CRUD access
Application: Full CRUD access
🧑‍💼 HR Recruiter
Company: Read-only access
Job Posting: Full CRUD access
Student: Read-only access
Application: Full CRUD access
🎓 Student
Company: No access
Job Posting: Read-only access
Student: No access to other student records
Application: Read and Write access restricted to their own submitted records only

CRUD = Create, Read, Update, Delete

🛠️ Tech Stack & Skills
Platform Ecosystem
ServiceNow App Engine
ServiceNow Platform Analytics
Architecture
Scoped Applications
Relational Database Design
Custom Application Tables
Security
Access Control Lists (ACLs)
Role-Based Access Control (RBAC)
Scripted Row-Level ACLs
User-Based Data Restriction
Workflow Automation
Flow Designer
Service Catalog
Process Engine
Automated Record Creation
User Experience
Service Catalog Forms
Dynamic User Identity Resolution
caller_id Session Data
Analytics
Executive Dashboards
Pie Charts
Bar Charts
Donut Charts
KPI Score Widgets
