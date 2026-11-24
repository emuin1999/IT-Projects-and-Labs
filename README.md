# IT Projects and Labs

A collection of hands-on IT projects covering Windows Server administration, Active Directory, networking, help desk troubleshooting, and cybersecurity.

## About This Repository

Welcome to my IT Projects and Labs repository!

This repository documents my hands-on experience building, configuring, managing, and troubleshooting IT environments. Through these projects, I practice real-world IT support and systems administration tasks using virtual machines, Windows Server, Active Directory, and other IT tools.

My goal is to develop practical technical skills, strengthen my troubleshooting abilities, and build a strong foundation for a career in IT support, systems administration, and cybersecurity.

Each project includes an objective, tools and technologies used, implementation steps, lessons learned, and screenshots documenting the configuration and troubleshooting process.

---

## Technical Skills & Technologies

### Operating Systems
- Windows Server
- Windows 11

### Active Directory & Windows Server Administration
- Active Directory Domain Services (AD DS)
- Active Directory Users and Computers (ADUC)
- Domain Controller Configuration
- Organizational Units (OUs)
- User and Security Group Management
- Group Policy Objects (GPOs)
- AGDLP Group Management
- Password and Account Lockout Policies
- Share and NTFS Permissions
- Group Policy Preferences
- Network Drive Mapping
- Item-Level Targeting

### Networking
- DNS Configuration
- TCP/IP Networking
- Static IP Configuration
- Network Connectivity Testing
- `ipconfig /all`
- `ping`
- `nslookup`

### Help Desk & Technical Support
- Ticket Creation and Management
- Spiceworks Help Desk
- Account Lockout Troubleshooting
- Password Resets
- Remote Desktop Support
- User Communication
- Technical Documentation
- Incident Resolution

### Virtualization & Lab Environment
- VMware
- Windows Server Virtual Machines
- Windows 11 Client Virtual Machines
- Client-Server Networking

---

## Projects & Labs

The following projects demonstrate my hands-on experience with Windows Server administration, Active Directory, network configuration, and IT support.

### 1. Windows Server & Active Directory

**Project 1: Installing Active Directory Domain Services (AD DS)**

- Installed Windows Server using VMware.
- Installed the Active Directory Domain Services role.
- Promoted Windows Server to a Domain Controller.
- Created the `wintip.local` domain.

**Project 2: Creating Active Directory Users, Groups, and Organizational Units**

- Created a company OU named LexCorp.
- Established HR, IT, and Sales departmental OUs.
- Created domain users and security groups.
- Implemented nested groups using the AGDLP model.
- Organized users and groups for centralized administration.

**Project 3: Joining a Windows 11 Client to the Domain**

- Installed Windows 11 using VMware.
- Configured client DNS settings.
- Tested connectivity between the client and server.
- Joined the Windows 11 client to the `wintip.local` domain.

### 2. Group Policy & Access Management

**Project 4: Configuring and Managing Group Policy**

- Configured password and account lockout policies.
- Restricted Control Panel access.
- Automated network drive mapping.
- Configured Group Policy Preferences.
- Implemented Item-Level Targeting.
- Applied and verified GPOs on a Windows 11 client.

**Project 5: Configuring Shared Folder Permissions**

- Created shared folders for different departments.
- Configured Share and NTFS permissions.
- Implemented read-only access for HR Interns.
- Restricted access to the IT Licenses folder.
- Used Active Directory security groups to manage resource access.
- Tested permissions using different domain user accounts.

### 3. Help Desk & Technical Support

**Project 6: Creating and Documenting a Support Ticket in Spiceworks**

- Created a support ticket for an Active Directory account lockout.
- Reviewed the user's reported issue and attached screenshot.
- Accepted and managed the support ticket.
- Unlocked the user's account using ADUC.
- Reset the user's password.
- Communicated with the user and verified the resolution.
- Documented the troubleshooting steps and closed the ticket.

---

## Lab Environment

My projects are completed using a virtualized Windows Server and Windows 11 client environment.

| Component | Configuration |
|---|---|
| Virtualization Platform | VMware |
| Server Operating System | Windows Server |
| Client Operating System | Windows 11 |
| Domain Name | wintip.local |
| Directory Service | Active Directory Domain Services |
| Administration Tools | Server Manager, ADUC, Group Policy Management |
| Ticketing System | Spiceworks |

## Learning Objectives

Through these projects, I am developing practical experience in:

- Building and managing Windows Server environments.
- Installing and configuring Active Directory.
- Creating and managing domain users, groups, and OUs.
- Implementing security policies through Group Policy.
- Managing shared folder access using Share and NTFS permissions.
- Troubleshooting DNS and network connectivity issues.
- Supporting users and resolving common IT problems.
- Documenting incidents and maintaining support tickets.
- Applying security principles such as least privilege.

## Project Documentation

Each project has its own folder containing:

- **README.md:** Project objective, overview, tools, implementation steps, and lessons learned.
- **Screenshots:** Visual documentation demonstrating the completed configurations and troubleshooting results.

## Future Projects

I plan to expand this repository with additional hands-on projects covering:

- Remote Desktop Troubleshooting
- Windows Troubleshooting and System Administration
- DNS Troubleshooting and Configuration
- DHCP Server Configuration
- Printer Troubleshooting
- Windows Event Viewer and Log Analysis
- PowerShell Automation
- Network Security
- Cybersecurity Fundamentals

## Career Goals

I am continuously developing my technical skills through hands-on labs and practical IT projects.

My goal is to build a strong foundation in IT support and systems administration while expanding my knowledge of networking, infrastructure management, and cybersecurity.

I believe that practical experience, continuous learning, and effective troubleshooting are essential to becoming a successful IT professional.

---

**Thank you for visiting my IT Projects and Labs repository!**
