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
<h2>Step 1: Enable IIS in Windows with CGI</h2>
<img src="https://i.imgur.com/S8lrjzX.png" height="50%" width="33%" alt="Disk Sanitization Steps"/><img src="https://i.imgur.com/kzRHI9k.png" height="50%" width="33%" alt="Disk Sanitization Steps"/><img src="https://i.imgur.com/sw6QGNa.png" height="50%" width="33%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h3>Step 1: Enable IIS in Windows with CGI</h3>

- Click into the search bar next to Start >> Type in "Control" and select Control Panel.
  - Choose "Programs" >> Click "Turn Windows Features on or Off"
  - Scroll down to activate "Internet Information Services (IIS)" by checking its box on the left
  - Expand IIS to reach "World Wide Web Services" >> Expand that to reach "Application Development Features" >> Expand that, scroll down and activate "CGI" by clicking the box on its left
  - Click OK
</p>
<br/><hr>

<p>
<h2>Step 2: Get access to files for installation</h2>
<img src="https://i.imgur.com/vAheUwX.png" height="50%" width="33%" alt="Disk Sanitization Steps"/>
</p>
<p>
- Go to Microsoft Edge >> skip any personalization or marketing ads and open a new tab>> use this <a href="https://drive.google.com/drive/u/1/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6">link</a> to access prerequisite installation files
</p>
<br /><hr>

<p>
<h2>Step 3: Create C:\PHP Folder </h2>
<img src="https://i.imgur.com/XgkgOBC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
- Open Windows Exlorer in the taskbar

  - Click on "This PC" on left sidebar >> Go to and the Windows (C:\) drive >> Right click, select "New", then select "New Folder" >> Rename the new folder "PHP"
</p>
<br /><hr>

<p>
<h2>Step 4: Intstall PHP Manager </h2>
<img src="https://i.imgur.com/flUt8iT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/><img src="https://i.imgur.com/mt6FA0C.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
- Download and install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi)

  - Click & download PHPManagerForIIS_V1.5.0.msi (If you receive an message saying, "this file type might be dangerous", click to "download anyway"; Be sure to do this for ALL file downloads if necessary.)
  - After downloading, click "Open File" to start installation of the file
  - Click "Next", then choose "I Agree" and click "Next" again
  - After installation completes, click "Close"
</p>
<br /><hr>

<p>
<h2>Step 5: Intstall Rewrite Module </h2>
<img src="https://i.imgur.com/M4dgnEX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
- Download and install the Rewrite Module (rewrite_amd64_en-US.msi)

  - After downloading, click "Open File" to start installation of the file
  - Check the "I Agree" box and click "Next" 
  - After installation completes, click "Finish"
</p>
<br /><hr>

<p>
 <h2>Step 6: Install PHP 7.3.8</h2>
<img src="https://i.imgur.com/ap7nxgJ.png" height="50%" width="50%" alt="Disk Sanitization Steps"/><img src="https://i.imgur.com/bfARSTG.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
- After downloading the zip file, move its contents into your new C:\PHP folder

  - Right click inside the zip file, choose "Extract All"
  - Click "Browse" and choose C:\PHP as your destination folder
  - Click "Extract" and then verify the contents moved are in the C:\PHP folder
</p>
<br /><hr>

<p>
<h2>Step 7: Intstall Microsoft Visual C++ </h2>
<img src="https://i.imgur.com/HlS0Bm0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
- Download VC_redist.x86.exe to install Microsoft Visual C++

  - After downloading, click "Open File" to start installation of the file
  - Check the "I Agree" box and click "Install" 
  - After installation completes, click "Close"
</p>
<br /><hr>

<p>
<h2>Step 8: Intstall MySQL Server 5.5.62 </h2>
<img src="https://i.imgur.com/M58yw2o.png" height="50%" width="33%" alt="Disk Sanitization Steps"/> <img src="https://i.imgur.com/QFUOmG8.png" height="50%" width="33%" alt="Disk Sanitization Steps"/> <img src="https://i.imgur.com/xiY7per.png" height="50%" width="33%" alt="Disk Sanitization Steps"/>
</p>
<p>
- Download and install MySQL 5.5.62 (mysql-5.5.62-win32.msi)
 
 - After downloading, click "Open File" to start installation of the file
 - Click Next >> Check the "I Agree" box and click "Next" 
 - Choose "Typical" Setup type, then click "Next" 
 - CLick "Install", then click "Finish"
 - Choose "Standard Configuration", then click "Next" >> Leave "Install As Windows Service" choice AS IS and click "Next"
 - Make new password like "Password1" for root MySQL Server account, then click "Next"
 - Click "Execute" >> Click "Finish"
  
</p>
<br /><hr>


<p>
<h2>Step 8: Enable PHP in IIS </h2>
<img src="https://i.imgur.com/TpTuKGJ.png" height="50%" width="33%" alt="Disk Sanitization Steps"/> <img src="https://i.imgur.com/mjpomq4.png" height="50%" width="33%" alt="Disk Sanitization Steps"/> <img src="https://i.imgur.com/2dQ5Y8B.png" height="50%" width="33%" alt="Disk Sanitization Steps"/>
</p>
<p>
- Go to Search next to Start>> Type "IIS" >> When IIS comes up in search, scroll below its heading and select "Run as administrator"
 
 - In IIS, click "PHP Manager" >> Under PHP Setup, click "Register New PHP Session"
 - In next pop-up window, click "..." to find to the "php-cgi.exe" executable file required. It's in the C:\PHP folder created earlier. (Make sure to select "PHP executable" before clicking "Open"!)
 - Click "OK"  
 - Choose "Typical" Setup type, then click "Next" 
 - CLick "Install", then click "Finish"
 - Choose "Standard Configuration", then click "Next" >> Leave "Install As Windows Service" choice AS IS and click "Next"
 - Make new password like "Password1" for root MySQL Server account, then click "Next"
 - Click "Execute" >> Click "Finish"
  
</p>
<br /><hr>
