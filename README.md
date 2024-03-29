<h1>Network File Shares and Permissions</h1>

<h2>Prerequisites</h2>
- Active Directory installed

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop

<h2>Operating Systems Used </h2>

- Windows 10
- Windows Server 2022</b>

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/NYaAokA.jpg" height="80%" width="80%" alt="Reset password"/>
<img src="https://i.imgur.com/enWYm4I.jpg" height="80%" width="80%" alt="Make the DC1 into a static ip address"/>
</p>
<p>
In DC1, reset a normal user's account. After resetting, log into the user with Client1's pc. In DC1, go to C:\drive; create 4 folders named "read-access", "write-access", and "no-access".
</p>
<br />

<p>
<img src="https://i.imgur.com/5gDazDu.jpg" height="80%" width="80%" alt="Give permission to Read Access"/>
<img src="https://i.imgur.com/ofvDdUW.jpg" height="80%" width="80%" alt="Give permission to Write access"/>
<img src="https://i.imgur.com/QAa0ckj.jpg" height="80%" width="80%" alt="Give permission to no Access"/>
</p>
<p>
Create in Folder: “read-access”, Group: “Domain Users”, Permission: “Read”.
Create in Folder: “write-access”,  Group: “Domain Users”, Permissions: “Read/Write”. 
Create in Folder: “no-access”, Group: “Domain Admins”, “Permissions: “Read/Write”. 
</p>
<br />

<p>
<img src="https://i.imgur.com/BQaiVDT.jpg" height="80%" width="80%" alt="Write a file"/>
<img src="https://i.imgur.com/jW6FQZF.jpg" height="80%" width="80%" alt="Your file is in the folder"/>
<img src="https://i.imgur.com/0YziQyz.jpg" height="80%" width="80%" alt="Read a file"/>
<img src="https://i.imgur.com/PS3aB48.jpg" height="80%" width="80%" alt="You have no access"/>
</p>
<p>
On Client-1, navigate to the shared folder (start, run, \\dc-1). Try to access the folders you just created. Which folders can you access? Which folders can you create stuff in? Does it make sense?
</p>
<br />
