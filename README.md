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

- Enable IIS
- Install Web Platform Installer
- Install MySQL and setup username and password
- Install Microsoft Visual C++ 2009 Redistributable Package
- Configure permissions and install osTicket

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/zal6veX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>
<p>
You’ll be starting this project on a Virtual Machine using Microsoft Azure. Here we have the VM spun up.
</p>
<br />

<p>
<img src="https://i.imgur.com/oZQTFw8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now you’ll connect to the VM remotely using Microsoft Remote Desktop 
</p>
<br />

<p>
<img src="https://i.imgur.com/gX2n5Dv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once you’ve got Windows 10 open, head over to the Control Panel and click “Uninstall a program” underneath Program. On the left you’ll see “Turn Windows features on or off”. Click this and the window above will pop up. Select “Internet Information Services” (ISS) and click okay.
</p>
<br />

<p>
<img src="https://i.imgur.com/ahaMYKm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download and install Microsoft Web Platform 5.1
</p>
<br />

<p>
<img src="https://i.imgur.com/oMf0oig.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Launch Microsoft Web Platform 5.1 and add MySQL Windows 5.5
</p>
<br />

<p>
<img src="https://i.imgur.com/sDo9FjD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next, search for “php” and sort the list to make it easier to select the necessary versions. Add PHP 5.6.31, 7.0.33(x86), 7.1.29(x86), 7.2.26(x86), and 7.3.25(x86). There should be 12 items to install. Click install.
</p>
<br />

<p>
<img src="https://i.imgur.com/2e3MII3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
You’ll be asked to create a password for MySQL. The user will be “root”. Write down the password twice and don’t forget it. Click continue.
</p>
<br />

<p>
<img src="https://i.imgur.com/mRniTA5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once the installation completes, you’ll notice a few things failed and that’s okay. We will install those next.
</p>
<br />

<p>
<img src="https://i.imgur.com/Lkxsldh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download Microsoft Visual C++ 2008 (vcredist_x86) and PHPManagerForIIS_V1.5.0
</p>
<br />

<p>
<img src="https://i.imgur.com/jYUUuJ7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install Microsoft Visual C++ 2008 (vcredist_x86)
</p>
<br />

<p>
<img src="https://i.imgur.com/2vVx8pO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install PHP Manager
</p>
<br />

<p>
<img src="https://i.imgur.com/KI85cGV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download and extract osTicket-v1.15.8
</p>
<br />

<p>
<img src="https://i.imgur.com/52YbM64.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After extracting, copy the upload folder.
</p>
<br />

<p>
<img src="https://i.imgur.com/alzXpo8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Paste the “upload” folder to This PC > Windows (C:) > inetpub > wwwroot
</p>
<br />

<p>
<img src="https://i.imgur.com/6mTFLut.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Rename the “upload” folder to “osTicket”
</p>
<br />

<p>
<img src="https://i.imgur.com/glp9LTe.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open up IIS. You can search for it in the search bar on the bottom left. On the right side of the window, click “restart”.
</p>
<br />

<p>
<img src="https://i.imgur.com/AwHv4ta.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
On the left, open the drop down vm-osticket > Sites > Default Web Site > osTicket. Select osTicket and on the right side of the window, click “Browse *:80 (http)”
</p>
<br />

<p>
<img src="https://i.imgur.com/CGuJDNk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
The browser should open with osTicket Installer.
</p>
<br />

<p>
<img src="https://i.imgur.com/jHvdLNv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open IIS Manager again and click PHP Manager.
</p>
<br />

<p>
<img src="https://i.imgur.com/6AjT21A.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click “Enable or disable an extension” on the bottom
</p>
<br />

<p>
<img src="https://i.imgur.com/IaO37s3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Right click and enable php_intl.dll
</p>
<br />

<p>
<img src="https://i.imgur.com/cSxaw13.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Make sure php_imap.dll is enabled.
</p>
<br />

<p>
<img src="https://i.imgur.com/6R8DEdw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Enable php_opcache.dll
</p>
<br />

<p>
<img src="https://i.imgur.com/IjLJn53.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Refresh the browser and observe the changes.
</p>
<br />

<p>
<img src="https://i.imgur.com/ZOaIWaH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Changes made.
</p>
<br />

<p>
<img src="https://i.imgur.com/BuxGKBe.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Navigate to the folder: This PC > Windows (C:) > inetpub › wwwroot > oslicket > include. Find and rename “ost-sampleconfig.php” to “ost-config.php”. Make sure the spelling is correct.
</p>
<br />

<p>
<img src="https://i.imgur.com/VAKeQRB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Disable the inheritance of the ost-config.php file.
</p>
<br />

<p>
<img src="https://i.imgur.com/XxCwwSi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Select principal and allow “Everyone”.
</p>
<br />

<p>
<img src="https://i.imgur.com/yEGovZG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Allow all permissions.
</p>
<br />

<p>
<img src="https://i.imgur.com/sgawatV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click continue on osTicket and you’ll see “osTicket Basic Installation”.
</p>
<br />

<p>
<img src="https://i.imgur.com/QYaNgsY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Fill in the info. The email addresses will need to be different.
</p>
<br />

<p>
<img src="https://i.imgur.com/mBG83fM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Download and install HeidiSQL 12.0.0.6468.

</p>
<br />

<p>
<img src="https://i.imgur.com/g32SSAW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create a new connection and use the password you created with MySQL. Remember the user was “root”. Click open.
</p>
<br />

<p>
<img src="https://i.imgur.com/oIOvqLh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now create a new database.
</p>
<br />

<p>
<img src="https://i.imgur.com/huwXby8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
I went ahead and named it osticket to keep things simple.
</p>
<br />

<p>
<img src="https://i.imgur.com/wrL9yMS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Navigate back to the browser and osTicket Basic Installation and input the database name, root user, and the password created with MySQL.
</p>
<br />

<p>
<img src="https://i.imgur.com/CBTUHUg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click Install to finish the process. Congratulations!
</p>
<br />

<p>
<img src="https://i.imgur.com/mrevCZl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now let’s navigate back to delete the setup folder, otherwise osTicket will bug you with alerts to setup.
</p>
<br />

<p>
<img src="https://i.imgur.com/U7NNFhS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Delete the contents of the setup folder to be able to delete the actual folder.
</p>
<br />

<p>
<img src="https://i.imgur.com/rWtGVEC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Navigate back to the ost-config.php file and change its permissions to “Read and execute” and “Read”. Don’t forget to apply the changes before hitting okay.
</p>
<br />

<p>
<img src="https://i.imgur.com/Wd9ScQL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Head back to the browser with osTicket and open a new tab with the link underneath “Your Staff Control Panel”.
</p>
<br />

<p>
<img src="https://i.imgur.com/feGq0Fx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Login with the username and password you chose during the installation of osTicket.
</p>
<br />

<p>
<img src="https://i.imgur.com/7mAzrXp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This is how the application should look like after initial log in. Congratulations on installing osTicket!
</p>
<br />
