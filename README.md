<h1>ZeroLogon (CVE-2020-1472) Exploitation Lab</h1>

<h2>Description</h2>
The purpose of this project is to demonstrate the ZeroLogon, also known as CVE-2020-1472 vulnerability in a controlled lab environemnt. This vulnerability poses a significant threat to Microsoft Windows domain controllers, potentially leading to unauthorized access and compromise of an entire network.
<br />

<h2>Environments Used </h2>

- <b>Windows Server 2019</b> (Unpatched)
- <b>Kali Linux</b> (Impacket & Zerologon Script) 

<h2>Lab walk-through:</h2>

<p align="center">
Set Up Domain Controller: <br/>
<img src="https://i.imgur.com/H9Ayzrq.png" height="80%" width="80%"/> <br />
The host name is “HYDRA-DC” with an IP address of 10.0.2.7. The domain “MARVEL.local” was configured with users. A device running on Windows 10 Enterprise is joined into the “MARVEL” domain, the device is called “Spiderman”. The active users within the domain includes Peter Parker, Miles Morales, the Administrator & SQL Service, the latter both are within the administrators group.
<br />
<br />
Installing Impacket & Run ZeroLogon Scripts:  <br/>
<img src="https://i.imgur.com/fT1rBSj.png" height="80%" width="80%"> <br />
<img src="https://i.imgur.com/mf1D0XX.png" height="80%" width="80%"> <br />
<br />
Dump Hashes: <br/>
<img src="https://i.imgur.com/Lsam6YW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Login to domain controller using Admin hash:  <br/>
<img src="https://i.imgur.com/AfsFzYd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
