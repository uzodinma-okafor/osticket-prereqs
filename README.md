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
<h2>Step 9: Enable PHP in IIS </h2>
<img src="https://i.imgur.com/TpTuKGJ.png" height="50%" width="33%" alt="Disk Sanitization Steps"/> <img src="https://i.imgur.com/mjpomq4.png" height="50%" width="33%" alt="Disk Sanitization Steps"/> <img src="https://i.imgur.com/2dQ5Y8B.png" height="50%" width="33%" alt="Disk Sanitization Steps"/><img src="https://i.imgur.com/TjU4bIC.png" height="50%" width="33%" alt="Disk Sanitization Steps"/>
</p>
<p>
- Go to Search next to Start>> Type "IIS" >> When IIS comes up in search, scroll below its heading and select "Run as administrator"
 
 - In IIS, click "PHP Manager" >> Under PHP Setup, click "Register New PHP Session"
 - In next pop-up window, click "..." to find to the "php-cgi.exe" executable file required. It's in the C:\PHP folder created earlier. (Make sure to select "PHP executable" before clicking "Open"!)
 - Click "OK"  
 - Restart IIS by going back to its home page and click "Restart" on the top right side
</p>
<br /><hr>

<p>
<h2>Step 10: Install osTicket v1.15.8 </h2>
<img src="https://i.imgur.com/beXK3tM.png" height="50%" width="33%" alt="Disk Sanitization Steps"/> <img src="https://i.imgur.com/CdHdmcg.png" height="50%" width="33%" alt="Disk Sanitization Steps"/> 
</p>
<p>
- Download osTicket v1.15.8 from the Installation Files Folder

  - Open the zip folder >> Extract and copy “upload” folder to c:\inetpub\wwwroot
  - Within c:\inetpub\wwwroot, Rename “upload” folder to “osTicket”
  - Reload IIS by going to its home page and click "Restart" on the top right side
  
</p>
<br /><hr>

<p>
<h2>Step 11: Enable PHP extensions in PHP Manager </h2>
<img src="https://i.imgur.com/F2DYgmS.png" height="50%" width="33%" alt="Disk Sanitization Steps"/> <img src="https://i.imgur.com/2ZVuPlA.png" height="50%" width="33%" alt="Disk Sanitization Steps"/> 
</p>
<p>
- On left sidebar panel of IIS, Go to sites -> Default -> osTicket
 
 - On the right, click “Browse *:80” >> Note: on the webpage, there are some extensions not enabled
 - Go back to IIS>> on the left sidebar move to sites -> Default -> osTicket
 - Double-click PHP Manager >> Click “Enable or disable an extension”
 - Enable these extensions: php_imap.dll, php_intl.dll, and php_opcache.dll
 - Refresh the OsTicket site and notice the changes due to the enabled extensions
  
</p>
<br /><hr>

<p>
<h2>Step 12: Rename & Assign permissions for ost-config.php </h2>
<img src="https://i.imgur.com/08urZO5.png" height="50%" width="33%" alt="Disk Sanitization Steps"/> <img src="https://i.imgur.com/An9jSTD.png" height="50%" width="33%" alt="Disk Sanitization Steps"/> 
</p>
<p>
- Rename from "C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php" to "C:\inetpub\wwwroot\osTicket\include\ost-config.php"
 
- Next, right click "ost-config.php" >> select Properties >> Click on Security tab >> Click "Advanced" 
- Click "Disable inheritance" >> Click "Remove All..." >> Click "Add" 
- On new window, click "select a principal" >> In Permissions window, type "Everyone" and click OK
- In next permission window, Select checkbox for "Full Control" >> Click OK >> back in previous window, click Apply and then click OK
- Click OK a final time to close ost-config.php Properties

</p>
<br /><hr>

<p>
<h2>Step 13: OsTicket Setup Continued </h2>
<img src="https://i.imgur.com/tNhAeHI.png" height="50%" width="33%" alt="Disk Sanitization Steps"/> <img src="https://i.imgur.com/IukDV9g.png" height="50%" width="33%" alt="Disk Sanitization Steps"/> 
</p>
<p>
- Refresh OsTicket Installer page >> There are more features now. >> Click "Continue"
 
- New page require information to be filled out. 
- Focusing on the "system Settings" and "Admin User" sections, fill out those details. Feel free to use example username and passwords in the pic above this step. Just use non-personal testing email addresses. 
 - Pic Example (HelpDesk Name: Din Help Desk, Admin Username: Din, Admin Password: Machine321virt)
 
</p>
<br /><hr>

<p>
<h2>Step 14: Install HeidiSQL </h2>
<img src="https://i.imgur.com/ODtuVGu.png" height="50%" width="33%" alt="Disk Sanitization Steps"/><img src="https://i.imgur.com/VsBBgVk.png" height="50%" width="33%" alt="Disk Sanitization Steps"/><img src="https://i.imgur.com/Za7GvcH.png" height="50%" width="33%" alt="Disk Sanitization Steps"/>
</p>
<p>
- Download MS Word document from the Google Drive Installation Files page >> click on link in the MS Word doc >> Download the ".exe" file for HeidiSQL

- Click "Open File" in Downloads >> select "I accept..." and click Next >>Click Next 3x times, then click Install >> Click Finish
- Close any pop-up window that asks to make updates to HeidiSQL
- HeidiSQL will launch and open up its session manager>> Click on down arrow on "New" button and select "Session in root folder"
- You'll be prompted to put password for your MySQL root account, which set up earlier to be "Password1" >> Click Open
- In new window, right click main branch in left sidebar >> select Creat New >> select Database >> name new database "osTicket", and click OK

</p>
<br /><hr>

<p>
<h2>Step 15: OsTicket setup continued </h2>
<img src="https://i.imgur.com/zmGN1cV.png" height="50%" width="33%" alt="Disk Sanitization Steps"/> <img src="https://i.imgur.com/ZsIn34k.png" height="50%" width="33%" alt="Disk Sanitization Steps"/> 
</p>
<p>
- Finish filling out Database settings on OsTicket Installer page (just like 1st pic above) and click "Install Now"
 
- Congrats! If you followed these steps right so far, you should see the 2nd pic above.
 - You can browse to your help desk login page with this link: http://localhost/osTicket/scp/login.php
 - End users of osTicket should be able to send tickets to your helpdesk with this link:http://localhost/osTicket/ 
</p>
<br /><hr>

<p>
<h2>Step 16: Clean up: delete "setup" folder </h2>
<img src="https://i.imgur.com/XW7tc7v.png" height="50%" width="33%" alt="Disk Sanitization Steps"/><img src="https://i.imgur.com/63GylNv.png" height="50%" width="33%" alt="Disk Sanitization Steps"/>
</p>
<p>
- Delete this folder--> C:\inetpub\wwwroot\osTicket\setup
  
- Next, right click on C:\inetpub\wwwroot\osTicket\include\ost-config.php >> select Properties >> Click on Security tab >> Click "Advanced"
- Double Click on "Everyone" >> Uncheck all boxes EXCEPT "Read" and "Read and Execute" >> Click OK >> On previous window, Click "Apply", then click "OK"
- Click OK a final time
  
</p>
<br /><hr>
