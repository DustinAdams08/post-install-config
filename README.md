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

- Windows 11</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

1.	Item 1 – Configuration of Roles for Grouping Permissions
2.	Item 2 – Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Network
3.	Item 3 – Configure Teams (Admin Panel, Agents, and Teams)
4.	Item 4 – Configure Agents (workers)
5.	Item 5 – Configure Users (customers)
6.	Item 6 – Configure SLA (Admin Panel, Manage, and SLA)
7.	Item 7 – Configure Help Topics (For when users create a ticket)


<h2>Configuration Steps</h2>

Step 1. Admin Login Page 
•[	http://localhost/osTicket/scp/login.php](http://localhost/osTicket/scp/login.php)

•	Username: adminuser
•	Password: Password1

![image](https://github.com/user-attachments/assets/2b9b24a8-88eb-43e8-96b0-2754a5d71981)

Step 2. Configure Roles
•	Click on Admin Panel in the right-hand corner
•	Then click the Agent Tab
•	Then Roles

![image](https://github.com/user-attachments/assets/c714c6d4-e629-4f1a-8b42-04391269fb4a)

Step 3. Configure Departments 
•	Allow SysAdmin to see all Departments
•	Admin Panel – Agents – Departments
•	Click Add New Department
•	Select Top Level Department
•	Then, click create after you enter the name SysAdmin

![image](https://github.com/user-attachments/assets/4e36f69d-94ed-43c0-8076-c7de501443fb)

Step 4. Configure Teams
•	From Admin Panel – Agents – Teams
•	This will put agents from different Departments on a Team
•	Name it Online Banking and click Create Team

![image](https://github.com/user-attachments/assets/7cc9394e-7469-446e-bc49-92d11fb6c1b8)

Step 5. Allow Anyone to create Tickets
•	Under the Admin Panel – Click Settings – User Settings
•	Uncheck The Registration Required Box

![image](https://github.com/user-attachments/assets/5f3b0b5a-a475-4d72-946c-ea05838b77c6)

Step 6. Configure Agents (Workers)
•	Under Admin Panel – Click Agents – Add New
•	Create New Agent - osTicket
•	Under Account: Jane Doe – email: jane@lognpacific.com – password: Password1
•	Under Access: Department: SysAdmin – Role: Supreme Admin
•	Under Teams: Online Banking Team

![image](https://github.com/user-attachments/assets/57a3042e-aab8-4c3e-beec-a4b32c9e36b2)

•	Under Admin Panel – Click Agents – Add New
•	Create New Agent – osTicket 
•	Under Account: John Doe – email: john@lognpacific.com – password: Password1
•	Under Access: Department: Support – Role: Supreme Admin

![image](https://github.com/user-attachments/assets/eb8670ae-760c-4554-9aac-e39f3435b4ed)

Step 7. Configure Users (Customers)
•	Under Agent Panel – Click Users – Click Add New User – OsTicket User
•	Name: Karen – email: Karen@lognpacific.com
•	Name: Ken – email: Ken@lognpacific.com 

![image](https://github.com/user-attachments/assets/b181dea9-6742-408c-9a4e-08494ecd2b3b)
![image](https://github.com/user-attachments/assets/6761efea-5ba5-4892-be2b-8e70534a85cc)

Step 8. Configure SLA (Service Level Agreement)
•	Under Admin Panel – click Manage – Click SLA – Click Add New SLA Plan
•	Sev-A (Grace Period 1 hour. Schedule 24/7)
•	Sev-B (Grace Period 4 hours. Schedule 24/7)
•	Sev-C (Grace Period 8 hours. Schedule 24/7 business hours)

![image](https://github.com/user-attachments/assets/5f17c660-1168-4521-88bb-70c1d9d2a6f7)
![image](https://github.com/user-attachments/assets/e4e513da-d61c-4580-971b-125ff1f48ee0)

Step 9. Configure Help Topics
•	Used for Users to create a ticket
•	Under Admin – click Manage – click Help Topics 
•	Create Several Help Topics
•	Business Critical Outage
•	Personal Computer Issues
•	Password Reset 

![image](https://github.com/user-attachments/assets/85df0f40-e42d-46e9-80c1-3701026e8c58)
![image](https://github.com/user-attachments/assets/78ea43b4-5b2f-40bb-bb18-6f715dcf634e)






