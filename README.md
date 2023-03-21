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

- Step 1: Configuration of Roles
- Step 2: Configuration of Departments
- Step 3: Configuration of Teams
- Step 4: Adjusting Settings To Allow Ticket Creation By Anyone
- Step 5: Configuration of Agents (i.e. employees)
- Step 6: Configuration of Users (i.e. clients/customers)
- Step 7: Configuration of Service Level Argreements (SLAs)
- Step 8: Configuration of Help Topics

<h2>Configuration Steps</h2>

<p>
<h2>Step 1: Configuration of Roles</h2>
<img src="https://i.imgur.com/fKfLfv7.png" height="50%" width="50%" alt="Disk Sanitization Steps"/><img src="https://i.imgur.com/YPR3Y6K.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
- Start this part of the overall osTicket tutorial by logging into your help desk login page via this link: http://localhost/osTicket/scp/login.php (Make sure you get through last part of this tutorial, <a href="https://github.com/uzodinma-okafor/osticket-prereqs">osTicket: Prerequisites and Installation</a>, in order to follow along.)

- You should be in the Admin Panel after logging in. If not, click "Admin Panel" on top right corner of page. NOTE: "Agent Panel" will show in top right menu whenever you're in the "Admin Panel" and vice versa. This is how you move between both panels.
- Click on "Agents" tab in upper menu, then click on Roles in the lower menu.
- Click on "Add New Role" just above "Last Updated" column of the list of existing roles. NOTE: This feature is used to create as many Roles needed for the organization. The Roles are set up according to what access levels each group of members needs depending upon their departments and abilities to assign or close tickets etc.
- Make a new role and label it "Supreme Admin" in Definition Tab. Then, go to Permissions Tab to give it all permissions in the subtabs, Tickets, Tasks, & Knowledgebase. 
- Click "Save Changes" to add the role to list of existing roles.
</p>
<br /><hr>

<p>
<h2>Step 2: Configuration of Departments</h2>
<img src="https://i.imgur.com/iSikp3Z.png" height="50%" width="50%" alt="Disk Sanitization Steps"/><img src="https://i.imgur.com/6peR3NL.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
- In this step, you're going to make a new department.

- Click "Admin Panel" on top right corner of page
- Click on "Agents"tab, then click on "Departments"
- Click on "Add New Department" just above "Created" column of the list of existing departments. From here (2nd pic), choose the appropriate settings that will apply to the access levels for this department. The "Departments" have many different settings which apply to tickets as they are routed through the departments, and determine the visibility as well as whether tickets can be routed to each department.

- Make a new department and label it "System Administrators".
- Click "Create Dept" when you're finished configuring the settings according to your preference.
</p>
<br /><hr>

<p>
<h2>Step 3: Configuration of Teams</h2>
<img src="https://i.imgur.com/i84VlAw.png" height="50%" width="50%" alt="Disk Sanitization Steps"/><img src="https://i.imgur.com/4lCzRYE.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
- In this step, you're going to make new teams.

- Click "Admin Panel" on top right corner of page
- Click on "Agents"tab, then click on "Teams"
- Click on "Add New Team" above the teams already set up in top right area
- Make a new team and label it "Level II Support". On this page (2nd pic), choose the appropriate members for the team and set the access levels that will apply. Configuring Teams will allow Agents from different Departments to be organized to solve a specific issue or help a specific user via a Help Topic or Ticket Filter, regardless of the Agents' Department rules.
- Click "Create Team" to save the new team to existing list of teams.
</p>
<br /><hr>

<p>
<h2>Step 4: Adjusting Settings To Allow Ticket Creation By Anyone</h2>
<img src="https://i.imgur.com/FqN4pjB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
- In this step, you're going to adjust settings to allow anyone to make tickets.

- Click "Admin Panel" on top right corner of page>> Go to Settings >> Click User Settings
- In the checkbox section that reads "Registration Required: Require registration and login to create tickets", leave the box unchecked. THis will allow for anyone to anonymously create tickets.

</p>
<br /><hr>

<p>
<h2>Step 5: Configuration of Agents (i.e. employees)</h2>
<img src="https://i.imgur.com/fXEahj4.png" height="50%" width="50%" alt="Disk Sanitization Steps"/><img src="https://i.imgur.com/6b5L1aI.png" height="50%" width="50%" alt="Disk Sanitization Steps"/></p>
<p>
- In this step, you're going to configure accounts for 2 new agents (i.e. workers).

- Click "Admin Panel" on top right corner of page>> Go to "Agents" >> Click "Add New"
- NOTE: Agents are given access to the help desk with the intent to respond and resolve the tickets. When an Agent is added to the help desk, they should be assigned to a Primary Department and given a Primary Role any Tickets or Tasks sent to that department. 
- Make a new account for "Jane Doe" with username "jane.doe" and password "Password1". Make sure leave "passwrod rest email" and "require password change at next login" options UNCHECKED with setting up the password. Add Jane to the "System Administrators" dept as a "Supreme Admin" in the "Access" Tab. Also, add her to the Level II Support team in the "Teams" Tab. Then, click "Create" at the bottom.
- Get back to the "Agents" page you were previously on and repeat the process again to make an account for "John Doe" with username "john.doe" and same password. Add John to the "Support" dept in a "View Only" role in the "Access" Tab.
</p>
<br /><hr>

<p>
<h2>Step 6: Configuration of Users (i.e. clients/customers)</h2>
<img src="https://i.imgur.com/BhwNddr.png" height="50%" width="50%" alt="Disk Sanitization Steps"/><img src="https://i.imgur.com/GPbyUwR.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
- In this step, you're going to configure accounts for 2 new users (i.e. customers).

- Click "Agent Panel" on top right corner of page>> Go to "Users" >> Click "User Directory" >> Click "Add New". NOTE: When you see "Admin Panel" in top right of page, you're in "Agent Panel" and vice versa.
- Make a new account for "Karen Karen" with email "karen@osticket.com" and password "Password1". Then click "Add user".
- Get back to the "Agents" page you were previously on and repeat the process again to make an account for "Ken Ken" with email "ken@osticket.com" and same password.
</p>
<br /><hr>

<p>
<h2>Step 7: Configuration of Service Level Argreements (SLAs)</h2>
<img src="https://i.imgur.com/oLwZoFC.png" height="50%" width="50%" alt="Disk Sanitization Steps"/><img src="https://i.imgur.com/sdyBVrj.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>

</p>
<p>
- In this step, you're going to configure new SLAs for responding to tickets.

- Click "Admin Panel" on top right corner of page>> Go to "Manage" >> Click "SLA">> Click "Add New"
- Make a new SLA called "SEV-A" with grace period to respond in 1 hour and 24/7 working schedule. Then, Click "Add Plan" at the bottom.
- Get back to the "SLA" page you were previously on and repeat the process again to make a new SLA called "SEV-B" with grace period to respond in 4 hours and 24/7 working schedule.
- Get back to the "SLA" page you were previously on and repeat the process again to make a new SLA called "SEV-C" with grace period to respond in 8 hours and working schedule only during business hours.
<br /><hr>

<p>
<h2>Step 8: Configuration of Help Topics</h2>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
- In this step, you're going to configure new Help Topics for responding to tickets.

- Click "Admin Panel" on top right corner of page>> Go to "Manage" >> Click "Help Topics">> Click "Add New"
- Make a new Help Topic called "Business Critical Outage" >> Click "Create"
- Get back to the "Help Topics" page you were previously on and repeat the process again to make new Help Topics for these categories : Personal Computer Issues, Equipment Request, Password Reset

</p>
<br /><hr>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br /><hr>

