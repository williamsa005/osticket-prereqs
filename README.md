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

- Windows 10</b> (22H2-x64 Gen2)

<h2>List of Prerequisites</h2>

- Create Virtual Machine in Azure: Windows 10 Virtual Machine (VM) with at least 2-4 virtual CPUs
- Install / Enable IIS in Windows with CGI, common HTTP features, and IIS Management Console 
- Install osTicket 
- Install VC_redist, MySQL, and HeidiSQL

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/tLnCcb9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Here is the initial setup for IIS within the programs section of the control panel. I installed/enabled IIS, CGI, common HTTP features, and Management Console. 
</p>
<br />

<p>
<img src="https://i.imgur.com/LgA5576.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Before continuing with the installation of osTicket I check to ensure IIS has been successfully installed via the loopback network interface (127.0.0.1)
</p>
<br />

<p>
<img src="https://i.imgur.com/VR7RLGA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
osTicket is working but we still need to enable some of the extensions to use certain features.
</p>
<br />
