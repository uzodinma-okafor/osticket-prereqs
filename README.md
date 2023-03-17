<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computers)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Internet Information Services (IIS) with CGI 
- PHP Manager for IIS
- Rewrite Module
- C:/PHP directory 
- PHP 7.3.8 
- Microsoft Visual C++ 
- MySQL 5.5.62

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/uPkkeVX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/8X8C6by.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    <img src="https://i.imgur.com/KtjRszO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To follow along in this tutorial, first create your own virtual machine (VM) in Azure with this previous tutorial, <a href="https://github.com/uzodinma-okafor/vm-creation">Creation of a Virtual Machine via Microsoft Azure</a>. Make sure to create your login credentials (username and password), to use Windows 10 Pro as the OS, & to use 4 vCPUs with a low monthly cost for your VM (pics# 2-4 down). The resource group for this tutorial is RG_OST_3. The VM used in this tutorial is VM-OST-3. For the VM's login credentials, I used the username "labuserdin" and "Virtual123mach" as my password. In VM-OST-3, I complete the steps for installation for osTicket.
</p><hr>
<br />

<p>
<img src="https://i.imgur.com/X2JizIf.png" height="50%" width="33%" alt="Disk Sanitization Steps"/><img src="https://i.imgur.com/IFKF7mk.png" height="50%" width="33%" alt="Disk Sanitization Steps"/><img src="https://i.imgur.com/vAheUwX.png" height="50%" width="33%" alt="Disk Sanitization Steps"/>
</p>
<p>
As seen above(left pic), VM-OST-3 is all set up. I copied VM-OST-3's public IP address (172.174.137.146). I'm connnecting and logging into it via Remote Desktop Connection to continue the steps of installation. To follow along with this part of the  tutorial, connect to your own virtual machine (VM) by following the steps in this previous tutorial, <a href="https://github.com/uzodinma-okafor/vm-connection">Connecting to & Utilization of Virtual Machines via Microsoft Remote Desktop Connection</a>. After logging into VM-OST-3 (middle pic), I went on Microsoft Edge to log into Google Drive to open a folder with the necessary prerequisite installation files(right pic).
</p><hr>
<br />


<p>
<h2>Enable IIS in Windows with CGI</h2>
<img src="https://i.imgur.com/S8lrjzX.png" height="50%" width="50%" alt="Disk Sanitization Steps"/><img src="https://i.imgur.com/kzRHI9k.png" height="50%" width="50%" alt="Disk Sanitization Steps"/><img src="https://i.imgur.com/sw6QGNa.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h3>Step 1: Enable IIS in Windows with CGI</h3>

- Click into the search bar next to Start >> Type in "Control" and select Control Panel.
  - Choose "Programs" >> Click "Turn Windows Features on or Off"
  - Scroll down to activate "Internet Information Services (IIS)" by checking its box on the left
  - Expand IIS to reach "World Wide Web Services" >> Expand that to reach "Application Development Features" >> Expand that, scroll down and activate "CGI" by clicking the box on its left
  - CLick OK

</p><hr>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
