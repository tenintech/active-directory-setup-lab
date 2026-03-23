<h1>Active Directory User Account Management Lab</h1>
<h2>Objective</h2>
Deploy Windows Server and Active Directory to simulate onboarding and supporting users in a corporate Active Directory environment.

<h2>Technologies/Environments Used</h2>
  
  - Windows Server 2025 (Domain Controller)
 
  - Active Directory Domain Services (ADDS)
  
  - Windows 10 Enterprise Version 22H2 x64 Gen 2
  
  - Remote Desktop (RDP)
  
  - PowerShell
  
  - Virtualization (Azure VM)


<br />



<h2>Installation & Setup Steps:Program walkthrough</h2>



## 1. Create the Domain Controller deploying a Windows Server Virtual Machine(VM)- Operating System: Windows Server 2025- Name DC1
<img width="1920" height="1080" alt="2created dc" src="https://github.com/user-attachments/assets/2e95058d-039e-450f-80d1-d68e1015592e" />

---
<br />


## 2. Create another Windows VM- Operating System: Windows 10 Enterprise- Name- Client1 and add to the same Virtual Network as the DC
<img width="1920" height="1080" alt="3created client1" src="https://github.com/user-attachments/assets/f1cfc3f4-1d6a-4dad-88f2-5dd9b40c8fe1" />



---
<br />
## 3. Set the Domain Controllers Network Interface Card (NIC) to a static private IP address so that it won't change and Client1 can use the VM as the Domain Name Server(DNS). 
<img width="1920" height="1080" alt="4changing ip to static" src="https://github.com/user-attachments/assets/129a2b34-0409-4c4b-b4f2-437b7fc79510" />

---
<br />
## 4. Log into the VM-DC1 using Microsoft Remote Desktop Conncection
<img width="1920" height="1080" alt="5using rdc to connect to dc" src="https://github.com/user-attachments/assets/e8894acc-6bb7-4411-bba3-00da07647754" />

---
<br />
## 5. Disable the firewall so that we can ping and confirm connection between the DC and Client1 VM.
<img width="1272" height="984" alt="9disable firewall" src="https://github.com/user-attachments/assets/0fb3ecf4-b5db-47c4-98de-aa5da97eb6a3" />



---
<br />
## 6. Set Client1 DNS settings to point to DC1's Private IP Address allowing us to join the domain from Client1's VM
<img width="1076" height="996" alt="7changing ip to static dc1" src="https://github.com/user-attachments/assets/64087d13-0377-48f8-8104-4e5e3fd8c581" />


---
<br />
## 7. Open Powershell from Client1 to PING DC1's private IP Address and see if the connection is successful. Use IPCONFIG command to confirm connection to the DNS Server
<img width="951" height="967" alt="10successful ping from dc" src="https://github.com/user-attachments/assets/e72a658e-4c85-41d4-ab91-57dc85b4d0e8" /><img width="1080" height="925" alt="11ipconfig showing dns server" src="https://github.com/user-attachments/assets/80e8d3d8-04b1-43d2-91d9-876d1890156b" />







---
<br />
