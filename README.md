
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

<img width="1280" height="1440" alt="make_AD" src="https://github.com/user-attachments/assets/e659fa59-6a33-42ff-9956-87973569ae94" />


keep pressing next until it says install and you will be sighed ouy by now you should have a AD running
key 



once everthing is booted up and now you can open an app type "user" after pressing the windows key and you should
see something along the line "Active Directory User and Computer". 

<img width="1280" height="720" alt="Screenshot from 2026-03-03 17-30-37" src="https://github.com/user-attachments/assets/6c881ebf-e0cb-45cd-b1e6-cc3e7a2e680a" />


now once you open that go to you domain and right click and make an OU (orginiation unit) and name it whatever you like. 

<img width="1280" height="720" alt="OU" src="https://github.com/user-attachments/assets/842f359c-9876-4af5-84ab-6a733657a813" />



now with that folder there you make other OUs for the "Users", "Computers". For right now i will make a user called John Doe

<img width="1280" height="1016" alt="Screenshot from 2026-03-03 17-35-27" src="https://github.com/user-attachments/assets/5209a2ae-91be-42ed-ac61-70e9bcada8c3" />


once youve made an OU for "Users", right click them and hit Users and make the user and make there password. 
i checked that the user must change there password next time they sighned in. 


<img width="1280" height="1016" alt="john_pass" src="https://github.com/user-attachments/assets/460ca0e2-b264-4283-ad7e-d9b5f7c303ec" />

before you go to the other vm you must, set up a static ip in this instince due to being a lab and leaving the gateway blank cause we arent connecting to the internet. 

first go to control panel on the Win Server 


<img width="1024" height="839" alt="Screenshot from 2026-03-03 15-56-31" src="https://github.com/user-attachments/assets/6ce5e3cc-8171-47f1-b74e-3197e4fd62bb" />

from there go to network and sharing center 

from there go to "change adapter settings" 

doulble click and then hit properties 

and look for this setting 

<img width="1024" height="839" alt="Screenshot from 2026-03-03 15-58-14" src="https://github.com/user-attachments/assets/8faec8f9-569f-4a05-a6e2-13eceebf6230" />

and apply these settings 

<img width="1280" height="784" alt="server_ip" src="https://github.com/user-attachments/assets/366e5d76-c1ef-46c5-abac-afae00aaacb9" />

 
go back to virtual box and i open the Cli windows pro, launched it and went throgh all the prompts 

and when inside windows pro set the ip as well as you did for the server to this 

<img width="1024" height="839" alt="cli_ip" src="https://github.com/user-attachments/assets/180a83e2-1eeb-4a57-a26f-6928a3d0552f" />


Once that is done last is to connnect the client to the Domain 

go to setting in windows pro and go to system from there to the "about" section, scoll down to "Related settings" and press "Advanced system settings"

<img width="1024" height="839" alt="Screenshot from 2026-03-03 15-51-42" src="https://github.com/user-attachments/assets/1f389e2a-fb22-4b70-b451-c2a4ac68d61d" />

press change and make put the domain name 
its gonna prompt you to log in do as so and bam your in!


<img width="1024" height="839" alt="Screenshot from 2026-03-03 15-51-51" src="https://github.com/user-attachments/assets/b2e3bc04-b488-47ad-a049-44b17a6a5496" />

from here you can sign in on the Wins Pro into a user you created in the Domain like John Doe you can sign in as him and from the Server in AD you have access to his account by Resetiing his password if needed, if he gets locked out, change his password. 






 
