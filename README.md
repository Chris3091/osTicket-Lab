<img width="511" height="291" alt="image" src="https://github.com/user-attachments/assets/99798902-d0b9-4790-b189-43360e960888" />


# osTicket---Prerequisites-and-Installation
In this lab, I will install osTicket which is an open-source software used for help desk ticketing. This will be completed using a VM created in Azure. 

# Environments and Technologies Used

Microsoft Azure (Virtual Machines/Compute)

Remote Desktop

Internet Information Services (IIS)

# Windows Services Used
 
Windows 11

# List of Prequisities

Microsoft Azure virtual machine

osTicket v1.15.8

Installing Active Directory in one of the virtual instances

Heidi SQL

MySQL

PHP Manager

VC Redist

Rewrite Module

# Installation Steps

First, I to created a resource group in Azure (os-Ticket) in which our VM will be installed into. Once the VM is running, I can make all the necessary installations to get osTicket installed. I'm using a VM build with Windows (Windows Server 2025 Datacenter Azure Edition) and it is using a core of 2 with 42GB of RAM which should be sufficient for this lab to supply with enough computing power. The location is in East US (Zone 1).

<img width="1763" height="844" alt="image" src="https://github.com/user-attachments/assets/132c2277-4121-4d24-8041-5763f4a423fe" />

Next, You have to copy the public IP address that from the VM and put it into remote desktop. I need connect to this newly created VM using the Remote Desktop Connection which is a default Windows program and use the username and password that I inputed the VM.

<img width="542" height="312" alt="image" src="https://github.com/user-attachments/assets/2d489f0e-c832-4be0-8ace-c15666086200" />

Then, proceed to select yes then you should be on the virtual desktop. I will be masking the username and password for this part of the lab.

<img width="511" height="485" alt="image" src="https://github.com/user-attachments/assets/dcfcf0da-e278-408c-8976-e08fda3f0c91" />

Once Inside the virtual machine. The first thing you should see is the server manager when you connect to the virtual desktop.

<img width="1452" height="592" alt="image" src="https://github.com/user-attachments/assets/09f9cb54-cff0-47f4-aa1d-b3272e719132" />

Next, I used the os-ticket installation file from earlier in the course i copied and pasted it. Then , I put it in the virtual desktop and downloaded the file so, I can proceed to the next step.

<img width="872" height="101" alt="image" src="https://github.com/user-attachments/assets/8427916a-c68c-40cf-9470-9a900b487e89" />

Next, we are going to do the IIS. we have to go the control panel in the command bar. We are going to open the control and click programs ten, click uninstall program ( click the turn window features on or off)

<img width="812" height="538" alt="image" src="https://github.com/user-attachments/assets/bfa374de-6070-40f6-be1a-9ca26692bb8c" />
<img width="699" height="420" alt="image" src="https://github.com/user-attachments/assets/44d6fb36-8be9-44e7-b1de-423e79a7854e" />

Once, you click that your screen should like mine (it might not it might depends on your OS your using). Then, your going to click next and then role based, then click next and next again for the select server roles.

<img width="997" height="708" alt="image" src="https://github.com/user-attachments/assets/390ebad4-222e-4b14-8c5d-c102aacd5572" />

Next, you want to install IIS with CGI you will have to go to server manager then click add roles or features then, click next, go to web server IIS click web server, then application development then, click CGI

<img width="990" height="685" alt="image" src="https://github.com/user-attachments/assets/4bb88067-c04c-4327-96b3-591d74011166" />

<img width="446" height="437" alt="image" src="https://github.com/user-attachments/assets/90a3f87e-2836-41b2-a4f5-fa1385559d05" />

Next, you want to click install then wait a few minutes for the CGI can be installed.

<img width="253" height="238" alt="image" src="https://github.com/user-attachments/assets/d89b013e-6a48-4899-8eac-fd7bdf0e487d" />

Next, We are going to install PHP manager for IIS, so we are going back to the ostick installation file and clicking the PHP Manager.

<img width="1337" height="558" alt="image" src="https://github.com/user-attachments/assets/30eeb993-f011-41ed-8b41-20ffe311427c" />

<img width="735" height="546" alt="image" src="https://github.com/user-attachments/assets/4d7f30b5-795a-4532-9446-939a2e2ae7dd" />

That is what you will see when you open PHP Manager, then you click next and click agree then it will automatically install and that's how PHP manager will installed.

<img width="640" height="531" alt="image" src="https://github.com/user-attachments/assets/443154f7-59b7-4c92-869c-c77c9b8bd3e4" />

Next, we going to install rewrite, so we are going back to the osticket file installation and clicking rewrite.

<img width="665" height="536" alt="image" src="https://github.com/user-attachments/assets/3df9f9ed-34fc-46d2-962f-3b674d8b2407" />

Then, you will click I agree and then click install and it will begin to install and you will then see this scrren letting you know rewrite is installed

<img width="631" height="530" alt="image" src="https://github.com/user-attachments/assets/ff1bb817-f920-419e-bc31-026b89946a0f" />

Next, we are going to proceed to the next step and that is to create a directory called PHP. You will go to the directory files then, click this PC, next click window C and make your own folder.

<img width="780" height="382" alt="image" src="https://github.com/user-attachments/assets/1aacae1f-6043-4b9a-a31d-65261df51823" />

Next, we are going to unzip PHP in the os ticket installion file folder and to do that we will have to extract all info in that folder and we will put it in the PHP folder

<img width="926" height="685" alt="image" src="https://github.com/user-attachments/assets/566d50b4-9fd0-41d7-b25e-408e763b37ac" />

This is what your screen should look like when you complete the transfer to PHP

<img width="1007" height="650" alt="image" src="https://github.com/user-attachments/assets/aa28fd36-c653-4497-85c4-7c6238503138" />

Now we are going to install VC redist and MySQL 5.5. ( go back to the osticket installation file folder and install these two programs)

<img width="727" height="422" alt="image" src="https://github.com/user-attachments/assets/d5af510c-3bd9-4389-8a54-737949712c96" />

In the MySQL is a two part process on the secord part click standard configuration and then next and make up a easy username and password for this lab.

<img width="696" height="485" alt="image" src="https://github.com/user-attachments/assets/5e444acb-575c-44cb-9112-57aa7ad57794" />

When your done you have this screen when you click install.

<img width="669" height="463" alt="image" src="https://github.com/user-attachments/assets/df66e550-7048-4476-8f93-a7b6e77f3b21" />

Next, We are going to open IIS as admin. Then click the name of your lab and then open  PHP Manager.

<img width="1222" height="507" alt="image" src="https://github.com/user-attachments/assets/61cd8763-99b0-4083-a0b7-75f5cdf0cecd" />

Now register a new PHP version and once you click that click the 3 dots and go to php and click phi cgi as the new php.

<img width="786" height="502" alt="image" src="https://github.com/user-attachments/assets/21c0de9e-f7db-4aa0-9dd2-e0dc68b8801c" />

<img width="741" height="388" alt="image" src="https://github.com/user-attachments/assets/abccd276-d37a-48a1-8b50-10d8e557cb7a" />

Next, Reload IIS (Open IIS, Stop and Start the server)

<img width="1087" height="579" alt="image" src="https://github.com/user-attachments/assets/c54dba9b-1d43-4a50-a153-864cb773d7c8" />

Next, Install osTicket v1.15.8 (go back to the osticket installation file folder) From the osTicket-Installation-Files folder, unzip osTicket-v1.15.8.zip and copy the upload folder into c: \inetpub\wwwroot. Within c:\inetpub\wwwroot, Rename upload to osTicket.

<img width="1268" height="465" alt="image" src="https://github.com/user-attachments/assets/a4965748-4a5c-46a0-9212-c470f489e849" />

Reload IIS (Open IIS, Stop and Start the server)

<img width="280" height="482" alt="image" src="https://github.com/user-attachments/assets/b1275595-5639-415b-9ed4-3fe6b9ac834f" />

Go to sites -> Default -> osTicket. Click 80

<img width="240" height="205" alt="image" src="https://github.com/user-attachments/assets/c14ad025-524d-4f57-9534-fb9b5b48790b" />

This will be the outcome if you did everything right until now. we should see osticket installer installed on microsoft edge.

<img width="1234" height="829" alt="image" src="https://github.com/user-attachments/assets/b425bb76-10f9-46d9-bd70-416f409c07d1" />

Next, Go back to IIS, sites -> Default -> osTicket
Double-click PHP Manager, Click Enable or disable an extension
Enable: php_imap.dll, Enable: php_intl.dll, Enable: php_opcache.dll

<img width="435" height="573" alt="image" src="https://github.com/user-attachments/assets/c94055f0-577b-46da-bac2-3a2b7a116c17" />

Refresh the IIS 

<img width="574" height="697" alt="image" src="https://github.com/user-attachments/assets/2e4f68ac-21c2-43df-a510-ad26647334f1" />

Now go to microsoft edge where the osticket installer is on and refresh the page.

<img width="721" height="708" alt="image" src="https://github.com/user-attachments/assets/ce9f2fba-209c-408c-bad2-d33c1c77700e" />

From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php and rename it ost-config.php

<img width="1018" height="607" alt="image" src="https://github.com/user-attachments/assets/9272189c-e835-4b36-8f83-ceb12354e423" />

Assign Permissions: ost-config.php. To do you have click on it and go to properties. Go to advanced and Disable inheritance -> Remove All. New Permissions -> Everyone -> All

<img width="904" height="451" alt="image" src="https://github.com/user-attachments/assets/95dcd83f-1f0d-45de-94a0-a2ce92b89984" />

<img width="1050" height="507" alt="image" src="https://github.com/user-attachments/assets/423e119a-64b0-4d87-9fae-7d9629008c96" />

<img width="1345" height="732" alt="image" src="https://github.com/user-attachments/assets/8e6c1b2b-9d43-4bc4-816b-8d4700481b1e" />

Next select full control 

<img width="702" height="452" alt="image" src="https://github.com/user-attachments/assets/cd0ac84b-0312-474b-a019-06db3e60be0f" />

Continue Setting up osTicket in the browser (click Continue). Fill out the whole page until you reach mysql pleease leave that blank for a while until we proceed to the next step.

<img width="1146" height="827" alt="image" src="https://github.com/user-attachments/assets/76e15512-9a6f-4898-a470-8672e723220e" />

Next, go back to the osticket installation file folder and install heidiSQL Connect to the session. Create a database called osTicket

<img width="1488" height="803" alt="image" src="https://github.com/user-attachments/assets/fc4ca185-cc05-447c-9896-c74c6fc3b678" />

Next, once you finish the installing click finish and click new and enter your password that you used earlier for IIS.

<img width="1176" height="739" alt="image" src="https://github.com/user-attachments/assets/31cc0a09-b117-464b-aa4c-674618afe68a" />

<img width="1194" height="497" alt="image" src="https://github.com/user-attachments/assets/0965bd94-ed64-4391-bba8-0b52ffff4acb" />

Then Continue Setting up osTicket in the browser. Click Install Now. 
Congrats you have now installed osTicket installed.

<img width="1092" height="836" alt="image" src="https://github.com/user-attachments/assets/1ee88573-099e-4ce2-a338-7e9ee601fbc2" />

The click the upper left link to login as a admin or in your profile.

<img width="806" height="527" alt="image" src="https://github.com/user-attachments/assets/337dc855-f3bc-46c8-807b-ddf385dc6f90" />

 Congrats you have logged in the osTicket website.

 <img width="1273" height="551" alt="image" src="https://github.com/user-attachments/assets/103b4732-b53e-4be8-9b23-a77be526afb9" />























