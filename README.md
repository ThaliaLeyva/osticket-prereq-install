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

- Create and Set up Virtual Machine
- Install PHP Manager
- Install Rewrite Module
- Install MySQL
- Install OS Ticket

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/N8Eb2Je.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Sign into Azure (create account if subscritption not already obtained). Create a Virtual Machine of which will deploy a rescource group, the Vitrual Machine itself and a subnet. Once Virtual Machine is running obtain the IP address to allow access through remote desktop tool.
</p>
<br />

<p>
<img src="https://i.imgur.com/cv3jaqZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Within the Virtual Machine manually enabling IIS and CGI through the control panel must be done inorder to utilize os Ticket since it runs off of a website itself. Download and install PHP Manager along with IIS rewrite module. After creating a directory C:\PHP we can then download PHP and contents into the folder. Then download MySQL and create creditentials for standard configuration, by doing this it will provide the Virtual Machine with a database of which is needed for osTicket to be able to store the application data. 
</p>
<br />

<p>
<img src="https://i.imgur.com/5EBFl57.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Opening up IIS as an admin to register PHP within IIS. Then restart the server to ensure settings are captured accordingly. Once downloading osTicket itself into the C:\, restart server once more.
</p>
<br />

<img src="https://i.imgur.com/KpPqHNo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Launch osTicket web page. upon first launch some suggested PHP extensions are not enable, therefore we much manually correct via IIS/PHP manager. Download HeidiSQL, create new connection with MySQL then create new database named "osTicket" to finalize complete connection.
</p>
<br />
