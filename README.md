<h1>Preparing Active Directory Infrastructure in Microsoft Azure</h1>
<h2>Objective</h2>
This project demonstrates the deployment of an on-premises-style Active Directory infrastructure using Microsoft Azure Virtualization. The lap walks through creating a Domain Contoller on a Virtual Network and a client machine, configuring network connectivity, and implementing the required Domain Name Service settings to support Active Directory Domain Services.  
<img width="799" height="891" alt="Screenshot 2026-03-23 195750" src="https://github.com/user-attachments/assets/60595e1c-e055-4b46-a273-c6e0c373ca93" />

<h2>Technologies/Environments Used</h2>
  
  - Microsoft Azure(Virtual Network, Machines)
    
       - Windows Server 2025 (Domain Controller)
 
       - Windows 10 Enterprise Version 22H2 x64 Gen 2
  
  - Active Directory Domain Services (ADDS)
  
  - Remote Desktop (RDP)
  
  - PowerShell
  


<br />



<h2>Step by Step Lab Walkthrough</h2>



### 1. Within Microsoft Azure, create the Domain Controller deploying a Windows Server Virtual Machine(VM)- Image: Windows Server 2025 (Name- DC1)


<img width="900" height="1000" alt="2created dc" src="https://github.com/user-attachments/assets/2e95058d-039e-450f-80d1-d68e1015592e" />

---
<br />


### 2. Create another Windows Virtual Machine- Image: Windows 10 Enterprise (Name- Client1) and add to the same Virtual Network as the Domain Controller


<img width="1920" height="1080" alt="3created client1" src="https://github.com/user-attachments/assets/f1cfc3f4-1d6a-4dad-88f2-5dd9b40c8fe1" />



---
<br />

### 3. Set the Domain Controllers Network Interface Card (NIC) to a static private IP address so that it won't change and VM "Client1" can use the DC as the Domain Name Server(DNS). 


<img width="1920" height="1080" alt="4changing ip to static" src="https://github.com/user-attachments/assets/129a2b34-0409-4c4b-b4f2-437b7fc79510" />

---
<br />

### 4. Log into the VM "DC1" using Microsoft Remote Desktop Connection and disable the firewall so that I can use 'ping' command to confirm connection between the DC and  VM "Client1". Run: wf.msc


<img width="1920" height="1080" alt="5using rdc to connect to dc" src="https://github.com/user-attachments/assets/e8894acc-6bb7-4411-bba3-00da07647754" />
<img width="1272" height="984" alt="9disable firewall" src="https://github.com/user-attachments/assets/0fb3ecf4-b5db-47c4-98de-aa5da97eb6a3" />

---
<br />





### 5. Set VM "Client1" DNS settings to point to, or match, VM "DC1"'s Private IP Address allowing us to join the domain as a user 


<img width="1076" height="996" alt="7changing ip to static dc1" src="https://github.com/user-attachments/assets/64087d13-0377-48f8-8104-4e5e3fd8c581" />


---
<br />

### 6. Open Powershell from "Client1" to "ping" "DC1"'s private IP Address and see if the connection is successful. "ping" IP address 10.0.0.4. Use "ipconfig/all" command to observe DNS settings and confirm connection to the DNS Server 


<img width="951" height="967" alt="10successful ping from dc" src="https://github.com/user-attachments/assets/e72a658e-4c85-41d4-ab91-57dc85b4d0e8" /><img width="1080" height="925" alt="11ipconfig showing dns server" src="https://github.com/user-attachments/assets/80e8d3d8-04b1-43d2-91d9-876d1890156b" />




---
<br />
