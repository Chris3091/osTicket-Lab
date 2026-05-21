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

First, I to created a resource group in Azure (os-Ticket) in which our VM will be installed into. Once the VM is running, I can make all the necessary installations to get osTicket installed. I'm using a VM build with Windows and it is using a core of 2 with 42GB of RAM which should be sufficient for this lab to supply with enough computing power.

<img width="1763" height="844" alt="image" src="https://github.com/user-attachments/assets/132c2277-4121-4d24-8041-5763f4a423fe" />

Next, I connect to this newly created VM using the Remote Desktop Connection which is a default Windows program.

<img width="542" height="312" alt="image" src="https://github.com/user-attachments/assets/2d489f0e-c832-4be0-8ace-c15666086200" />

Then, proceed to select yes then you should be on the virtual desktop. I will be masking the username and password for this part of the lab.

<img width="511" height="485" alt="image" src="https://github.com/user-attachments/assets/dcfcf0da-e278-408c-8976-e08fda3f0c91" />

Once Inside the virtual machine. The first thing you should see is the server manager when you connect to the virtual desktop.

<img width="1452" height="592" alt="image" src="https://github.com/user-attachments/assets/09f9cb54-cff0-47f4-aa1d-b3272e719132" />
