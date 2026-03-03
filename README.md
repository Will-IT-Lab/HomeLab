
# HomeLab
making a step by step on how i made my lab enjoy!

Step 1 Download 2 different kinds of windows OS ISO files, the first is the client and the other will run the Active Directory, and also download virtualbox! (in this i chose windows 10 & 2019). 

Link for Client Win:https://www.microsoft.com/en-us/software-download/windows10ISO
Link for Server Win:https://www.microsoft.com/en-us/evalcenter/download-windows-server-2019
Link for Box:https://www.virtualbox.org/wiki/Downloads

Step 2 Once everthing is downloaded, open virual box and this is where all the magic happens. 
go to where it says "New" and add the ISO file into the ISO image section and where is says type add windows 10 pro this will be the client the one that will be a user in the helpdesk situation.

<img width="790" height="423" alt="cli_iso" src="https://github.com/user-attachments/assets/86dc4c97-52e3-43aa-989b-e9eada23b769" />


Step 3 now do the same for the server in terms of versions to pick for the server pick the standard desktop expericance 

<img width="790" height="423" alt="serveriso" src="https://github.com/user-attachments/assets/bd8d4f53-f1c6-483e-946b-d0d1a5bf1f2e" />


now open an application called server manager go to "manage"
<img width="1280" height="1440" alt="AD" src="https://github.com/user-attachments/assets/c7be24d3-2d7f-4d08-9e6e-562ec20e2578" />

 add roles and add the roles you see in the 
screenshot 

<img width="1280" height="1440" alt="Server_roles" src="https://github.com/user-attachments/assets/c6024ff5-1eb8-4c4e-a3da-c8f97b9f5f77" />


Dowload them and wait 

while waiting in order for the vms to be on the same network you must change this setting, 

<img width="742" height="496" alt="Screenshot from 2026-03-03 17-23-57" src="https://github.com/user-attachments/assets/fe2fe4a6-ec79-4505-b231-2e05210c228e" />



now once it has downloaded 

go to AD DS and Add your AD and Add a new forest make a domain name, make a password 

keep pressing next until it says install and you will be sighed ouy by now you should have a AD running
key 

once everthing is booted up and now you can open an app type "user" after pressing the windows key and you should
see something along the line "Active Directory User and Computer". 

now once you open that go to you domain and right click and make an OU (orginiation unit) and name it whatever you like. 

now with that folder there you make other OUs for the "Users", "Computers". For right now i will make a user called John Doe

once youve made an OU for "Users", right click them and hit Users and make the user and make there password. 
i checked that the user must change there password next time they sighned in. 





go back to virtual box and i open the Cli windows pro, launched it and went throgh all the prompts 

go to settings and from there go to systems and go to about 








 
