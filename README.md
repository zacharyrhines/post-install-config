<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used</h2>

- Windows 10 (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Acknowledge the difference between the Agent Panel and Admin Panel.
- Configure Roles to define permissions for agents.
- Set up Departments to group tickets by areas of responsibility.
- Create Teams to pull agents from multiple departments.
- Configure user settings to allow or restrict ticket creation.
- Add Agents (workers) and Users (customers).
- Set up Service Level Agreements (SLAs) for ticket response times.
- Create Help Topics for users to categorize their tickets.

<h2>Configuration Steps</h2>

<h3>1.) Acknowledge Agent Panel vs Admin Panel</h3>

- The **Agent Panel** is used by agents to work on tickets.
- The **Admin Panel** is used to manage system settings, configurations, and permissions.

<h3>2.) Configure Roles</h3>

- Navigate to **Admin Panel -> Agents -> Roles**.
- Add a new role called **Supreme Admin**.
  - Define permissions for agents based on the role they will have.

<p>
<img src="https://imgur.com/XAdPoXQ.png" height="80%" width="80%" alt="Step 2 Lab 3"/>
</p>

<p>
<img src="https://imgur.com/CqWKHm4.png" height="80%" width="80%" alt="Step 2 Lab 3"/>
</p>

<h3>3.) Configure Departments</h3>

- Navigate to **Admin Panel -> Agents -> Departments**.
- Add a new department called **SysAdmins**.
  - Use departments to control ticket visibility and assign areas of responsibility (e.g., Help Desk, SysAdmins, Networking).

<p>
<img src="https://imgur.com/aMvPLZ0.png" height="80%" width="80%" alt="Step 2 Lab 3"/>
</p>

<h3>4.) Configure Teams</h3>

- Navigate to **Admin Panel -> Agents -> Teams**.
- Create a new team called **Online Banking**.
  - Pull agents from different departments to form specialized teams.

<p>
<img src="https://imgur.com/nfAhfgy.png" height="80%" width="80%" alt="Step 2 Lab 3"/>
</p>

<h3>5.) Allow Anyone to Create Tickets</h3>

- Navigate to **Admin Panel -> Settings -> User Settings**.
- Uncheck **Require registration and login to create tickets** to enforce ticket creation by anyone.
- Enable **Public - Anyone can register** to disable requiring users to register and log in before creating tickets.

<p>
<img src="https://imgur.com/cy4pG2Z.png" height="80%" width="80%" alt="Step 2 Lab 3"/>
</p>

<h3>6.) Configure Agents (Workers)</h3>

- Navigate to **Admin Panel -> Agents -> Add New**.
- Add agents with the following details:
  - **Jane**: Assigned to the **SysAdmins** department.
  - **John**: Assigned to the **Support** department.

<p>
<img src="https://imgur.com/JfsgQcX.png" height="80%" width="80%" alt="Step 2 Lab 3"/>
</p>

<p>
<img src="https://imgur.com/in2jjvm.png" height="80%" width="80%" alt="Step 2 Lab 3"/>
</p>

<p>
<img src="https://imgur.com/UzIHvtJ.png" height="80%" width="80%" alt="Step 2 Lab 3"/>
</p>

<h3>7.) Configure Users (Customers)</h3>

- Navigate to **Agent Panel -> Users -> Add New**.
- Add users with the following details:
  - **Karen**
  - **Ken**
 
<p>
<img src="https://imgur.com/9SzEQ4p.png" height="80%" width="80%" alt="Step 2 Lab 3"/>
</p>

<h3>8.) Configure SLA (Service Level Agreements)</h3>

- Navigate to **Admin Panel -> Manage -> SLA**.
- Add the following SLAs:
  - **Sev-A**: Grace Period = 1 hour, Schedule = 24/7.
  - **Sev-B**: Grace Period = 4 hours, Schedule = 24/7.
  - **Sev-C**: Grace Period = 8 hours, Schedule = Business Hours.

<p>
<img src="https://imgur.com/QNQMtmC.png" height="80%" width="80%" alt="Step 2 Lab 3"/>
</p>

<p>
<img src="https://imgur.com/XS5xpMb.png" height="80%" width="80%" alt="Step 2 Lab 3"/>
</p>

<h3>9.) Configure Help Topics</h3>

- Navigate to **Admin Panel -> Manage -> Help Topics**.
- Add the following help topics for users to select when creating a ticket:
  - **Business Critical Outage**
  - **Personal Computer Issues**
  - **Equipment Request**
  - **Password Reset**
  - **Other**

<p>
<img src="https://imgur.com/vXYJ7bQ.png" height="80%" width="80%" alt="Step 2 Lab 3"/>
</p>

<h2>Conclusion</h2>

By completing the post-installation configuration steps, you have successfully customized osTicket to suit your organization's requirements. You are now ready to start using osTicket to manage and resolve customer issues efficiently.
