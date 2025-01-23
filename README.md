<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Set up roles and permissions for agents and users.
- Configure ticket visibility and help desk functionality.
- Establish SLAs to define response times for tickets.
- Enhance user experience by organizing help topics.
- Secure the osTicket system with proper permissions and user settings.

<h2>Configuration Steps</h2>

### Step 1: Configure Roles
- Navigate to Admin Panel -> Agents -> Roles.
- Create a role:
  - Supreme Admin

### Step 2: Configure Departments
- Navigate to Admin Panel -> Agents -> Departments.
- Create departments for ticket visibility:
  - Example: SysAdmins
 
### Step 3: Configure Teams
- Navigate to Admin Panel -> Agents -> Teams.
- Create a team and pull agents from different departments:
  - Example: Online Banking
 
### Step 4: User Settings
- Navigate to Admin Panel -> Settings -> User Settings.
- Configure ticket creation settings:
  - Uncheck: Unregistered users can create tickets.
  - Require registration and login to create tickets.

### Step 5: Configure Agents (Workers)
- Navigate to Admin Panel -> Agents -> Add New.
- Add agents:
  - Jane (Dept: SysAdmins)
  - John (Dept: Support)

### Step 6: Configure Users (Customers)
- Navigate to Agent Panel -> Users -> Add New.
- Add users:
  - Karen
  - Ken
 
### Step 7: Configure SLA
- Navigate to Admin Panel -> Manage -> SLA.
- Create SLAs:
  - Sev-A (Grace Period: 1 hour, Schedule: 24/7)
  - Sev-B (Grace Period: 4 hours, Schedule: 24/7)
  - Sev-C (Grace Period: 8 hours, Business Hours)

### Step 8: Configure Help Topics
- Navigate to Admin Panel -> Manage -> Help Topics.
- Add help topics:
  - Business Critical Outage
  - Personal Computer Issues
  - Equipment Request
  - Password Reset
  - Other

## Conclusion
These steps complete the post-installation setup for osTicket. With these configurations, you can manage your help desk efficiently and ensure a smooth workflow for both agents and users.

