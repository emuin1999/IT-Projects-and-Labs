# Project: Joining a Windows 11 Client to an Active Directory Domain

## Objective
Connect a Windows 11 client machine to an Active Directory domain and establish communication with a Windows Server Domain Controller.

## Project Overview
In this project, I created a Windows 11 virtual machine using VMware and configured it to communicate with a Windows Server environment.

I configured the client's DNS settings using the Domain Controller's static IP address, tested network connectivity between the two virtual machines, and successfully joined the Windows 11 client to the `wintip.local` domain.

This project demonstrates the process of preparing a client computer for a centralized Active Directory environment.

## Tools & Technologies Used
- **VMware:** Created and managed virtual machines.
- **Windows Server:** Hosted Active Directory Domain Services (AD DS).
- **Windows 11:** Client operating system.
- **Active Directory Domain Services (AD DS):** Managed the domain environment.
- **DNS:** Configured name resolution between the client and Domain Controller.
- **Command Prompt:** Used `ipconfig /all` and `ping` to troubleshoot network connectivity.

## What I Did

1. **Installed Windows 11:** Downloaded and installed Windows 11 on a new VMware virtual machine.
2. **Checked Server Network Configuration:** Used `ipconfig /all` on the Windows Server to identify and verify its static IP address.
3. **Configured Client DNS Settings:** Configured the Windows 11 client's preferred DNS server to point to the Windows Server's static IP address.
4. **Tested Network Connectivity:** Used the `ping` command to verify communication between the Windows 11 client and Windows Server.
5. **Joined the Active Directory Domain:** Connected the Windows 11 client to the `wintip.local` domain.
6. **Verified Domain Connection:** Confirmed that the Windows 11 client successfully joined the domain.

## What I Learned

Through this project, I gained hands-on experience creating and configuring a Windows 11 virtual machine using VMware and preparing it to communicate with a Windows Server.

I learned how important DNS configuration is when joining a client computer to an Active Directory domain. I configured the client's preferred DNS server to use the Domain Controller's static IP address, allowing the client to locate domain services.

I also practiced using Command Prompt commands to troubleshoot network connectivity. I used `ipconfig /all` to examine network configuration details and identify the server's static IP address. I then used the `ping` command to test communication between the client and server.

Finally, I learned how to join a Windows 11 computer to the `wintip.local` domain. This helped me understand how client computers communicate with a Domain Controller and become part of a centralized Active Directory environment.

This project strengthened my understanding of virtual machine configuration, DNS, TCP/IP networking, network troubleshooting, and Active Directory domain administration.

## Commands Used

### 1. Check Server Network Configuration

```cmd
ipconfig /all
```

**Purpose:** Displays detailed network configuration information, including the server's IP address, subnet mask, default gateway, and DNS server.

### 2. Test Network Connectivity

```cmd
ping SERVER_IP_ADDRESS
```

**Purpose:** Tests whether the Windows 11 client can communicate with the Windows Server using its IP address.

### 3. Verify Domain Name Resolution

```cmd
nslookup wintip.local
```

**Purpose:** Checks whether the client's configured DNS server can resolve the Active Directory domain name.

## Screenshot Checklist

The following screenshots document the setup process and demonstrate that the Windows 11 client successfully joined the Active Directory domain.

| # | Screenshot | What It Proves |
|---|---|---|
| 01 | Installed Windows 11 on VMware | Demonstrates that a Windows 11 virtual machine was successfully created using VMware. |
| 02 | Check Server Static IP Using `ipconfig /all` | Shows the Windows Server's network configuration and static IP address. |
| 03 | Use Server IP to Configure Client DNS | Demonstrates that the client's DNS settings were configured using the server's static IP address. |
| 04 | Test Client Connection Using `ping` | Shows that the Windows 11 client can communicate with the Windows Server. |
| 05 | Client Connected to Domain | Confirms that the Windows 11 client successfully joined the `wintip.local` domain. |

## Final Verification

After configuring the client's DNS settings, I tested network connectivity using the `ping` command and verified domain name resolution.

I then joined the Windows 11 client to the `wintip.local` domain and confirmed that the computer successfully connected to the Active Directory environment.

The project demonstrated how to:
- Create and configure virtual machines using VMware.
- Identify and configure static IP and DNS settings.
- Troubleshoot network connectivity using Command Prompt.
- Understand the relationship between DNS and Active Directory.
- Join a Windows client computer to an Active Directory domain.

**Project Status:** Completed
