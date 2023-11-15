<h1>Setting Up an Active Directory Home Lab with PowerShell Automation</h1>

<h2>Description</h2>
<p>
    This lab involves the creation of an Active Directory home environment utilizing Oracle VirtualBox. Active Directory administration is performed on Server 2019, while PowerShell automation is employed for provisioning, maintaining, and deprovisioning user accounts.
</p>

## Step-by-Step Project Guide:

| 1. Download and Install VirtualBox               | 5. Setup Server Network Adapters                   |  |  |
| -------------------------------------------------| ----------------------------------------------- | ---------------------------------- |---------------------- |
| 1.1  ![Image 1](https://i.imgur.com/SBPXYNb.png) | 5.1 ![Image 1](https://i.imgur.com/lBYrFN0.png) |  |
| 2. Download Windows ISOs                         | 5.2 ![Image 2](https://i.imgur.com/JqTzulO.png) |  |
| 2.1 ![Image 1](https://i.imgur.com/cEGicx0.png)  | 6. Assign IP address to internal adapter        |  |
| 2.2 ![Image 2](https://i.imgur.com/GP5aeep.png)  | 6.1 ![Image 1](https://i.imgur.com/DUUiQum.png) |  |  
| 3. Create Server 2019 Virtual Machine            | 7. Rename Server to "DC"                        |  | 
| 3.1 ![Image 1](https://i.imgur.com/uQKJpKA.png)  | 7.1 ![Image1](https://i.imgur.com/FXmqNYs.png)  |  | 
| 3.2 ![Image 2](https://i.imgur.com/ZVppEHJ.png)  | 7.2 ![Image2](https://i.imgur.com/hN6YrUk.png)  |  | 
| 3.3 ![Image 3](https://i.imgur.com/o5Co8WA.png)  | 8. Install Active Directory Domain Services     |  |
| 3.4 ![Image 4](https://i.imgur.com/vq0AjEy.png)  | 8.1 ![Image1](https://i.imgur.com/y3gsJnF.png)  |  |
| 3.5 ![Image 5](https://i.imgur.com/lmSpDkU.png)  | 8.2 ![Image2](https://i.imgur.com/1pVtAHQ.png)   |  |
| 3.6 ![Image 6](https://i.imgur.com/QmAE0N3.png)  | 8.3 ![Image3](https://i.imgur.com/fIMP2Bo.png)  |  |
| 3.7 ![Image 7](https://i.imgur.com/TMmqrFK.png)  | 8.4 ![Image4](https://i.imgur.com/zSeb8y7.png)  |   |
| 3.8 ![Image 8](https://i.imgur.com/ftMQcpQ.png)  | 8.5 ![Image5](https://i.imgur.com/JplrHZJ.png)  |   |
| 3.9 ![Image 9](https://i.imgur.com/AbKw5Is.png)  | 8.6 ![Image6](https://i.imgur.com/hHaxxwf.png)  |  |
| 3.10 ![Image 10](https://i.imgur.com/7EeKcUb.png) | 8.7 ![Image7](https://i.imgur.com/sEFNViM.png) |    |
| 3.11 ![Image 11](https://i.imgur.com/MB5uFKI.png) | 9. Promote Domain Controller (MyDomain.com)    |   |
| 3.12 ![Image 12](https://i.imgur.com/QSRds0a.png) | 9.1 ![Image1](https://i.imgur.com/aHt83Ho.png) |   |
| 3.13 ![Image 13](https://i.imgur.com/1cMsguP.png) | 9.2 ![Image2](https://i.imgur.com/9IO75Lk.png) |   |
| 3.14 ![Image 14](https://i.imgur.com/6o1Iiai.png) | 9.3 ![Image3](https://i.imgur.com/tExnBXX.png) |   |
| 3.15 ![Image 15](https://i.imgur.com/WIywJxK.png) | 9.4 ![Image4](https://i.imgur.com/KDWmSmU.png) |   |
| 3.16 ![Image 16](https://i.imgur.com/3g5IAIJ.png) | 9.5 ![Image5](https://i.imgur.com/Cp4aC20.png) |   |
| 4. Install Server 2019 OS                         | 9.6 ![Image6](https://i.imgur.com/oTjWYJj.png) |   |
| 4.1 ![Image 1](https://i.imgur.com/WxDcALv.png) |  9.7 ![Image7](https://i.imgur.com/v40RW5i.png) |    |
| 4.2 ![Image 2](https://i.imgur.com/y0krTh4.png) | 9.8 ![Image8](https://i.imgur.com/AL4dCrP.png)  |    |
| 4.3 ![Image 3](https://i.imgur.com/Z9gZsyb.png) | 10. Create Domain Admin Account                     |    |
| 4.4 ![Image 4](https://i.imgur.com/JI0VDrG.png) |  10.1 ![Image1](https://i.imgur.com/fU6o2pS.png)    |    |
| 4.5 ![Image 5](https://i.imgur.com/xzlM4zN.png) | 10.2 ![Image2](https://i.imgur.com/NwM7gvv.png)    |    |
| 4.6 ![Image 6](https://i.imgur.com/mOfvMYS.png) | 10.3 ![Image3](https://i.imgur.com/T20Sg1a.png)    |    |
| 4.7 ![Image 7](https://i.imgur.com/cqQ3IsC.png) | 10.4 ![Image4](https://i.imgur.com/WE7x1Lm.png)    |     |
|   | 10.5 ![Image5](https://i.imgur.com/ftkJk33.png) |   |  
|   |  10.6 ![Image6](https://i.imgur.com/5vUGzAe.png) |  |
