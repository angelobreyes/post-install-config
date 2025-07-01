<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
Welcome to the next step of osTicket installation! This tutorial outlines the post-install configuration of osTicket where we will create/configure the roles (Admin, Agents, Users), teams, permissions, and etc.

<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Configure Users
- Configure SLAs ( Service Level Agreements ) and Help Topics

<h2>Configuration Steps</h2>

<h3>1. Log in to the Admin/Analyst page.</h3>

  - Go to http://localhost/osTicket/scp/login.php and log in. Use the Admin username and password you made from the previous lab.

![image](https://github.com/user-attachments/assets/d61c2fb0-4abd-4131-9dd8-b496c4d128a1)

<br />

<h3>2. Take note of Admin Panel and Agent Panel.</h3>

  - Once you're logged in, look to the top-right corner, "Admin Panel" and click. This panel allows you a wide variety of configurations and settings as an Administrator.

![image](https://github.com/user-attachments/assets/e53d2841-34be-4c79-ae4f-4ac097151438)

![image](https://github.com/user-attachments/assets/8dff88ca-625e-4265-a94d-a233829f279b)

<br />

  - Then click on "Agent Panel" and observe. You'll see that this panel doesn't have the variety of options and focuses on tickets and tasks as an Agent.

![image](https://github.com/user-attachments/assets/d632575f-4579-41ef-8a1b-1e3604d112e4)

![image](https://github.com/user-attachments/assets/6355d8d0-4884-44e8-ad12-eb5ce3cc8cbf)

<br />

<h3>3. Configure Roles.</h3>

  - First, we will create a role with all permissions allowed to simulate a head administrator.
  - Go to the Admin Panel -> hover on Agents tab -> click Roles

![image](https://github.com/user-attachments/assets/e53d2841-34be-4c79-ae4f-4ac097151438)

![image](https://github.com/user-attachments/assets/4bf4e105-cdc9-4e28-a293-d778f9b9fa49)

  - Click Add New Role -> type in the name of your Admin -> click Permissions and click all checkboxes

![image](https://github.com/user-attachments/assets/71b2422d-6950-4209-a87a-6953697e45c6)

![image](https://github.com/user-attachments/assets/278430b0-2e9a-463c-b03f-32b56c5b9177)

![image](https://github.com/user-attachments/assets/e800c4c1-c7bf-490d-9a4a-2cde2739a7c1)





<br />


Configure Roles (for grouping permissions)
Admin Panel -> Agents -> Roles
Supreme Admin

Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)
Admin Panel -> Agents -> Departments
SysAdmins

Configure Teams
Admin Panel -> Agents -> Teams (Pull Agents from different Departments)
Online Banking

Allow anyone to create tickets
Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)
Registration Required: Require registration and login to create tickets 

Configure Agents (workers)
Admin Panel -> Agents -> Add New
Jane (Dept: SysAdmins)
John (Dept: Support)

Configure Users (customers)
Agent Panel -> Users -> Add New
Karen
Ken

Configure SLA
Admin Panel -> Manage -> SLA
Sev-A (Grace Period: 1 hour, Schedule: 24/7)
Sev-B (Grace Period: 4 hours, Schedule: 24/7)
Sev-C (Grace Period: 8 hours, Business Hours)

Configure Help Topics (For when users create a ticket)
Admin Panel -> Manage -> Help Topics
Business Critical Outage
Personal Computer Issues
Equipment Request
Password Reset
Other

