<h1>Setting Up an Active Directory Home Lab with PowerShell Automation</h1>

<h2>Description</h2>
<p>
    This lab involves the creation of an Active Directory home environment utilizing Oracle VirtualBox. Active Directory administration is performed on Server 2019, while PowerShell automation is employed for provisioning, maintaining, and deprovisioning user accounts.
</p>

<h2>Step-by-Step Project Guide:</h2>


<p align="center">
Download and Install VirtualBox: <br/>
<img src="https://i.imgur.com/SBPXYNb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Download Windows ISOs: <br/>
<img src="https://i.imgur.com/cEGicx0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/GP5aeep.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create Server 2019 Virtual Machine: <br/>
<img src="https://i.imgur.com/uQKJpKA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/ZVppEHJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/o5Co8WA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/vq0AjEy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/lmSpDkU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/QmAE0N3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/TMmqrFK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/ftMQcpQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/AbKw5Is.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/7EeKcUb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/MB5uFKI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/QSRds0a.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/1cMsguP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/6o1Iiai.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/WIywJxK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/3g5IAIJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Install Server 2019 OS: <br/>
<img src="https://i.imgur.com/WxDcALv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/y0krTh4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/Z9gZsyb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/JI0VDrG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/xzlM4zN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/mOfvMYS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/cqQ3IsC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Setup Server Network Adapters: <br/>
<img src="https://i.imgur.com/lBYrFN0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/JqTzulO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Assign IP address to internal adapter: <br/>
<img src="https://i.imgur.com/DUUiQum.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Rename Server to "DC": <br/>
<img src="https://i.imgur.com/FXmqNYs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/hN6YrUk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Install Active Directory Domain Services: <br/>
<img src="https://i.imgur.com/y3gsJnF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/1pVtAHQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/fIMP2Bo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/zSeb8y7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/JplrHZJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/hHaxxwf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/sEFNViM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Promote Domain Controller (MyDomain.com): <br/>
<img src="https://i.imgur.com/aHt83Ho.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/9IO75Lk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/tExnBXX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/KDWmSmU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/Cp4aC20.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/oTjWYJj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/v40RW5i.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/AL4dCrP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create Domain Admin Account: <br/>
<img src="https://i.imgur.com/fU6o2pS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/NwM7gvv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/T20Sg1a.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/WE7x1Lm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/ftkJk33.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/5vUGzAe.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Relogin with Domain Admin Account:  <br/>
<img src="https://i.imgur.com/cjKvP99.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/fUt7dKO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Install and Configure RAS/NAT:  <br/>
<img src="https://i.imgur.com/O5yOpnQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/JSNZ4NI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/o0Twoln.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/iAV6vz0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/M9XXaOD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/1bGscIT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/J6yV4di.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/QQ9w1Uq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/RvfnFRg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/DcGEpWM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/vDhkilJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/ruwPyTy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/1jxr5aA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/uAZtA4y.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Install and Configure DHCP:  <br/>
<img src="https://i.imgur.com/JZV8Hz9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/r4Ft7wp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/MeqQAe8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/gH4mX5P.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/vKWVclA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/oomFm2Q.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/NE3Ivtm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/sKB8hoB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/otDhod5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/aW4cjdm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enable Browsing on the DC:  <br/>
<img src="https://i.imgur.com/6gwrhpi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Setup PowerShell Scripts:  <br/>
<img src="https://i.imgur.com/7ZyN1uQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/7WAwvgk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/Ql59y80.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Change Directory to Script Directory:  <br/>
<img src="https://i.imgur.com/71GfGTW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Run Script to Create Users:  <br/>
<img src="https://i.imgur.com/JbItA8F.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create Windows 10 VM:  <br/>
<img src="https://i.imgur.com/pKFwqcr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/hXJ4MjM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/fTJIpiJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/9rZ7foN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/FecNHLZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/fkSPVJ5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/ZYeVIrk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/E1MYiLB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/O7xmdV9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/Bm43R9R.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Install Windows 10 OS:  <br/>
<img src="https://i.imgur.com/jGBbxMD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/ZtAnycI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/OrKatUp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/0FMKmSc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/eoooE7I.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/lmYizxf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/woLCMO1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/pkRroWL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/HtBzI7X.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/vmOzFVv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/8grSKjD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/oboR626.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Join Windows 10 to Domain and Rename:  <br/>
<img src="https://i.imgur.com/TfJaCjK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/I9Gp3D2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/R1dwD3R.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/TxSW7kC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Login to Client1 with Domain Credentials:  <br/>
<img src="https://i.imgur.com/VXT03Fw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/cbbB8yP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
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

