<h1>Active Directory User Account Management Lab</h1>
<h2>Objective</h2>
Simulate onboarding and supporting users in a corporate Active Directory environment.

<h2>Technologies/Environments Used</h2>
  
  - Windows Server (Domain Controller)
 
  - Active Directory Domain Services
  
  - Windows 10 / Windows 11 VM
  
  - Remote Desktop (RDP)
  
  - PowerShell (optional)
  
  - Virtualization (Azure VM)

<h2>Description</h2>
Project consists of a simple PowerShell script that walks the user through "zeroing out" (wiping) any drives that are connected to the system. The utility allows you to select the target disk and choose the number of passes that are performed. The PowerShell script will configure a diskpart script file based on the user's selections and then launch Diskpart to perform the disk sanitization.
<br />


<h2>Program walk-through:</h2>

<p align="center">
Launch the utility: <br/>
![Alt text](https://github.com/tenintech/ad-infrastructure/blob/25347f832d878dc31009e41f8f6787fd66c7d5d2/2created%20dc.png)
 <img src=""C:\Users\Teni\OneDrive\Pictures\Capturas de pantalla\1.Prepare AD Infrastructure\1resource group.png"" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select the disk:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the number of passes: <br/>
<img src="[https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps](https://github.com/tenintech/ad-infrastructure/blob/main/1resource%20group.png?raw=true)"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>

![Image Alt](image_url)
