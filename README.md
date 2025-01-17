<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Install Active Directory
- Create 2 Organizational Units and an new User
- Allow domain users(non-administrative users) access to remote desktop
- Create additional users and logon with one of those users 

<h2>Deployment and Configuration Steps</h2>

<p>
                                  Install Active Directory
</p>

![IMG_9854](https://github.com/user-attachments/assets/8bd135c8-c3f0-490d-a094-cd466df8e2e3)



<p>
Successfully installed active directory.
</p>
<br />

<p>
                          Create 2 Organizational Units and an new User
  
  ![IMG_9855](https://github.com/user-attachments/assets/8a3a0a35-0351-4960-acd2-17ae6b78fc45)

  ![IMG_9856](https://github.com/user-attachments/assets/7cc762cb-ce98-4ca6-a949-86c8f3977913)
</p>
<p>
Within the AD folder I created 2 OU folders _EMPLOYEES and _ADMINS. After I added Jane Doe to _ADMINS group
</p>
<br />

<p>
                       Allow domain users(non-administrative users) access to remote desktop

  ![IMG_9857](https://github.com/user-attachments/assets/61417234-d2d8-4de7-8995-00e84fde2a2e)

</p>
<p>
I can now log into Client-1 as a normal, non-administrative user.
</p>
<br />

                         Create additional users and logon with one of those users 

![IMG_9859](https://github.com/user-attachments/assets/c9f9b9bc-94a1-459f-ae70-5bcd258c0438)
                         
![IMG_9862](https://github.com/user-attachments/assets/d885e0c9-72a7-42b1-8556-98d6f2da458e)

I logged onto DC-1 with jane_admin and opened powershellise, and ran a script that created over 10000 new users and I successfully chose a random user and logged into client 1 with one of those users.


                                                     EXTRAS
                                               

![IMG_9860](https://github.com/user-attachments/assets/b4a1d9b3-0603-49e1-8c0d-9b907a2a6a69)
Successfully unlocked an users account after they got locked out

![IMG_9863](https://github.com/user-attachments/assets/541ebec9-b1c4-4dc6-8d67-bb8c6f1b6f59)

![IMG_9864](https://github.com/user-attachments/assets/c3412103-3e3c-41c4-be36-5cf2256c6bf8)

Was able to disable and then re enable an users account
