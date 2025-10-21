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
Next, open the osTicket installation folder you unzipped on your desktop and double-click PHP Manager for IIS. Follow the setup wizard by clicking Yes or Next as prompted, and allow the installation to complete.


</p>
<br />

<p>
<img width="2560" height="1440" alt="image" src="https://github.com/user-attachments/assets/24c4e927-b9c0-4111-a4c1-9b83069abe5c" />

</p>
<p>
Next, open the folder and install the Rewrite Module by double-clicking the installer file. Follow the prompts by clicking Next until the installation completes and the Finish message appears.


</p>
<br />

<p>
<img width="2560" height="1440" alt="image" src="https://github.com/user-attachments/assets/24c4e927-b9c0-4111-a4c1-9b83069abe5c" />

</p>
<p>
Next, Create a folder in the C drive called "PHP" then from the osTicket installation folder extract the folder PHP 7.3.8 into the C:\PHP folder in the c drive


</p>
<br />

<p>
<img width="2560" height="1392" alt="image" src="https://github.com/user-attachments/assets/98d28253-c676-48e5-8026-b5361d84a689" />

</p>
<p>
Next, from the osTicket Installation Files folder, install VC_redist.x86.exe.

</p>
<br />

<p>
<img width="2560" height="1392" alt="image" src="https://github.com/user-attachments/assets/98d28253-c676-48e5-8026-b5361d84a689" />

</p>
<p>
Then, from the same osTicket installation folder, install MySQL 5.5.62 by clicking Yes as prompted until you reach the setup type. Choose "Typical," then proceed to install the MySQL server. After installation, be sure to launch the Configuration Wizard, select Standard Configuration, and set both the username and password to "root.". Click next then execute.


</p>
<br />

<p>
<img width="2560" height="1392" alt="image" src="https://github.com/user-attachments/assets/98d28253-c676-48e5-8026-b5361d84a689" />

</p>
<p>
Next, open IIS as an administrator. In IIS, go to PHP Manager, select 'Register new PHP version,' navigate to the C drive and open the PHP folder. Select 'php-cgi,' click Open, and then refresh IIS.

<br />

<p>
<img width="2560" height="1392" alt="image" src="https://github.com/user-attachments/assets/98d28253-c676-48e5-8026-b5361d84a689" />

</p>
<p>
Next, install osTicket by unzipping the osTicket v1.15.8 folder from the Installation Files. Copy the 'upload' folder to C:\inetpub\wwwroot, then rename the 'upload' folder to 'osTicket' within the wwwroot directory.

</p>
<br />

<p>
<img width="2560" height="1392" alt="image" src="https://github.com/user-attachments/assets/98d28253-c676-48e5-8026-b5361d84a689" />

</p>
<p>
Next, navigate to C:\inetpub\wwwroot\osTicket\include and rename 'ost-sampleconfig.php' to 'ost-config.php.' Right-click the file, select Properties > Security > Advanced, disable inheritance, and grant new permissions to everyone.


<br />

<p>
<img width="2560" height="1392" alt="image" src="https://github.com/user-attachments/assets/98d28253-c676-48e5-8026-b5361d84a689" />

</p>
<p>
With the osTicket site open in your browser, enter the basic installation information until you reach the database settings section.
</p>
<br />

<p>
<img width="2560" height="1392" alt="image" src="https://github.com/user-attachments/assets/98d28253-c676-48e5-8026-b5361d84a689" />

</p>
<p>
From the osTicket Installation Files folder, install HeidiSQL. Create a new session in HeidiSQL using 'root' as both the username and password. After opening the session, right-click the unnamed server, select 'Create New' > 'Database,' and name it 'osTicket.'
</p>
<br />

<p>
<img width="2560" height="1392" alt="image" src="https://github.com/user-attachments/assets/98d28253-c676-48e5-8026-b5361d84a689" />

</p>
<p>
Return to the browser with the osTicket site open. Complete the database details, using 'osTicket' as the database name and 'root' for both the username and password. Then, click 'Install Now' to proceed.
</p>
<br />
