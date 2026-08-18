🎓 Placement Drive Management (ServiceNow Scoped App)

A custom end-to-end scoped application built on ServiceNow (App Engine) to digitally transform and automate the campus placement process.

🚀 Key Features & Architecture
Relational Data Model: Engineered a custom schema within a dedicated scope (x_snc_placement) featuring interconnected tables for Companies, Students, Job Postings, and Applications.
Advanced Security (ACLs): Implemented strict Role-Based Access Control (RBAC) using custom roles and Scripted Row-Level ACLs (gs.getUser().getEmail()) to ensure data privacy.
Service Catalog & UX: Designed a frictionless frontend intake form that uses platform session data (caller_id) for dynamic identity resolution, eliminating manual data entry.
Flow Designer Automation: Built a zero-code backend pipeline that triggers upon catalog submission, dynamically cross-references user records, and auto-generates application junction records.
Platform Analytics: Configured real-time executive dashboards (Pie, Bar, Donut, and KPI Score widgets) to track placement pipelines and company-wise metrics.

🔐 Security & Access Control (RBAC)
Placement Officer: Full CRUD (Create, Read, Update, Delete) access across all system tables (Company, Job Posting, Student, Application).
HR Recruiter: CRUD access to Job Postings and Applications. Read-only access to Company and Student records.
Student: Read-only access to Job Postings. Read and Write access to the Application table is strictly limited to their own submitted records. No access to Company or other Student records.

🛠️ Tech Stack & Skills
Platform Ecosystem: ServiceNow App Engine, Platform Analytics
Architecture: Scoped Applications, Relational Database Design
Security: Access Control Lists (ACLs), Role-Based Access Control (RBAC)
Workflow Automation: Flow Designer, Service Catalog, Process Engine
