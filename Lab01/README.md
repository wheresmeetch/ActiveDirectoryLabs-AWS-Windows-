# Lab 01: Active Directory Domain Controller Setup

## Objective

The objective of this lab is to create and configure a Windows Server–based Active Directory Domain Controller in MS Azure. This domain controller will establish the framework for our test environment and serve as the foundation for subsequent Active Directory labs in this repository.

This lab highlights networking configuration, Active Directory Domain Services installation and DNS integration.

## Environment Overview

- **Cloud Platform:** Microsoft Azure  
- **Operating System:** Windows Server 2022 Datacenter  
- **Server Role:** Active Directory Domain Services (AD DS)  
- **Domain Name:** `corp.local`  
- **Domain Controller:** `DC-01`  
- **Administrator Account:** `corp\dc-admin`  
- **Networking:** Azure Virtual Network with static private IP  

## Step 1: Create Resource Group

Create a dedicated resource group to isolate all Active Directory lab resources.

Name:
- active-directory-labs
<img width="520" height="290" alt="Resource Group image" src="https://github.com/wheresmeetch/ActiveDirectoryLabs-MS-Azure-/blob/main/Lab01/screenshots/create%20rg.png" />


## Step 2: Create Virtual Network and Subnet

Creating the virtual network to mirror a work environment

Configuration setting:
- VNet: domain-controller-vnet
- address space: 10.0.0.0/16
-Subnet: subnet-ad
- Subnet range: 10.0.0.0/24
<img width="520" height="290" alt="Virtual Network and Subnet" src="https://github.com/wheresmeetch/ActiveDirectoryLabs-MS-Azure-/blob/main/Lab01/screenshots/Screenshot%202026-06-01%20001852.png" />

## Step 2: Luanch Windows Server Virtual Machine

Configure a windows 2022 server to be promoted to a domain controller 
Configurations:
- Virtual Machine name: domain-controller
- Image: Windows Server 2022 Datacenter
- Size: small D sized VM
- Public IP: enabled
- Virtual Network: domain-controller-vnet
- subnet: ad-subnet
<img width="520" height="290" alt="Virtual Network and Subnet" src="https://github.com/wheresmeetch/ActiveDirectoryLabs-MS-Azure-/blob/main/Lab01/screenshots/vn1.png" />
<img width="520" height="290" alt="Virtual Network and Subnet" src="https://github.com/wheresmeetch/ActiveDirectoryLabs-MS-Azure-/blob/main/Lab01/screenshots/vn1.png" />


