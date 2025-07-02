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

  - We will create a role with all permissions allowed to simulate a head administrator.
  - Go to the Admin Panel -> hover on Agents tab -> click Roles

![image](https://github.com/user-attachments/assets/e53d2841-34be-4c79-ae4f-4ac097151438)

![image](https://github.com/user-attachments/assets/4bf4e105-cdc9-4e28-a293-d778f9b9fa49)

  - Click Add New Role -> type in the name of your Admin -> click Permissions and click all checkboxes -> click Add Role

![image](https://github.com/user-attachments/assets/71b2422d-6950-4209-a87a-6953697e45c6)

![image](https://github.com/user-attachments/assets/278430b0-2e9a-463c-b03f-32b56c5b9177)

![image](https://github.com/user-attachments/assets/e800c4c1-c7bf-490d-9a4a-2cde2739a7c1)

![image](https://github.com/user-attachments/assets/af9acf37-ec3b-4cad-b0ea-1a8ca68a5bb7)

![image](https://github.com/user-attachments/assets/cf8f5ee6-c818-47fa-8751-44886997c852)

![image](https://github.com/user-attachments/assets/811dbdfa-35d0-47e8-834e-937efd8b1049)

<br />

<h3>4. Configure Departments. (Ticket Visibility, Help Desk vs SysAdmins, vs Networking) </h3>

  - You can create different departments such as Networking, Sys Admins and Help Desk. 
    
  - To configure departments, stay on Admin Panel and click Departments (under Agents)

![image](https://github.com/user-attachments/assets/4a82cf4e-e362-4d88-b6e1-a77532e3b11a)

  - Click Add New Department

![image](https://github.com/user-attachments/assets/07337b2f-b27f-4331-9e6b-a0dd0a9080eb)

  - Type in the name of the Department you want to create -> scroll down and click Create Dept

![image](https://github.com/user-attachments/assets/fd44d7eb-f61e-4ffd-b82a-1e1a72af54ec)

![image](https://github.com/user-attachments/assets/54c95af5-e8c0-44b6-b37f-9cdd7e3734db)

<br />

<h3>5. Configure Teams </h3>

  - To configure Teams, stay on Admin Panel and Agents tab -> click Agents

![image](https://github.com/user-attachments/assets/7d28d489-0b4d-4bef-acd9-83cec2767722)

  - On the Agents page, click Teams -> click Add New Team 

![image](https://github.com/user-attachments/assets/a1eeaaa0-a8c6-4722-a980-2f334f1f9d4c)

![image](https://github.com/user-attachments/assets/8e39d302-5279-4154-9a02-a0ac63163e0e)

  - For this example, type in Online Banking and click Create Team

![image](https://github.com/user-attachments/assets/c9538a02-790e-49c7-a867-4d38b52f5980)

![image](https://github.com/user-attachments/assets/64c5a1f5-00c6-42af-99c7-2e34c7150159)

<br />

<h3>5. Allow anyone to create tickets </h3>

  - Stay on Admin Panel -> hover on Settings tab -> click Users

![image](https://github.com/user-attachments/assets/e46ade26-c1f0-4411-bcd2-be4343b567d0)

  - on User Settings, make sure the box is UNCHECKED for "Require registration and login to create tickets"
  - if it is, the uncheck the box and click Save Changes below

![image](https://github.com/user-attachments/assets/737d4ef6-e9d2-4446-8cd2-e15db2359e27)

<br />

<h3>6. Configure Agents </h3>

  - Now, we will create Agents to simulate people who work on the tickets
  - Stay on Admin Panel -> hover on Agents tab -> click Agents

![image](https://github.com/user-attachments/assets/d325d5dc-a793-4536-a1c4-0370919f22ce)

  - For this example, we will create two Agents.
  - Click Add New Agent 

![image](https://github.com/user-attachments/assets/e81382b3-ca61-46e5-b2d5-20c2e2bab5de)

  - Name : Jane Doe
  - Email : jane@heldesk.com
  - Username : janedoe
  - Click Set Password

![image](https://github.com/user-attachments/assets/9833ce33-3007-4504-b094-39a2e572e6d8)

  - Uncheck the two boxes and type in a password then click Set

![image](https://github.com/user-attachments/assets/f5d060b4-c60d-4537-8320-3b1e16c84e6e)

 - Click Access -> choose System Administrators -> choose Senior Administrator -> Assign to Online Banking and create

![image](https://github.com/user-attachments/assets/d80de3dc-7738-436e-afde-42a5e720605a)

![image](https://github.com/user-attachments/assets/28e2ae96-93a5-4aba-bb3a-f62fc0978625)

![image](https://github.com/user-attachments/assets/6bbe850f-1b9b-493e-a9e3-1278e494045c)

![image](https://github.com/user-attachments/assets/136447db-f58d-4d91-8e3e-c9db5df136df)

 - We will create one more agent, go back to Agents page
  - Click Agents -> Add New Agent

![image](https://github.com/user-attachments/assets/5345e997-6a53-4635-82cf-e95cbd0c6dcf)

![image](https://github.com/user-attachments/assets/288c1035-f06a-4f96-9397-918e30c0d50b)

  - Name : John Doe
  - Email : john@helpdesk.com
  - Username : johndoe
  - Click Set Password

![image](https://github.com/user-attachments/assets/629c73ad-5126-465d-9527-c825d8418b23)

  - Uncheck the two boxes and type in a password then click Set

![image](https://github.com/user-attachments/assets/7e738620-fd06-432a-bebd-2bcdb5effe49)

  - Click Access -> choose Support -> choose limited Access

![image](https://github.com/user-attachments/assets/6acc73b6-98f3-4e62-a0b7-29a0d9ebc2f1)






<br />

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

