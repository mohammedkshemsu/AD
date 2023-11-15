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
| 3.9 ![Image 9](https://i.imgur.com/AbKw5Is.png)  | 8.6 ![Image6](https://i.imgur.com/hHaxxwf.png)   |  |
| 3.10 ![Image 10](https://i.imgur.com/7EeKcUb.png) | 8.7 ![Image7](https://i.imgur.com/sEFNViM.png)|    |
| 3.11 ![Image 11](https://i.imgur.com/MB5uFKI.png) |   |   |
| 3.12 ![Image 12](https://i.imgur.com/QSRds0a.png) |   |   |
| 3.13 ![Image 13](https://i.imgur.com/1cMsguP.png) |   |   |
| 3.14 ![Image 14](https://i.imgur.com/6o1Iiai.png) |   |   |
| 3.15 ![Image 15](https://i.imgur.com/WIywJxK.png) |   |   |
| 3.16 ![Image 16](https://i.imgur.com/3g5IAIJ.png) |   |   |
| 4. Install Server 2019 OS                         |   |   |
| 4.1 ![Image 1](https://i.imgur.com/WxDcALv.png) |    |    |
| 4.2 ![Image 2](https://i.imgur.com/y0krTh4.png) |    |    |
| 4.3 ![Image 3](https://i.imgur.com/Z9gZsyb.png) |    |    |
| 4.4 ![Image 4](https://i.imgur.com/JI0VDrG.png) |     |    |
| 4.5 ![Image 5](https://i.imgur.com/xzlM4zN.png) |     |    |
| 4.6 ![Image 6](https://i.imgur.com/mOfvMYS.png) |     |    |
| 4.7 ![Image 7](https://i.imgur.com/cqQ3IsC.png) |     |     |
