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

<h3>6. Allow anyone to create tickets </h3>

  - Stay on Admin Panel -> hover on Settings tab -> click Users

![image](https://github.com/user-attachments/assets/e46ade26-c1f0-4411-bcd2-be4343b567d0)

  - on User Settings, make sure the box is UNCHECKED for "Require registration and login to create tickets"
  - if it is, the uncheck the box and click Save Changes below

![image](https://github.com/user-attachments/assets/737d4ef6-e9d2-4446-8cd2-e15db2359e27)

<br />

<h3>7. Configure Agents </h3>

  - Now, we will create Agents to simulate people who work on the tickets
  - Stay on Admin Panel -> hover on Agents tab -> click Agents

![image](https://github.com/user-attachments/assets/d325d5dc-a793-4536-a1c4-0370919f22ce)

  - For this example, we will create two Agents. 1 system admin and 1 support
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

  - Click Access -> choose Support -> choose View Only -> click Create

![image](https://github.com/user-attachments/assets/6acc73b6-98f3-4e62-a0b7-29a0d9ebc2f1)

![image](https://github.com/user-attachments/assets/46f82772-a0d2-48bb-9fac-0b1fabb51d61)

![image](https://github.com/user-attachments/assets/b9e5d3a7-b94d-4f9a-badc-10ea4754be24)

<br />

<h3>8. Configure Users </h3>

  - Now, we will create two Users to simulate people who create the tickets
  - Go to Agent Panel, hover on Users Tab -> click User Directory

![image](https://github.com/user-attachments/assets/66bab3ce-008b-4ff2-a951-a13c40a876ed)

![image](https://github.com/user-attachments/assets/c8ec5e93-cc31-41b8-b973-c205d0a8e2a2)

  - Click Add User -> fill the email address and full name -> click Add User

![image](https://github.com/user-attachments/assets/e3cea49f-b37d-41f6-b558-0a87b4f9e6a7)

![image](https://github.com/user-attachments/assets/62a23d3a-de6e-40c9-a9c9-e0ad46716010)

  -  Go back to User Directory -> repeat the process but use a different name

![image](https://github.com/user-attachments/assets/98264150-e364-4d67-8202-87c35886e0b2)

![image](https://github.com/user-attachments/assets/7842062a-c51d-4a07-82a5-fb42268743d5)

![image](https://github.com/user-attachments/assets/4605a1c8-37da-414a-b690-b8a19912ee11)


<br />

<h3>9. Configure SLAs </h3>

  - Now, we will create SLAs (Service Level Agreements). This determines the severity of tickets
    and the appropriate incident response protocol
  - Go to Admin Panel -> hover on Manage and click SLA

![image](https://github.com/user-attachments/assets/326e8a5f-348b-46ae-8e88-abdf5151d300)

![image](https://github.com/user-attachments/assets/05ba303a-3474-4b67-af3e-aa125ecdb334)

  -  Click Add New SLA Plan

![image](https://github.com/user-attachments/assets/eec07a9a-5a62-4d14-9f5e-2791eab6b789)

  -  We will create 3 SLAs
  - Sev-A (Grace Period: 1 hour, Schedule: 24/7) then Add Plan

![image](https://github.com/user-attachments/assets/2785b38f-7c3d-4b33-a450-3342371388f4)

  - Sev-B (Grace Period: 4 hours, Schedule: 24/7) then Add Plan

![image](https://github.com/user-attachments/assets/7becf405-68d0-4055-877a-40ddeaf697c3)

  - Sev-C (Grace Period: 8 hours, Business Hours) then Add Plan

![image](https://github.com/user-attachments/assets/473b473f-3b76-4c87-be70-158798a27f92)

![image](https://github.com/user-attachments/assets/85012d45-3125-46dc-99d5-0e259881dd42)

<br />

<h3>10. Configure Help Topics </h3>

  -  Lastly, we will configure help topics for when users create a ticket
  -  Go to help topics and click Add New Help Topic

![image](https://github.com/user-attachments/assets/5a57d40a-6b71-4e1e-acb2-fdfdd08293f6)

![image](https://github.com/user-attachments/assets/9e455609-8444-439c-8d7f-c13d65199b60)

  -  We will create 5 help topics

  - Business Critical Outage / Report a Problem -> Add Topic -> back to Help Topics

![image](https://github.com/user-attachments/assets/1a8819fe-977e-4ee1-bce4-da5f927b2806)
      
  - Personal Computer Issues / Report a Problem -> Add Topic -> back to Help Topics

![image](https://github.com/user-attachments/assets/fcf76e6f-1271-44fe-951c-81974a7c956b)

  - Equipment Request / General Inquiry -> Add Topic -> back to Help Topics

![image](https://github.com/user-attachments/assets/24605199-c266-4222-8f36-3eb1b4c636fb)

  - Password Reset / Report a Problem -> Add Topic -> back to Help Topics

![image](https://github.com/user-attachments/assets/e21fa13c-f86d-41a1-b037-f8f062a3117c)

  - Other / General Inquiry -> Add Topic
 
![image](https://github.com/user-attachments/assets/71eb0578-c5df-4c77-8dbd-cf870a4b533e)

<br />

<h2>Congratulations on finishing the post installation and configuration of osTicket!</h2>

![image](https://github.com/user-attachments/assets/50839632-6ff8-4cfe-a993-dd4f92d135af)

<br />

<h3>Hope you find this helpful.</h3>
