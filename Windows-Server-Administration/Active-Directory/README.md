# Project: Installing and Configuring Active Directory Domain Services (AD DS)

## Objective
Install the Active Directory Domain Services (AD DS) role and configure Windows Server as a Domain Controller to establish a centralized Active Directory environment.

## Project Overview
In this project, I created a Windows Server virtual machine using VMware and installed the necessary Windows Server components to establish an Active Directory environment.

I installed the Active Directory Domain Services (AD DS) role, configured the required administrative tools, and promoted Windows Server to a Domain Controller.

During the configuration process, I created the `wintip.local` domain, establishing a centralized environment for managing domain users, computers, security groups, and network resources.

## Tools & Technologies Used
- **VMware:** Created and managed the Windows Server virtual machine.
- **Windows Server:** Operating system used to host Active Directory.
- **Active Directory Domain Services (AD DS):** Provided centralized directory services and domain management.
- **Server Manager:** Used to install server roles and features.
- **Active Directory Administrative Tools:** Provided tools for managing domain users, computers, and security groups.
- **Domain Controller:** Managed authentication and domain services.
- **wintip.local:** Custom Active Directory domain.

## What I Did

1. **Installed Windows Server:** Downloaded and installed Windows Server on a VMware virtual machine.
2. **Installed AD DS Role:** Used Server Manager to install the Active Directory Domain Services role.
3. **Installed Administrative Tools:** Installed the necessary management tools for administering Active Directory.
4. **Promoted Windows Server to Domain Controller:** Configured the server as a Domain Controller using the Active Directory Domain Services Configuration Wizard.
5. **Created the Active Directory Domain:** Established the `wintip.local` domain during the domain controller promotion process.
6. **Verified Domain Configuration:** Confirmed that Windows Server was successfully configured as a Domain Controller for the new domain.

## What I Learned

Through this project, I gained hands-on experience creating and configuring a Windows Server virtual machine using VMware. I learned how to install Windows Server and prepare the environment for centralized network and user management.

I also learned how to install the Active Directory Domain Services (AD DS) role and the necessary Windows administrative tools. I practiced promoting Windows Server to a Domain Controller and creating the `wintip.local` domain.

This project helped me understand the role of a Domain Controller in an organization. A Domain Controller provides centralized authentication and allows administrators to manage users, computers, security groups, and network resources from one location.

I also developed a better understanding of how Active Directory serves as the foundation for other Windows Server administration tasks, including creating Organizational Units, managing user accounts, configuring Group Policy, and assigning shared folder permissions.

This project established the foundation for my other Active Directory and Windows Server administration labs.

## Screenshot Checklist

The following screenshots document the installation and configuration process and demonstrate that Active Directory Domain Services was successfully established.

| # | Screenshot | What It Proves |
|---|---|---|
| 01 | VMware Windows Server Installation | Demonstrates that a Windows Server virtual machine was successfully created using VMware. |
| 02 | Install AD DS and Windows Administrative Tools | Shows that the Active Directory Domain Services role and necessary management tools were installed. |
| 03 | Configure Server for Domain Services | Demonstrates the server configuration process before promoting it to a Domain Controller. |
| 04 | Join/Configure `wintip.local` Domain | Confirms that the Windows Server was successfully configured as a Domain Controller for the `wintip.local` domain. |

## Final Verification

After installing the AD DS role, I used the Active Directory Domain Services Configuration Wizard to promote Windows Server to a Domain Controller.

I successfully created the `wintip.local` domain and verified that the server was configured to provide Active Directory services.

The project demonstrated how to:
- Create and configure a Windows Server virtual machine.
- Install Active Directory Domain Services.
- Install Windows administrative tools.
- Promote Windows Server to a Domain Controller.
- Create a new Active Directory domain.
- Establish a centralized environment for managing domain resources.

**Project Status:** Completed
