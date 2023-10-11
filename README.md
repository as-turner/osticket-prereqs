<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com/watch?v=dEvGaxOgqf0)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- PHP Manager For IIS
- Rewrite Module
- PHP 7.3.8
- Microsoft Visual C++ Redistributable
- MYSQL 5.5.62
- HeidiSQL

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Create a Resource Group
- Create a Virtual Machine
- Create a file on your local desktop and upload it into the Storage Account
- Edit the file within the Storage Account (within the Azure Portal)
- Download the file and observe the changes

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/cW13zor.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>
<p>
1. Navigate to Azure portal

2. Click Resource groups

3.  Click "+ Create" to create a new Resource Group

4. Select the Subscription from the drop down menu

5. Name the new Resource group

6. Select the Region. Even though you choose a region for your resource group, the resources that you put into it don't all have to be in that region!

7. Click "Next : Tags >"

8. Add Tags (optional)

9. Click "Next: Review + create >"

10. Click Create
</p>
<br />

<p>
<img src="https://i.imgur.com/Qw0QdOt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

1. Enter virtual machines in the search.
   
2. Under Services, select Virtual machines.
   
3. In the Virtual machines page, select Create and then Azure virtual machine. The Create a virtual machine page opens.
   
4. Under Instance details, enter myVM for the Virtual machine name and choose Windows Server 2022 Datacenter: Azure Edition - x64 Gen 2 for the Image. Leave the other defaults.

5. Under Administrator account, provide a username, such as azureuser and a password. The password must be at least 12 characters long and meet the defined complexity requirements.

6. Under Inbound port rules, choose Allow selected ports and then select RDP (3389) and HTTP (80) from the drop-down.

7. Leave the remaining defaults and then select the Review + create button at the bottom of the page.

8. After validation runs, select the Create button at the bottom of the page.

9. After deployment is complete, select Go to resource.

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
