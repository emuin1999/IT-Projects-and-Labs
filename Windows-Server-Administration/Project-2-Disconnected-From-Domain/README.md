# Project 2: Employee Computer Disconnected From Domain

## Project Overview

An employee reports that their Windows 11 computer is experiencing problems communicating with the organization's Active Directory domain. The computer is unable to properly locate the domain controller, potentially affecting domain authentication and access to network resources.

As the Help Desk Technician, I investigate the issue, identify an incorrect DNS configuration, restore the correct DNS settings, and verify that the workstation can communicate with the domain controller again.

## Objective

Demonstrate the ability to troubleshoot and resolve an Active Directory domain connectivity issue caused by incorrect DNS configuration.

## Lab Environment

| Component | Configuration |
|---|---|
| Virtualization Software | VMware Workstation |
| Server | Windows Server |
| Client | Windows 11 |
| Directory Service | Active Directory Domain Services (AD DS) |
| Network Configuration | Static IP addressing |
| Remote Support | Remote Desktop Protocol (RDP) |
| Command-Line Tools | PowerShell, Command Prompt |
| DNS Service | Windows Server DNS |

## Simulated Help Desk Ticket

**Ticket Title:** Employee Computer Disconnected From Domain

**Issue Description:**

An employee reports that their workstation is experiencing domain connectivity problems. They are unable to properly access domain resources and may encounter authentication issues.

**Reported Symptoms:**
- Workstation cannot locate or communicate with the domain controller.
- Domain authentication may fail.
- Access to domain resources may be affected.
- DNS resolution may fail.

**Priority:** Medium

**Ticket Status:** In Progress

## Troubleshooting Process

### Step 1: Investigate Network Configuration

Used the following command to review the client's IP address, subnet mask, default gateway, and DNS server configuration.

```cmd
ipconfig /all
```

**Purpose:** Identify whether the workstation is configured to use the correct DNS server.

### Step 2: Test DNS Resolution

Used `nslookup` to determine whether the workstation could resolve the Active Directory domain name.

```cmd
nslookup yourdomain.local
```

**Purpose:** Verify that DNS can resolve the domain name.

### Step 3: Verify Domain Controller Discovery

Used the following command to check whether the workstation could locate a domain controller.

```cmd
nltest /dsgetdc:yourdomain.local
```

**Purpose:** Verify that the workstation can discover an available domain controller.

### Step 4: Identify the DNS Configuration Issue

Inspected the client's network adapter settings and identified an incorrect DNS server configuration.

The workstation was not using the domain controller's IP address as its preferred DNS server.

### Step 5: Correct DNS Configuration

Updated the Windows 11 client's preferred DNS server to the IP address of the Windows Server domain controller.

**Important:** Domain-joined Windows workstations should use the organization's internal DNS server for Active Directory domain resolution.

### Step 6: Verify DNS Resolution

Repeated the DNS lookup command:

```cmd
nslookup yourdomain.local
```

Confirmed that the domain name resolved successfully.

### Step 7: Verify Domain Controller Connectivity

Executed:

```cmd
nltest /dsgetdc:yourdomain.local
```

Confirmed that the workstation could locate the domain controller.

### Step 8: Verify Domain Connectivity

Performed additional checks to confirm that the workstation could communicate with the domain controller and access domain resources.

## Commands Used

| Command | Purpose |
|---|---|
| `ipconfig /all` | Displays IP and DNS configuration |
| `nslookup` | Tests DNS name resolution |
| `nltest /dsgetdc:domain.local` | Locates a domain controller |
| `ping server-IP` | Tests basic network connectivity |

## Resolution

The issue was caused by an incorrect DNS server configuration on the Windows 11 workstation.

The DNS settings were corrected to point to the Windows Server domain controller. DNS resolution and domain controller discovery were then tested to verify the repair.

**Final Result:** Workstation domain connectivity restored.

## Skills Demonstrated

- Active Directory troubleshooting
- DNS configuration and troubleshooting
- Windows 11 network configuration
- Domain controller discovery
- PowerShell and Command Prompt
- Remote Desktop troubleshooting
- Network connectivity testing
- Help Desk ticket documentation
- Technical problem-solving

## Project Evidence

The following screenshots will document the troubleshooting and resolution process:

| # | Screenshot | What It Demonstrates |
|---|---|---|
| 01 | Help Desk Ticket | Employee reports domain connectivity issue |
| 02 | Client IP Configuration | Shows incorrect DNS server configuration |
| 03 | Failed DNS Lookup | Demonstrates DNS resolution failure |
| 04 | Domain Controller Discovery | Shows initial domain controller discovery result |
| 05 | Corrected DNS Configuration | Shows DNS pointing to the domain controller |
| 06 | Successful DNS Lookup | Demonstrates restored DNS resolution |
| 07 | Successful Domain Controller Discovery | Confirms the workstation can locate the domain controller |
| 08 | Resolved Ticket | Documents the repair and final resolution |

## Conclusion

This project demonstrates how an incorrect DNS configuration can prevent a domain-joined workstation from communicating properly with Active Directory.

Through systematic troubleshooting, I identified the DNS configuration issue, corrected the workstation's DNS settings, and verified domain connectivity.

This exercise reinforced the importance of DNS in Active Directory environments and provided hands-on experience with common Help Desk troubleshooting procedures.
