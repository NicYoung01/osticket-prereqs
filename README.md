<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Install / Enable IIS in Windows WITH CGI
- Download / Install PHP Manager for IIS, Rewrite Module, PHP 7.3.8 (unzip into C:\PHP), VC_redist.x86.exe
- Download / Install MySQL 5.5.62 (Typical Setup / Standard Configuration / *password*)
- Register PHP from within IIS (IIS run as administrator)
- Download osTicket extract and copy “upload” folder to c:\inetpub\wwwroot and rename folder "osTicket"
- Enable: php_imap.dll, Enable: php_intl.dll, Enable: php_opcache.dll inside of PHP Manager
- Assign Permissions in C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php (rename ost-config.php)
- Install HeidiSQL and Create "osTicket" database (used for osTicket setup) 

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/PrBCSLg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
We installed and enabled "Internet Informations Services" inside of windows and enabled the "CGI" feature under the Application Development Features folder located in World Wide Web Services. 
</p>
<br />

<p>
<img src="https://i.imgur.com/xCTreDt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Inside IIS we opened PHP Manager and registered a new version of PHP from an earlier download.
</p>
<br />

<p>
<img src="https://i.imgur.com/tRzBIWw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To finish the setup in osTicket installer we had to create a new database inside of HeidiSQL another downloaded software that required username and password setup.
</p>
<br />
