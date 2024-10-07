<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Install Active Directory
- Create a Domain Admin user within the domain
- Join Client-1 VM to the domain
- Setup Remote Desktop for non-administrative users on Client-1

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://github.com/user-attachments/assets/c4391903-cf00-4460-bb67-6b251fcbe423" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Here I am installing Active Directory using the Server Manager application on the Windows Server Azure VM.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/ab9cfef0-92ef-40bf-b051-55db278a3258" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Here I am creating a new User and adding them to the Domain Admins Security Group using the Active Directory Control Panel.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/6982ffbf-cf27-4a69-8a8b-b73ce345e7ff" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Here I am on the Client Azure VM and using Windows Settings to join it to the domain on the Windows Server Azure VM.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/edde067d-548d-41c3-85a7-d24276cbd153" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Here I am allowing domain user access to remote desktop on the Client VM so that doamin users can access Client-1.
</p>
<br />

