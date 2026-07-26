# Lab 01: Active Directory Domain Controller Setup

### Objective

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

### Step 1: Create Resource Group

Create a dedicated resource group to isolate all Active Directory lab resources.

Name:
- rg-active-directory-labs
