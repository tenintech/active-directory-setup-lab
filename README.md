<h1>Active Directory User Account Management Lab</h1>
<h2>Objective</h2>
Deploy Windows Server and Active Directory and simulate onboarding and supporting users in a corporate Active Directory environment.

<h2>Technologies/Environments Used</h2>
  
  - Windows Server (Domain Controller)
 
  - Active Directory Domain Services
  
  - Windows 10 / Windows 11 VM
  
  - Remote Desktop (RDP)
  
  - PowerShell (optional)
  
  - Virtualization (Azure VM)
[CourseCareers IT Course Notes.pdf](https://github.com/user-attachments/files/26172042/CourseCareers.IT.Course.Notes.pdf)
![Alt text](https://github.com/user-attachments/files/26172042/CourseCareers.IT.Course.Notes.pdf))
![Alt text]("C:\Users\Teni\OneDrive\Pictures\Capturas de pantalla\1.Prepare AD Infrastructure\CourseCareers IT Course Notes.pdf")

<br />
(https://github.com/user-attachments/files/26171986/CourseCareers.IT.Course.Notes.pdf)
 <img src=""C:\Users\Teni\OneDrive\Pictures\Capturas de pantalla\1.Prepare AD Infrastructure\1resource group.png"" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<h2>Installation & Setup Steps:Program walkthrough</h2>
<b>Step 1 — Create the Domain Controller</b>

1. Deploy a Windows Server VM.
<img width="1920" height="1080" alt="2created dc" src="https://github.com/user-attachments/assets/2e95058d-039e-450f-80d1-d68e1015592e" />

2. Assign a static private IP address.
<img width="1920" height="1080" alt="4changing ip to static" src="https://github.com/user-attachments/assets/129a2b34-0409-4c4b-b4f2-437b7fc79510" />

3. Rename the server (Example: DC01).

4. Restart the server.


Step 2 — Install Active Directory


 1. Open Server Manager.

 2. Click Add Roles and Features.
      Select:
         - Active Directory Domain Services.

 3. Complete the installation.




   
<b>Step 3 — Promote Server to Domain Controller<b>

1. Click Promote this server to a domain controller.

2. Select:
     - Create a new forest.

3. Name Domain (Domain name example):

       company.local
4. Complete the configuration and restart.


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
