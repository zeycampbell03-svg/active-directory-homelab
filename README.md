# Active Directory Home Lab (Windows Server 2022)

## Overview

This project demonstrates a hands-on **Active Directory home lab environment** built using **Windows Server 2022** and a **Windows 11 Pro client machine** inside a virtualized environment using **VirtualBox**.

The goal of this lab was to simulate how enterprise organizations manage **users, computers, security policies, and shared resources** through **Active Directory Domain Services (AD DS)**.

In this lab, a Windows Server 2022 machine was configured as a **Domain Controller**, and a Windows 11 Pro machine was joined to the domain in order to test authentication, Group Policy enforcement, and network resource access.

This lab demonstrates how organizations structure their networks using **Active Directory, Organizational Units, security groups, Group Policy Objects, and centralized file services.**

---

## Lab Environment

Virtualization Platform  
VirtualBox

Server  
Windows Server 2022 (Domain Controller)

Client Machine  
Windows 11 Pro (Domain Joined)

Domain Name  
johncam.local

---

## Technologies Used

- Windows Server 2022
- Windows 11 Pro
- Active Directory Domain Services (AD DS)
- Group Policy Management Console (GPMC)
- Organizational Units (OUs)
- Security Groups
- File Services
- Network Drive Mapping
- VirtualBox

---

## Project Objectives

The main objectives of this lab were to:

- Install and configure Windows Server 2022
- Promote the server to a **Domain Controller**
- Create and configure an **Active Directory domain**
- Organize users and resources using **Organizational Units**
- Create **users, groups, and computer objects**
- Join a **Windows 11 Pro client machine** to the domain
- Configure and apply **Group Policy Objects**
- Create **shared network folders**
- Map network drives through Group Policy
- Implement **security policies**

---

## Active Directory Structure

The domain was organized using **Organizational Units (OUs)** to simulate a corporate environment.

### Regional Organizational Units

- USA
- Europe
- Asia

### Department Organizational Units

Within each region, departments were created including:

- IT
- Accounting
- HR
- Sales
- Management

This structure allows administrators to apply policies and permissions efficiently across departments.

---

## User and Group Management

Multiple users were created within each department to simulate employees within an organization.

Example structure:

USA  
Users  
- IT  
- Accounting  
- HR  
- Sales  
- Management  

### Security Groups

Security groups were created to manage permissions more efficiently across the environment.

Examples include:

- Accounting_Users  
- HR_Users  
- IT_Users  
- Management_Users  
- Sales_Users  

Using groups allows administrators to assign permissions to groups instead of individual users, which is a common enterprise best practice.

---

## Computer Organization

Computers were also organized within Active Directory based on departments.

USA  
Computer  
- IT  
- Accounting  
- HR  
- Sales  
- Management  

The **Windows 11 Pro client machine** was joined to the domain and placed into the appropriate organizational unit.

---

## Group Policy Implementation

Several **Group Policy Objects (GPOs)** were created to enforce security and system configuration across the domain.

Policies implemented include:

Password Policy  
Account Lockout Policy  
Disable USB Devices  
Restrict Control Panel Access  
Enforced Desktop Wallpaper  
Network Drive Mapping

These policies were linked to specific **Organizational Units**, ensuring they only apply to the intended users or computers.

---

## File Services and Network Sharing

Shared folders were created on the Windows Server to simulate a centralized file server used by departments.

Example shared folder structure:

Shared Drives  
- Accounting  
- HR  
- IT  
- Sales  
- Management  

Permissions were controlled using **Active Directory security groups** to ensure only authorized users could access their department’s files.

Network drives were automatically mapped to users using **Group Policy**, allowing easy access when logging into the domain.

---

## Windows 11 Client Testing

The Windows 11 Pro client machine was used to validate the Active Directory environment.

Testing included:

- Logging into the domain using AD user accounts
- Verifying Group Policy enforcement
- Confirming network drive mapping
- Testing department file access permissions
- Testing account lockout behavior

This confirmed that policies configured on the **Domain Controller** were successfully applied to **domain-joined client machines**.

---

## Skills Demonstrated

This lab demonstrates hands-on experience with:

- Active Directory Administration
- Organizational Unit Design
- User and Group Management
- Group Policy Configuration
- File Server Configuration
- Network Drive Mapping
- Identity and Access Management
- Windows Server Administration
- Domain Client Management
- Virtualized Lab Deployment

---

## Real World Application

Active Directory is widely used in enterprise networks to manage authentication, authorization, and security policies across organizations.

Real world uses include:

- Centralized user authentication
- Company-wide security policy enforcement
- Managing user permissions and access control
- Automating system configuration through Group Policy
- Managing devices across enterprise networks

Understanding Active Directory is essential for roles such as:

- System Administrator
- Cybersecurity Analyst
- SOC Analyst
- Network Administrator
- IT Support Engineer

---

## Tools Used

VirtualBox  
Windows Server 2022  
Windows 11 Pro  
Active Directory Domain Services  
Group Policy Management Console  
Windows File Services

---

