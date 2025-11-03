<h1 align="center">osTicket: Configuration</h1>
<img src="https://miro.medium.com/v2/0*5C2XvKOhIcjjmd7A" height="75%" width="100%"/>
</h1>
This tutorial will guide you through some post-installation tips and configurations for osTicket.
<br/>


<h2>Databases & Programs Used</h2>
<p>
 
- <b>Microsoft Edge</b>

</p>

<h2>Environments Used</h2>
<p>
 
- <b>Windows 10 Enterprise</b> (22H2)
- <b>osTicket</b>

<h2>Prerequisites</h2>

- <b>Windows 10 Enterprise (22H2) virtual machine setup through Azure</b>
- <b>osTicket installed on Windows 10 client with active session open through IIS & HeidiSQL</b>

<h2 align="center">Creating new items in osTicket</h2>

<p>After logging into your osTicket Control Panel as admin, add a new role named "Supreme Admin" by accessing Agents > Roles > Add New Role
<br><img src="https://github.com/user-attachments/assets/4961e43b-8b7f-4920-bcd0-30c33b0696ba" height="75%" width="100%"/>
<br/>

</p>
<p>Provision access to all Tickets permissions to the Supreme Admin role and save changes.
<br><img src="https://github.com/user-attachments/assets/cfda049e-4556-49e7-af10-a91020e33b2e" height="75%" width="100%"/>
<br/>
</p>

<p>Navigate to Agents > Departments and create a new department named "SysAdmins"
<br><img src="https://github.com/user-attachments/assets/60c85b94-661d-4cec-b0ba-4829f0b6e532" height="75%" width="100%"/>
<br/>
</p>

<p>Navigate to Agents > Teams and create a new team named "Store Front"
<br><img src="https://github.com/user-attachments/assets/d2eb42f2-f73b-4c88-a9d4-c0aa79a6c45c" height="75%" width="100%"/>
<br/>
</p>

<p>Navigate to Settings > Users and make sure the registration method is set to "Public -- Anyone can register" under Authentication Settings. (make sure to save changes!)
<br><img src="https://github.com/user-attachments/assets/2b784018-1849-40cd-a836-86bc974d539c" height="75%" width="100%"/>
<br/>
</p>

<p>Create and add two agents from Agents > Agents tab. Ensure that one agent is added to the SysAdmins department and the other to the Support department.
<br><img src="https://github.com/user-attachments/assets/68cb15ae-54c3-4924-bb7b-18c873f85ed1" height="75%" width="100%"/>
<br/>
</p>

<p>Click on "Agent Panel" in the top right corner of the page to access the agent portal. Then create two users from Users > User Directory.
<br><img src="https://github.com/user-attachments/assets/3b84172d-90b6-42b6-9a1a-738941dbefd0" height="75%" width="100%"/>
<br/>
</p>

<p>Return to the Admin Panel by clicking it at the top right corner and create three SLAs with varied Grace Periods and Schedules.
<br><img src="https://github.com/user-attachments/assets/ce1904fb-401a-426d-a29e-2305bc58bc61" height="75%" width="100%"/>
<img src="https://github.com/user-attachments/assets/837b4ea6-d232-4ace-ba58-9e1faa90da3f" height="75%" width="100%"/>
<img src="https://github.com/user-attachments/assets/37683381-7528-49c0-bfa7-18ac9fb06c5e" height="75%" width="100%"/>
<img src="https://github.com/user-attachments/assets/bfce147c-d59b-4ffa-91f1-7e130358babb" height="75%" width="100%"/>
<br/>
</p>

<p>Create some Help Topics from Manage > Help Topics > Add New Help Topic. Here, we created a variety of common account and business end-user issues or requests. Categorize requests and questions in General Inquiry and any problem that needs solving in Report a Problem. All created Help Topics should be directed to the Support department.
<br><img src="https://github.com/user-attachments/assets/90d5089f-abba-49ec-a1e0-a29276fbe460" height="75%" width="100%"/>
<br/>
</p>

You're all set! We've created these users, departments, roles, agents, and SLAs to create mock help desk environment where we can simulate working tickets to completion. Just following these configurations alone with help you understanding the pipeline and lifecycle of tickets, along with learning key access points that you may need to access later should any Panel issues occur.
