Azure Private Endpoint Lab

Overview

This lab demonstrates how to securely connect an Azure Virtual Machine to an Azure Storage Account using a Virtual Network and Private Endpoint.

Azure Services Used: 

Azure Virtual Machine
Azure Virtual Network
Azure Storage Account
Network Security Group
Private Endpoint
Private DNS
Azure Firewall

Objectives:

Deploy a Windows Server VM
Configure networking
Configure an NSG
Restrict Storage Account access
Create a Private Endpoint
Verify DNS resolution
Verify HTTPS connectivity

Lab Steps:

Step 1

Created a Virtual Network

Step 2

Created a Windows Server VM

Step 3

Configured NSG

Step 4

Created Storage Account

Step 5

Restricted Public Access

Step 6

Created Private Endpoint

Step 7

Verified connectivity

Verification:
DNS Resolution - nslookup azstorage104one.blob.core.windows.net = Output - 10.0.0.4

HTTPS Test:
Test-NetConnection azstorage104one.blob.core.windows.net -Port 443

Output -  TcpTestSucceeded : True

Lessons Learned:

How Private Endpoints work
Azure Private DNS
NSGs
RDP troubleshooting
Storage Account firewall
VM networking