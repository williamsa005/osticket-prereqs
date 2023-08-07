<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This quick guide outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<img src="https://i.imgur.com/6wKbhJc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



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

1. Once you've successfullly created a subscription within Azure https://portal.azure.com/ you are now ready to create a virtual machine by going to virtual machines > create Azure virtual machine.
2. Setup your virtual machine with Windows 10 Pro, version 22H2. Note: for optimal functionality create a virtual machine with at least 2-4 virtual CPUs and 16 gbs of memory.
3. Once you have created your virtual machine you will want to remote desktop connect to it by using the public IP address the VM has provided. A quick search within your computer system should lead you to the remote desktop connection app. *MAC users may need to download the appropriate remote desktop app to continue with the installation.  

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

Reload IIS (Open IIS, Stop and Start the server)

Go to sites -> Default -> osTicket

On the right, click “Browse *:80”

Note: some extensions are not enabled
  - Go back to IIS, sites -> Default -> osTicket

<img src="https://i.imgur.com/suUCwRA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    
  - Double-click PHP Manager

<img src="https://i.imgur.com/qnDtfP1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
    
  - Click “Enable or disable an extension”
    -  Enable: php_imap.dll
    - Enable: php_intl.dll
    - Enable: php_opcache.dll
  - Refresh the osTicket site in your browse, observe the changes

</p>
<br />
