<h1>Setting Up an Active Directory Home Lab with PowerShell Automation</h1>

<h2>Description</h2>
<p>
    This lab involves the creation of an Active Directory home environment utilizing Oracle VirtualBox. Active Directory administration is performed on Server 2019, while PowerShell automation is employed for provisioning, maintaining, and deprovisioning user accounts.
</p>

## Step-by-Step Project Guide:

| 1. Download and Install VirtualBox               | 5. Setup Server Network Adapters                | 11. Relogin with Domain Admin Account           | 15. Setup PowerShell Scripts | 20. Join Windows 10 to Domain and Rename |
| -------------------------------------------------| ----------------------------------------------- | ----------------------------------------------- |----------------------------- | ------------------------- |
| 1.1  ![Image 1](https://i.imgur.com/SBPXYNb.png) | 5.1 ![Image 1](https://i.imgur.com/lBYrFN0.png) | 11.1 ![Image1](https://i.imgur.com/cjKvP99.png) | 15.1 ![Image1](https://i.imgur.com/7ZyN1uQ.png) | 20.1 ![Image](https://i.imgur.com/TfJaCjK.png) |
| 2. Download Windows ISOs                         | 5.2 ![Image 2](https://i.imgur.com/JqTzulO.png) | 11.2 ![Image2](https://i.imgur.com/fUt7dKO.png) | 15.2 ![Image2](https://i.imgur.com/7WAwvgk.png) | 20.2 ![Image](https://i.imgur.com/I9Gp3D2.png) |
| 2.1 ![Image 1](https://i.imgur.com/cEGicx0.png)  | 6. Assign IP address to internal adapter        | 12. Install and Configure RAS/NAT               | 15.3 ![Image3](https://i.imgur.com/Ql59y80.png) | 20.3 ![Image](https://i.imgur.com/R1dwD3R.png) |
| 2.2 ![Image 2](https://i.imgur.com/GP5aeep.png)  | 6.1 ![Image 1](https://i.imgur.com/DUUiQum.png) | 12.1 ![Image1](https://i.imgur.com/O5yOpnQ.png) | 16. Change Directory to Script Directory | 20.4 ![Image](https://i.imgur.com/TxSW7kC.png) |
| 3. Create Server 2019 Virtual Machine            | 7. Rename Server to "DC"                        | 12.2 ![Image2](https://i.imgur.com/JSNZ4NI.png) | 16.1 ![Image](https://i.imgur.com/71GfGTW.png) |  21. Login to Client1 with Domain Credentials |
| 3.1 ![Image 1](https://i.imgur.com/uQKJpKA.png)  | 7.1 ![Image1](https://i.imgur.com/FXmqNYs.png)  | 12.3 ![Image3](https://i.imgur.com/o0Twoln.png) | 17. Run Script to Create Users | 21.1 ![Image](https://i.imgur.com/VXT03Fw.png) |
| 3.2 ![Image 2](https://i.imgur.com/ZVppEHJ.png)  | 7.2 ![Image2](https://i.imgur.com/hN6YrUk.png)  | 12.4 ![Image4](https://i.imgur.com/iAV6vz0.png) | 17.1 ![Image](https://i.imgur.com/JbItA8F.png) | 21.2 ![Image](https://i.imgur.com/cbbB8yP.png) |
| 3.3 ![Image 3](https://i.imgur.com/o5Co8WA.png)  | 8. Install Active Directory Domain Services     | 12.5 ![Image5](https://i.imgur.com/M9XXaOD.png) | 18. Create Windows 10 VM |
| 3.4 ![Image 4](https://i.imgur.com/vq0AjEy.png)  | 8.1 ![Image1](https://i.imgur.com/y3gsJnF.png)  | 12.6 ![Image6](https://i.imgur.com/1bGscIT.png) | 18.1 ![Image](https://i.imgur.com/pKFwqcr.png) |
| 3.5 ![Image 5](https://i.imgur.com/lmSpDkU.png)  | 8.2 ![Image2](https://i.imgur.com/1pVtAHQ.png)  | 12.7 ![Image7](https://i.imgur.com/J6yV4di.png) | 18.2 ![Image](https://i.imgur.com/hXJ4MjM.png) |
| 3.6 ![Image 6](https://i.imgur.com/QmAE0N3.png)  | 8.3 ![Image3](https://i.imgur.com/fIMP2Bo.png)  | 12.8 ![Image8](https://i.imgur.com/QQ9w1Uq.png) | 18.3 ![Image](https://i.imgur.com/fTJIpiJ.png) |
| 3.7 ![Image 7](https://i.imgur.com/TMmqrFK.png)  | 8.4 ![Image4](https://i.imgur.com/zSeb8y7.png)  | 12.9 ![Image9](https://i.imgur.com/RvfnFRg.png) | 18.4 ![Image](https://i.imgur.com/9rZ7foN.png) |
| 3.8 ![Image 8](https://i.imgur.com/ftMQcpQ.png)  | 8.5 ![Image5](https://i.imgur.com/JplrHZJ.png)  | 12.10 ![Image10](https://i.imgur.com/DcGEpWM.png) | 18.5 ![Image](https://i.imgur.com/FecNHLZ.png) |
| 3.9 ![Image 9](https://i.imgur.com/AbKw5Is.png)  | 8.6 ![Image6](https://i.imgur.com/hHaxxwf.png)  | 12.11 ![Image11](https://i.imgur.com/vDhkilJ.png) | 18.6 ![Image](https://i.imgur.com/fkSPVJ5.png) |
| 3.10 ![Image 10](https://i.imgur.com/7EeKcUb.png) | 8.7 ![Image7](https://i.imgur.com/sEFNViM.png) | 12.12 ![Image12](https://i.imgur.com/ruwPyTy.png) | 18.7 ![Image](https://i.imgur.com/ZYeVIrk.png) |
| 3.11 ![Image 11](https://i.imgur.com/MB5uFKI.png) | 9. Promote Domain Controller (MyDomain.com)    | 12.13 ![Image13](https://i.imgur.com/1jxr5aA.png) | 18.8 ![Image](https://i.imgur.com/E1MYiLB.png) |
| 3.12 ![Image 12](https://i.imgur.com/QSRds0a.png) | 9.1 ![Image1](https://i.imgur.com/aHt83Ho.png) | 12.14 ![Image14](https://i.imgur.com/uAZtA4y.png) | 18.9 ![Image](https://i.imgur.com/O7xmdV9.png) |
| 3.13 ![Image 13](https://i.imgur.com/1cMsguP.png) | 9.2 ![Image2](https://i.imgur.com/9IO75Lk.png) | 13. Install and Configure DHCP                    | 18.10 ![Image](https://i.imgur.com/Bm43R9R.png) |
| 3.14 ![Image 14](https://i.imgur.com/6o1Iiai.png) | 9.3 ![Image3](https://i.imgur.com/tExnBXX.png) | 13.1 ![Image1](https://i.imgur.com/JZV8Hz9.png)   | 19. Install Windows 10 OS |
| 3.15 ![Image 15](https://i.imgur.com/WIywJxK.png) | 9.4 ![Image4](https://i.imgur.com/KDWmSmU.png) | 13.2 ![Image2](https://i.imgur.com/r4Ft7wp.png)   | 19.1 ![Image](https://i.imgur.com/jGBbxMD.png) |
| 3.16 ![Image 16](https://i.imgur.com/3g5IAIJ.png) | 9.5 ![Image5](https://i.imgur.com/Cp4aC20.png) | 13.3 ![Image3](https://i.imgur.com/MeqQAe8.png)   | 19.2 ![Image](https://i.imgur.com/ZtAnycI.png) |
| 4. Install Server 2019 OS                         | 9.6 ![Image6](https://i.imgur.com/oTjWYJj.png) | 13.4 ![Image4](https://i.imgur.com/gH4mX5P.png)   | 19.3 ![Image](https://i.imgur.com/OrKatUp.png) |
| 4.1 ![Image 1](https://i.imgur.com/WxDcALv.png) |  9.7 ![Image7](https://i.imgur.com/v40RW5i.png) | 13.5 ![Image5](https://i.imgur.com/vKWVclA.png)    | 19.4 ![Image](https://i.imgur.com/0FMKmSc.png) |
| 4.2 ![Image 2](https://i.imgur.com/y0krTh4.png) | 9.8 ![Image8](https://i.imgur.com/AL4dCrP.png)  | 13.6 ![Image6](https://i.imgur.com/oomFm2Q.png)    | 19.5 ![Image](https://i.imgur.com/eoooE7I.png) |
| 4.3 ![Image 3](https://i.imgur.com/Z9gZsyb.png) | 10. Create Domain Admin Account                    | 13.7 ![Image7](https://i.imgur.com/NE3Ivtm.png) | 19.6 ![Image](https://i.imgur.com/lmYizxf.png) |
| 4.4 ![Image 4](https://i.imgur.com/JI0VDrG.png) |  10.1 ![Image1](https://i.imgur.com/fU6o2pS.png)   | 13.8 ![Image8](https://i.imgur.com/sKB8hoB.png) | 19.7 ![Image](https://i.imgur.com/woLCMO1.png) |
| 4.5 ![Image 5](https://i.imgur.com/xzlM4zN.png) | 10.2 ![Image2](https://i.imgur.com/NwM7gvv.png)    | 13.9 ![Image9](https://i.imgur.com/otDhod5.png) | 19.8 ![Image](https://i.imgur.com/pkRroWL.png) |
| 4.6 ![Image 6](https://i.imgur.com/mOfvMYS.png) | 10.3 ![Image3](https://i.imgur.com/T20Sg1a.png)    | 13.10 ![Image10](https://i.imgur.com/aW4cjdm.png) | 19.9 ![Image](https://i.imgur.com/HtBzI7X.png) |
| 4.7 ![Image 7](https://i.imgur.com/cqQ3IsC.png) | 10.4 ![Image4](https://i.imgur.com/WE7x1Lm.png)    | 14. Enable Browsing on the DC                     | 19.10 ![Image](https://i.imgur.com/vmOzFVv.png) |
|                                                 | 10.5 ![Image5](https://i.imgur.com/ftkJk33.png) | 14.1 ![Image1](https://i.imgur.com/6gwrhpi.png)      | 19.11 ![Image](https://i.imgur.com/8grSKjD.png) |
|                                                 | 10.6 ![Image6](https://i.imgur.com/5vUGzAe.png) |                                                      | 19.12 ![Image](https://i.imgur.com/oboR626.png) |
