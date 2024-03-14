<h1>Active Directory Home Lab</h1>


<h2>Description:</h2>
Installed and configured Windows Server 2019 for network operations, optimized Active Directory for streamlined user management and network security. Employed PowerShell script to efficiently generate 1000 user accounts, showcasing automation proficiency for scalability and efficiency.
<br />


<h2>The tools used in this project include:</h2>

- <b>Windows Server 2019: Installed and configured on a virtual machine to serve as the server environment.</b>
- <b>Active Directory: Implemented and fine-tuned to streamline user management and enhance network security.</b>
- <b>PowerShell: Utilized for scripting and automation, particularly for efficiently generating 1000 user accounts.</b>


<h2>Program walk-through:</h2>

<h3>To configute the Active Directory follow the below steps:</h3>

<p align="left">
Open Server Manager, click add roles and features: <br/>
<img src="https://i.imgur.com/KsZC1it.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Click next:  <br/>
<img src="https://i.imgur.com/EcqX7jv.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select Role-based or feature-based installation, click next: <br/>
<img src="https://i.imgur.com/B2iZLsR.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select a server from the server pool, click next:  <br/>
<img src="https://i.imgur.com/YjwLZ4I.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Tick Active Directory Domain Services, click next:  <br/>
<img src="https://i.imgur.com/503FHLx.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Click next:  <br/>
<img src="https://i.imgur.com/2MWwgCr.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Click next:  <br/>
<img src="https://i.imgur.com/JlSEgAI.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Click Install:  <br/>
<img src="https://i.imgur.com/hAJD4BS.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Installation started:  <br/>
<img src="https://i.imgur.com/bOxeIKQ.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Once installation gets completed, click the flag, click 'promote this server to domain controller':  <br/>
<img src="https://i.imgur.com/JWmQuFm.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select add a new forest > give the domain name > click next:  <br/>
<img src="https://i.imgur.com/F50euXW.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Set the password: *********  <br/>
<img src="https://i.imgur.com/GxegI6Z.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Click next:  <br/>
<img src="https://i.imgur.com/9jQ0UBZ.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Click next:  <br/>
<img src="https://i.imgur.com/OaPV0RB.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Click next:  <br/>
<img src="https://i.imgur.com/HGUx2cG.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Click next:  <br/>
<img src="https://i.imgur.com/e0Kb3p0.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Click Install:  <br/>
<img src="https://i.imgur.com/WT74r4l.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Once the installation get completed, system will restart
Select windows administrative tools > active directory users and computers:  <br/>
<img src="https://i.imgur.com/TkCImNi.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Creating OU _Admins, right click mydomain.com, select new, select organization unit, give name '_Admins':  <br/>
<img src="https://i.imgur.com/UavqWKo.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Creating user, right click _Admins, select new, select user:  <br/>
<img src="https://i.imgur.com/Neu5iz0.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Fill the details:  <br/>
<img src="https://i.imgur.com/T0AToPc.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Set the password: Password1, check password never expires:  <br/>
<img src="https://i.imgur.com/BdbLQeS.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Click finish:  <br/>
<img src="https://i.imgur.com/Lsqi6gr.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Making user admin: right click user, select properties, select tab member of, search the group- Domain Admins, click add, click apply, ok:  <br/>
<img src="https://i.imgur.com/2bwOK7A.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Signing-in with admin user:  <br/>
<img src="https://i.imgur.com/RWczByl.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
User signed-in:  <br/>
<img src="https://i.imgur.com/xNg7ad6.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
<h3>Powershell Script:</h3>
Now, download the powershell script from below path:
  https://github.com/joshmadakor1/AD_PS<br/>
<img src="https://i.imgur.com/WwQL8y5.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Open powershell ISE as admin > open powershell script
Give command: Set-ExecutionPolicy Unrestricted > Yestoall
Execute the script by clicking play button (navigate to path of the script first):  <br/>
<img src="https://i.imgur.com/Bd7YIzO.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
<br />
<br />
Users are created:  <br/>
<img src="https://i.imgur.com/Hl0siIn.png" height="80%" width="90%" alt="Disk Sanitization Steps"/>
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
