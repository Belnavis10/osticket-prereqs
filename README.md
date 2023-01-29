<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />






<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used</h2>

- Windows 10 (21H2)

<h2>List of Prerequisites</h2>

-  Create a Virtual Machine Windows 10, 4vCPUs in Azure
-  Install PHP Manager for IIS
-  Install Rewrite Module
-  Install PHP 7.3.8
-  Install Vc redist.x86.exe
-  Install MySQL 5.5.62



       

<h2>Installation Steps</h2>

-  Connect to the Virtual Machine that was created in Azure via Remote Desktop
-  Search for Control Panel
-  Underneath Programs, Select Uninstall a Program
-  On the left side of the screen, select Turn Windows Features On or Off
-  Select and expand Internet Information Services (IIS)
-  Select and expand World Wide Web Services
-  Select and expand Application Development Features
-  Select CGI

<p>
<img src="https://i.imgur.com/Dcjp44b.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

-  Install PHP Manager for IIS


<p>
<img src="https://i.imgur.com/RGHXeRq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

-  Install Rewrite Module
 
<p>
<img src="https://i.imgur.com/LMJfOar.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
       
-  Install PHP 7.3.8 by first creating a PHP folder on the C drive and then downloading and unzipping and extracting all the file contents
   into the PHP file that was just created.
</p>
<br />

<p>
<img src="https://i.imgur.com/n9EoIwq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
       
-  Install Vc redist.x86.exe
       
</p>
<br />

<p>
<img src="https://i.imgur.com/Qso7Mzk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
       
-  Install MySQL 5.5.62, do a typical Install and setup credentials Username: root Password: Password1
       
</p>
<br />

<p>
<img src="https://i.imgur.com/Ni1kFnI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
       
-  Now Open IIS as an Admin and  then reload IIS
-  Register PHP from within IIS
-  Restart the server
</p>
<br />

<p>
<img src="https://i.imgur.com/uiFmLH5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
       
-  Install osTicket v1.15.8
-  Download osTicket
-  Extract and copy"upload" folder to c:\inerpub\wwwroot
-  In c:\inetpub\wwwroot, Rename “upload” to “osTicket”
-  Restart Server
-  Go to sites -> Default-> os Ticket
-  On the right click browse *80. osTicket Installer should appear

</p>
<br />

<p>
<img src="https://i.imgur.com/5yfTSmF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/ >
</p>
<p>
       
-  Click “Enable or disable an extension”
-  Enable: php_imap.dll
-  Enable: php_intl.dll
-  Enable: php_opcache.dll
-  Refresh the osTicket and you should see the additional extentions enabled
-  Rename ost-config.php from C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php to -> C:\inetpub\wwwroot\osTicket\include\ost-config.php
-  Assign Permissions: ost-config.php
-  Disable inheritance -> Remove All
-  New Permissions-> Everyone-> All
-  Click continue on osTicket installer and proceed complted required fields
       
     
</p>
<br />

<p>
<img src="https://i.imgur.com/0mWKAtA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
       
-  Download and Install HeidiSQL
-  Open HeidiSQL
</p>
<br />

<p>
<img src="https://i.imgur.com/yR82XDl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
       
-  Create a new session, root/Password1
-  Connect to the session
-  Create a database called “osTicket”
-  Continue Setting up osTicket in browser with the following input below and click install now

</p>
<br />

<p>
<img src="https://i.imgur.com/tha5uO9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
       
-  osTicket should have installed successfully, you will see the screen below
</p>
<br />

<p>
<img src="https://i.imgur.com/QHXvCLA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
       
-  Browse to your help desk login page: http://localhost/osTicket/scp/login.php
-  Enduser osTicket URL:  http://localhost/osTicket/
       
</p>
<br />


