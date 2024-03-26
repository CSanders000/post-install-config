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

<h2>Post-Install Configuration Objective</h2>

- Configure osTicket by creating SLA's, roles, departments, teams, agents, users, and help topics.

  <h2>Prerequisites</h2>

  - Complete the installation of osTicket in Azure by following [these instructions](https://github.com/CSanders000/osticket-prereqs)
  - Log into osTicket via our administrator account

<h2>Configuration Steps</h2>

<p>
<img src=https://github.com/CSanders000/post-install-config/assets/161166823/badef148-b46b-4496-bba6-01f2a5fb3755"/>
</p>
<p>
We will start by creating an administrative role. We can name it whatever we want, so in this case we will name it "Supreme Admin". To do this we will make sure we're on the Admin Panel, then go to Agents, Roles, and then create new role. Once we create the role we are going to give this role every permission under the permissions tab. We can then click "Save Changes". 
</p>
<br />

<p>
<img src=https://github.com/CSanders000/post-install-config/assets/161166823/5fe0e38f-283d-43e3-bc44-549d401cacc4"/>
</p>
<p>
Next we will configure our Departments. To do this we will go to Agents, Departments, then add new department. We will name this department System Administrators and then save. 
</p>
<br />

<p>
<img src=https://github.com/CSanders000/post-install-config/assets/161166823/5e53e2a1-3039-447e-a8d2-056dd54f6afc"/>
</p>
<p>
We will next create a team. We can go to Agents, Teams, and then we will name this team "Level II Support". Then we can save changes and create our team. 
</p>
<br />

<p>
<img src=https://github.com/CSanders000/post-install-config/assets/161166823/a680dc74-3e76-48b5-ad43-994e1b66d118"/>
</p>
<p>
Next, we will create our agents. We'll click Agents, Agents, and add new agent. We will add two agents, Jane Doe and John Doe. When creating our agents we will make Jane a System Administrator and John will be in the Support department. When making these accounts; we can name them both, give them a fake email (ex. jane.doe@osticket.com), make their usernames something simple (ex. jane.doe), and then give them passwords. We'll uncheck the "Send the agent a password reset email" box to give them a password, then we will uncheck the "Request password change at next login" box. It is also important to assign them to a department and a role. Jane will be a System Administrator with the Supreme Admin role. We will also give her a secondary department in Support with a Supreme Admin Role. For John, we will just give him a Support role with expanded permissions (so he is able to close tickets).
</p>
<br />

<p>
<img src=https://github.com/CSanders000/post-install-config/assets/161166823/1f670306-fe8b-40e8-b2c2-aa80b613f08b"/>
</p>
<p>
Next, we wll create some users. For this we will switch to the agent panel in the top right, then go to Users and User Directory. We will add three users. Amanda Smitch, Ken James, and Ryan Johnson. To do this we will click "Add User", give them a name and email, and then save changes. 
</p>
<br />

<p>
<img src=https://github.com/CSanders000/post-install-config/assets/161166823/6ae1c9d8-7341-47be-ab83-129d1106ae39"/>
</p>
<p>
We will create three SLA plans, each of a different severity. To do this we will go back to the admin panel, then go to Manage, and then SLA. We will create "Sev-A", which will have a grace period of 1 hour and a schedule of 24/7. Then click "Add Plan" at the bottom. Sev-B will have a grace period of 4 hours and will also have a schedule of 24/7. Sec-C will be our least urgent SLA plan and will have a grace period of 8 hours and will be scheduled for "Monday - Friday 8am - 5pm with U.S. Holidays". 
</p>
<br />

<p>
<img src=https://github.com/CSanders000/post-install-config/assets/161166823/b012ce9a-9ea8-420c-be04-ec24fad0d448"/>
</p>
<p>
Finally, we will add out Help Topics. To get here we will click "Manage" and then "Help Topics". We will be adding four help topics, named Business Critical Outage, Equipment Reset, Password Reset, and Personal Computer Issues. All we have to do here is click "Add New Help Topic", name it, and then click save changes. That concludes the configuration of osTicket. 
</p>
<br />



