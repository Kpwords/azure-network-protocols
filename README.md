<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Network File Shares and Permissions Model</h2>

<img src="https://i.imgur.com/OTBu60k.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04


<h2>Actions and Observations</h2>

- On DC-1, On The C:/ Drive, Create 3 Folders Read-Access, Write-Access, No-Access
- Folder: Read-Access, Group: "Domain Users", Permissions: Read
- Folder: "Write-Access", Group: "Domain Users"/ Permission: Read/Write
- Folder: "No-Access", Group: "Domian Admins", Permissions: Read/Write

<p>
<img src="https://i.imgur.com/nmhmBFJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>



- On Client-1, navigate to the shared folder (start, run, \\dc-1)
- Try to access the folders you just created. Which folders can you access? Which folders can you create stuff in?


</p>
<br />

<p>
<img src="https://i.imgur.com/ZR7QNYD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/sh8rqJs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/8wwFQ9o.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
