# Optimizing-User-Group-and-Role-Management-with-Access-Control-and-Workflows

📘 Overview
This project demonstrates how ServiceNow can be used to create a secure and automated project task management system using Role-Based Access Control (RBAC), Flow Designer, and Dashboards.

It was developed as part of the Naan Mudhalvan / SmartInternz Internship Program, showcasing practical use of ServiceNow’s low-code capabilities to enhance project workflow visibility and accountability.

🎯 Problem Statement
In a small project team with a Project Manager (Alice) and a Team Member (Bob), the lack of structured roles, access restrictions, and automation leads to:

Confusion over task ownership
Uncontrolled data access
Difficulty tracking task progress
This project solves these issues by implementing role-based permissions, workflow automation, and visual reporting within ServiceNow.

🧠 Objective
To build a custom ServiceNow application that:

Defines distinct Users, Groups, and Roles
Enforces Access Controls (ACLs) on data
Automates task workflows using Flow Designer
Displays real-time reports and dashboards
⚙️ Tools & Technologies
Component	Tool/Feature Used
Platform	ServiceNow
Modules	User Administration, Flow Designer, Access Control (ACL), Reporting
Application Scope	Custom Scoped App: Project Task Management
Roles	x_project_manager, x_team_member
Dashboard Tools	Reports and Performance Analytics
🧩 Key Features
1. User, Group, and Role Management
Created users: Alice (Manager) and Bob (Team Member)
Created groups: Project Managers, Team Members
Created roles: x_project_manager, x_team_member
Assigned roles to groups and users for controlled access
2. Custom Scoped Application
Application Name: Project Task Management
Custom Table: Project Task (x_scope_project_task)
Fields: Task Title, Description, Assigned To, Status, Created By, Due Date
3. Access Control (ACL) Implementation
Managers: Full access (Create, Read, Write, Delete)
Team Members: Restricted to assigned tasks only
ACL scripts enforce security on both record and field levels
4. Workflow Automation (Flow Designer)
Trigger: Record creation or update
Condition: When a task is assigned
Actions:
Auto-update Status to “Assigned”
Send notifications to assigned user and manager
Update status to “Completed” when marked done
5. Reports & Dashboards
Pie Chart: Tasks by Status
Bar Chart: Tasks by Assigned User
Combined into a Dashboard for Project Manager
🧪 Testing Scenarios
Test Case	Action	Expected Result
Alice creates a new task and assigns Bob	Task created; status auto-changes to Assigned	✅
Bob views assigned tasks	Only his assigned tasks visible	✅
Bob updates task status to In Progress	Allowed; Manager notified	✅
Bob tries to edit other task fields	Access Denied	✅
Alice deletes a task	Successful	✅
📊 Outcome
🔒 Secure access control per user role
⚙️ Automated workflow reduces manual updates
📈 Dashboards give real-time project visibility
🤝 Improved accountability between manager and team member

