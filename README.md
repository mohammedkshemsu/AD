# Active Directory Lab Environment Setup with PowerShell User Creation

## Overview

This project guides users through setting up a virtual lab environment using VirtualBox, creating a domain controller with Active Directory, and automating user creation through PowerShell. The culmination involves joining a Windows 10 virtual machine to the domain, offering a hands-on experience in a controlled environment.

## Key Features

1. **Virtualized Environment:** Utilize VirtualBox to create an isolated lab environment for testing and learning.

2. **Active Directory Configuration:** Set up a Windows Server with Active Directory Domain Services (AD DS) to establish a domain controller.

3. **DHCP Configuration:** Configure a DHCP server to dynamically assign IP addresses within the network.

4. **PowerShell User Creation:** Employ PowerShell scripts to efficiently create a multitude of users within Active Directory.

5. **Windows 10 Integration:** Join a Windows 10 virtual machine to the domain, showcasing real-world domain integration scenarios.

6. **Network Connectivity:** Verify network settings, internet connectivity, and domain join functionality.

## Step-by-Step Guide

### Step 1: Prepare Your Environment

1. **Download and Install VirtualBox:**
   - Download and install VirtualBox for creating a virtualized environment.

2. **Download Windows 10 ISO:**
   - Download the Windows 10 ISO file from the official Microsoft website.

3. **Set Up VirtualBox Network:**
   - Configure your VirtualBox network settings to ensure proper communication between virtual machines.

### Step 2: Set Up the Domain Controller

4. **Install Windows Server:**
   - Use VirtualBox to create a new virtual machine for Windows Server.
   - Install Windows Server on the virtual machine.

5. **Configure Active Directory:**
   - Install the Active Directory Domain Services (AD DS) role.
   - Promote the server to a domain controller.

6. **Configure DHCP:**
   - Install DHCP role on the domain controller.
   - Configure a DHCP scope to provide IP addresses to clients.

### Step 3: Create PowerShell Script for User Creation

7. **Download User Creation Script:**
   - Find and download the PowerShell script for creating users. (Refer to the provided script.)

8. **Modify Names File:**
   - Open the "names.txt" file and add your name at the top.
   - Save and close the file.

9. **Run PowerShell Script:**
   - Open PowerShell as an administrator.
   - Navigate to the script directory.
   - Set the execution policy to unrestricted: `Set-ExecutionPolicy Unrestricted -Force`
   - Run the user creation script.

### Step 4: Configure Windows 10 Virtual Machine in VirtualBox

10. **Create Virtual Machine in VirtualBox:**
    - Open VirtualBox and create a new virtual machine for Windows 10.
    - Use the downloaded Windows 10 ISO as the installation media.

11. **Configure Networking:**
    - Set the network adapter to "Internal Network" to connect to the internal network created in VirtualBox.

12. **Install Windows 10:**
    - Start the Windows 10 virtual machine and install the operating system.
    - Skip product key and choose Windows 10 Pro edition.

13. **Set Up Windows 10:**
    - Create a local user during the Windows 10 setup process.
    - Ensure you don't create a Microsoft account during the setup.

### Step 5: Join Windows 10 to the Domain

14. **Change Computer Name:**
    - Open advanced system settings and rename the computer to "Client1."

15. **Join the Domain:**
    - Join the Windows 10 machine to the domain (mydomain.com).
    - Use credentials of a user with permission to join machines to the domain.

16. **Verify Domain Join:**
    - Check Active Directory Users and Computers to confirm the presence of the joined machine.

### Step 6: Verify Connectivity and User Login

17. **Verify Network Configuration:**
    - Open Command Prompt on Windows 10 and run `ipconfig`.
    - Ensure the system has the correct IP configuration with the domain controller as the default gateway.

18. **Test Internet Connectivity:**
    - Open a web browser and ensure internet access is working.

19. **Login with Domain Account:**
    - Log in to Windows 10 using the domain account created during user creation.

20. **Verify Active Directory Attributes:**
    - Open Command Prompt and run `whoami` to verify membership in the domain.

## Image Attribution

I'd like to mention that the images used to illustrate steps in this project are collected from the internet. I appreciate the creators for making them available.

## Network Diagram

![Image 1](https://imgur.com/pa8ZFFH.png)

## Step-by-Step Project Guide

|          |          |          |          |         |          |          |
|----------|----------|----------|----------|---------|----------|----------|
|  1. Install VirtualBox  |   1.1  ![Image 1](https://i.imgur.com/SBPXYNb.png)    |   2. Get Windows ISOs     |  2.1 ![Image 1](https://i.imgur.com/cEGicx0.png)       |   2.2 ![Image 2](https://i.imgur.com/GP5aeep.png)      |  3. Create Server 2019 Virtual Machine |  3.1 ![Image 1](https://i.imgur.com/uQKJpKA.png) |
|  3.2 ![Image 2](https://i.imgur.com/ZVppEHJ.png) |  3.3 ![Image 3](https://i.imgur.com/o5Co8WA.png) |  3.4 ![Image 4](https://i.imgur.com/vq0AjEy.png) |  3.5 ![Image 5](https://i.imgur.com/lmSpDkU.png) |   3.6 ![Image 6](https://i.imgur.com/QmAE0N3.png)  |  3.7 ![Image 7](https://i.imgur.com/TMmqrFK.png) | 3.8 ![Image 8](https://i.imgur.com/ftMQcpQ.png) |
|  3.9 ![Image 9](https://i.imgur.com/AbKw5Is.png) | 3.10 ![Image 10](https://i.imgur.com/7EeKcUb.png) | 3.11 ![Image 11](https://i.imgur.com/MB5uFKI.png)  | 3.12 ![Image 12](https://i.imgur.com/QSRds0a.png) | 3.13 ![Image 13](https://i.imgur.com/1cMsguP.png) | 3.14 ![Image 14](https://i.imgur.com/6o1Iiai.png) | 3.15 ![Image 15](https://i.imgur.com/WIywJxK.png) |
| 3.16 ![Image 16](https://i.imgur.com/3g5IAIJ.png) | 4. Install Server 2019 Operating System  |  4.1 ![Image 1](https://i.imgur.com/WxDcALv.png)   | 4.2 ![Image 2](https://i.imgur.com/y0krTh4.png)  |  4.3 ![Image 3](https://i.imgur.com/Z9gZsyb.png) | 4.4 ![Image 4](https://i.imgur.com/JI0VDrG.png)  | 4.5 ![Image 5](https://i.imgur.com/xzlM4zN.png) |
| 4.6 ![Image 6](https://i.imgur.com/mOfvMYS.png) | 4.7 ![Image 7](https://i.imgur.com/cqQ3IsC.png) | 5. Set Up Server Network Adapters | 5.1 ![Image 1](https://i.imgur.com/lBYrFN0.png) | 5.2 ![Image 2](https://i.imgur.com/JqTzulO.png) | 6. Assign IP Address to Internal Adapter | 6.1 ![Image 1](https://i.imgur.com/DUUiQum.png) |
| 7. Rename Server to "DC" | 7.1 ![Image1](https://i.imgur.com/FXmqNYs.png) | 7.2 ![Image2](https://i.imgur.com/hN6YrUk.png) | 8. Install Active Directory Domain Services | 8.1 ![Image1](https://i.imgur.com/y3gsJnF.png) | 8.2 ![Image2](https://i.imgur.com/1pVtAHQ.png) | 8.3 ![Image3](https://i.imgur.com/fIMP2Bo.png) |
| 8.4 ![Image4](https://i.imgur.com/zSeb8y7.png) | 8.5 ![Image5](https://i.imgur.com/JplrHZJ.png) | 8.6 ![Image6](https://i.imgur.com/hHaxxwf.png) | 8.7 ![Image7](https://i.imgur.com/sEFNViM.png) | 9. Promote Domain Controller (MyDomain.com) | 9.1 ![Image1](https://i.imgur.com/aHt83Ho.png) | 9.2 ![Image2](https://i.imgur.com/9IO75Lk.png) |
| 9.3 ![Image3](https://i.imgur.com/tExnBXX.png) | 9.4 ![Image4](https://i.imgur.com/KDWmSmU.png) | 9.5 ![Image5](https://i.imgur.com/Cp4aC20.png) | 9.6 ![Image6](https://i.imgur.com/oTjWYJj.png) | 9.7 ![Image7](https://i.imgur.com/v40RW5i.png) | 9.8 ![Image8](https://i.imgur.com/AL4dCrP.png) |          |
| 10. Create Domain Admin Account | 10.1 ![Image1](https://i.imgur.com/fU6o2pS.png) | 10.2 ![Image2](https://i.imgur.com/NwM7gvv.png) | 10.3 ![Image3](https://i.imgur.com/T20Sg1a.png) | 10.4 ![Image4](https://i.imgur.com/WE7x1Lm.png) | 10.5 ![Image5](https://i.imgur.com/ftkJk33.png) | 10.6 ![Image6](https://i.imgur.com/5vUGzAe.png) |
| 11. Log in Again with Domain Admin Account |11.1 ![Image1](https://i.imgur.com/cjKvP99.png) | 11.2 ![Image2](https://i.imgur.com/fUt7dKO.png) | 12. Configure RAS/NAT | 12.1 ![Image1](https://i.imgur.com/O5yOpnQ.png) | 12.2 ![Image2](https://i.imgur.com/JSNZ4NI.png) | 12.3 ![Image3](https://i.imgur.com/o0Twoln.png) |
| 12.4 ![Image4](https://i.imgur.com/iAV6vz0.png) | 12.5 ![Image5](https://i.imgur.com/M9XXaOD.png) | 12.6 ![Image6](https://i.imgur.com/1bGscIT.png) | 12.7 ![Image7](https://i.imgur.com/J6yV4di.png) | 12.8 ![Image8](https://i.imgur.com/QQ9w1Uq.png) | 12.9 ![Image9](https://i.imgur.com/RvfnFRg.png) | 12.10 ![Image10](https://i.imgur.com/DcGEpWM.png) |
| 12.11 ![Image11](https://i.imgur.com/vDhkilJ.png) | 12.12 ![Image12](https://i.imgur.com/ruwPyTy.png) | 12.13 ![Image13](https://i.imgur.com/1jxr5aA.png) | 12.14 ![Image14](https://i.imgur.com/uAZtA4y.png) | 13. Configure DHCP | 13.1 ![Image1](https://i.imgur.com/JZV8Hz9.png) | 13.2 ![Image2](https://i.imgur.com/r4Ft7wp.png) |
| 13.3 ![Image3](https://i.imgur.com/MeqQAe8.png) | 13.4 ![Image4](https://i.imgur.com/gH4mX5P.png) | 13.5 ![Image5](https://i.imgur.com/vKWVclA.png) | 13.6 ![Image6](https://i.imgur.com/oomFm2Q.png) | 13.7 ![Image7](https://i.imgur.com/NE3Ivtm.png) | 13.8 ![Image8](https://i.imgur.com/sKB8hoB.png) | 13.9 ![Image9](https://i.imgur.com/otDhod5.png) |
| 13.10 ![Image10](https://i.imgur.com/aW4cjdm.png) | 14. Enable Browsing on the DC | 14.1 ![Image1](https://i.imgur.com/6gwrhpi.png) | 15. Set Up PowerShell Scripts | 15.1 ![Image1](https://i.imgur.com/7ZyN1uQ.png) | 15.2 ![Image2](https://i.imgur.com/7WAwvgk.png) | 15.3 ![Image3](https://i.imgur.com/Ql59y80.png) |
| 16. Change Directory to Script Directory | 16.1 ![Image](https://i.imgur.com/71GfGTW.png) | 17. Run Script to Create Users | 17.1 ![Image](https://i.imgur.com/JbItA8F.png) | 18. Create Windows 10 Virtual Machine| 18.1 ![Image](https://i.imgur.com/pKFwqcr.png) | 18.2 ![Image](https://i.imgur.com/hXJ4MjM.png) |
| 18.3 ![Image](https://i.imgur.com/fTJIpiJ.png) | 18.4 ![Image](https://i.imgur.com/9rZ7foN.png) | 18.5 ![Image](https://i.imgur.com/FecNHLZ.png) | 18.6 ![Image](https://i.imgur.com/fkSPVJ5.png) | 18.7 ![Image](https://i.imgur.com/ZYeVIrk.png) | 18.8 ![Image](https://i.imgur.com/E1MYiLB.png) | 18.9 ![Image](https://i.imgur.com/O7xmdV9.png)  |
| 18.10 ![Image](https://i.imgur.com/Bm43R9R.png) | 19. Install Windows 10 Operating System | 19.1 ![Image](https://i.imgur.com/jGBbxMD.png) | 19.2 ![Image](https://i.imgur.com/ZtAnycI.png) | 19.3 ![Image](https://i.imgur.com/OrKatUp.png) | 19.4 ![Image](https://i.imgur.com/0FMKmSc.png) | 19.5 ![Image](https://i.imgur.com/eoooE7I.png) |
| 19.6 ![Image](https://i.imgur.com/lmYizxf.png) | 19.7 ![Image](https://i.imgur.com/woLCMO1.png) | 19.8 ![Image](https://i.imgur.com/pkRroWL.png) | 19.9 ![Image](https://i.imgur.com/HtBzI7X.png) | 19.10 ![Image](https://i.imgur.com/vmOzFVv.png) | 19.11 ![Image](https://i.imgur.com/8grSKjD.png) | 19.12 ![Image](https://i.imgur.com/oboR626.png) |
| 20. Join Windows 10 to Domain and Rename | 20.1 ![Image](https://i.imgur.com/TfJaCjK.png) | 20.2 ![Image](https://i.imgur.com/I9Gp3D2.png) | 20.3 ![Image](https://i.imgur.com/R1dwD3R.png) | 20.4 ![Image](https://i.imgur.com/TxSW7kC.png) |          |   | 
| 21. Log in to Client1 with Domain Credentials | 21.1 ![Image](https://i.imgur.com/VXT03Fw.png) | 21.2 ![Image](https://i.imgur.com/cbbB8yP.png) |   |   |   |   |
