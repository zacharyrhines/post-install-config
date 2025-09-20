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
<img width="80%" height="80%" alt="OSTickPost1" src="https://github.com/user-attachments/assets/f92e5d52-8dfb-4922-b0a9-c784b948e7e6" />
</p>

<p>
<img width="80%" height="80%" alt="OSTickPost2" src="https://github.com/user-attachments/assets/8041b321-8d17-4f82-8079-ce0a169717d8" />
</p>

<h3>3.) Configure Departments</h3>

- Navigate to **Admin Panel -> Agents -> Departments**.
- Add a new department called **SysAdmins**.
  - Use departments to control ticket visibility and assign areas of responsibility (e.g., Help Desk, SysAdmins, Networking).

<p>
<img width="80%" height="80%" alt="OSTickLifecycle6" src="https://github.com/user-attachments/assets/73321974-f84a-4393-82c1-0c270ca8dd1c" />
</p>

<h3>4.) Configure Teams</h3>

- Navigate to **Admin Panel -> Agents -> Teams**.
- Create a new team called **Online Banking**.
  - Pull agents from different departments to form specialized teams.

<p>
<img width="80%" height="80%" alt="OSTickPostIntall1" src="https://github.com/user-attachments/assets/e3b427fa-ec3c-4876-8963-102f1ba33b33" />
</p>

<h3>5.) Allow Anyone to Create Tickets</h3>

- Navigate to **Admin Panel -> Settings -> User Settings**.
- Uncheck **Require registration and login to create tickets** to enforce ticket creation by anyone.
- Enable **Public - Anyone can register** to disable requiring users to register and log in before creating tickets.

<p>
<img width="80%" height="80%" alt="OSTickPostIntall2" src="https://github.com/user-attachments/assets/5c905574-d965-438b-add3-6986bee0d0f9" />
</p>

<h3>6.) Configure Agents (Workers)</h3>

- Navigate to **Admin Panel -> Agents -> Add New**.
- Add agents with the following details:
  - **Jane**: Assigned to the **SysAdmins** department.
  - **John**: Assigned to the **Support** department.

<p>
<img width="80%" height="80%" alt="OSTickPostIntall3" src="https://github.com/user-attachments/assets/0a295d87-bccd-4495-a231-64d3c5ef3aa6" />
</p>

<p>
<img width="80%" height="80%" alt="OSTickPostIntall4" src="https://github.com/user-attachments/assets/bf587395-9dd5-4b15-882e-b8c2bc2535d7" />
</p>

<p>
<img width="80%" height="80%" alt="OSTickPostIntall5" src="https://github.com/user-attachments/assets/b63e893d-4ce3-48ea-b2f3-d4d12684c754" />
</p>

<h3>7.) Configure Users (Customers)</h3>

- Navigate to **Agent Panel -> Users -> Add New**.
- Add users with the following details:
  - **Karen**
  - **Ken**
 
<p>
<img width="80%" height="80%" alt="OSTickPostIntall6" src="https://github.com/user-attachments/assets/d30d00ec-c2a2-4371-b828-d5e1316aa05f" />
</p>

<h3>8.) Configure SLA (Service Level Agreements)</h3>

- Navigate to **Admin Panel -> Manage -> SLA**.
- Add the following SLAs:
  - **Sev-A**: Grace Period = 1 hour, Schedule = 24/7.
  - **Sev-B**: Grace Period = 4 hours, Schedule = 24/7.
  - **Sev-C**: Grace Period = 8 hours, Schedule = Business Hours.

<p>
<img width="80%" height="80%" alt="OSTickPostIntall7" src="https://github.com/user-attachments/assets/b5166f75-e6f3-4dd3-8f6b-c281ceb18de9" />
</p>

<p>
<img width="80%" height="80%" alt="OSTickPostIntall8" src="https://github.com/user-attachments/assets/b7ea4350-f87d-458b-8bde-4a9b0016791d" />
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
<img width="80%" height="80%" alt="OSTickPostIntall9" src="https://github.com/user-attachments/assets/6d02bf82-d2f6-454a-b81a-e5f5d4a2c28e" />
</p>

<h2>Conclusion</h2>

By completing the post-installation configuration steps, you have successfully customized osTicket to suit your organization's requirements. You are now ready to start using osTicket to manage and resolve customer issues efficiently.
