<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Install or enable IIS in Windows, ensuring CGI and required modules are enabled.
- Install the Web Platform Installer.
- Install MySQL and create the osTicket database.
- Install the C++ Redistributable.
- Configure permissions and install osTicket.

<h2>Installation Steps</h2>

<p>
<img width="2560" height="1392" alt="image" src="https://github.com/user-attachments/assets/98d28253-c676-48e5-8026-b5361d84a689" />

</p>
<p>
Set up an Azure VM with Windows 10 and at least 8 GB of memory to ensure smooth performance. Be sure to create an admin username and password.
</p>
<br />

<p>
<img width="2560" height="1440" alt="image" src="https://github.com/user-attachments/assets/24c4e927-b9c0-4111-a4c1-9b83069abe5c" />


</p>
<p>
Next, Within the windows vm open the osticket link and download the osTicket-Installation-Files to your desktop and unzip it onto your desktop.

</p>
<br />

<p>
<img width="2560" height="1440" alt="image" src="https://github.com/user-attachments/assets/24c4e927-b9c0-4111-a4c1-9b83069abe5c" />

</p>
<p>
Next, enable Internet Information Services (IIS) and CGI by opening the Control Panel, going to Programs, and selecting 'Turn Windows features on or off.' Enable Internet Information Services to install IIS, expand World Wide Web Services, then Application Development Features, and check CGI. Click OK to install the required features
</p>
<br />

<p>
<img width="2560" height="1440" alt="image" src="https://github.com/user-attachments/assets/24c4e927-b9c0-4111-a4c1-9b83069abe5c" />

</p>
<p>
Next, open the osTicket installation folder you unzip on your desktop and double click PHP manager for iis
</p>
<br />
