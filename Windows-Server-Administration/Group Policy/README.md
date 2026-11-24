# Project: Configuring and Managing Group Policy

## Objective
Apply security restrictions and automate user configurations through Group Policy in a Windows Server Active Directory environment.

## Project Overview
In this project, I configured and managed Group Policy Objects (GPOs) to enforce security settings and automate network resource access for domain users.

I created password and account lockout policies, restricted Control Panel access, and configured automatic network drive mapping using Group Policy Preferences and Item-Level Targeting.

I then linked the GPOs to the appropriate Organizational Units (OUs), refreshed Group Policy settings, and verified that the policies were successfully applied to a Windows 11 client machine.

## Tools & Technologies Used
- **Windows Server:** Managed Active Directory and Group Policy.
- **Active Directory Domain Services (AD DS):** Managed domain users, groups, and Organizational Units.
- **Group Policy Management Console (GPMC):** Created, configured, and linked GPOs.
- **Group Policy Preferences:** Automated network drive mapping.
- **Item-Level Targeting:** Assigned network drives based on user or group membership.
- **Windows 11:** Client machine used to test and verify Group Policy settings.
- **Command Prompt:** Used `gpupdate /force` to refresh Group Policy settings.

## What I Did

1. **Configured Password Policy:** Created a Group Policy Object to enforce password security requirements, including password complexity.
2. **Configured Account Lockout Policy:** Established account lockout thresholds, allowed failed login attempts, and configured account lockout duration.
3. **Restricted Control Panel Access:** Configured Group Policy to prevent users from accessing Control Panel and making unauthorized system configuration changes.
4. **Configured Automatic Network Drives:** Set up automatic network drive mapping for domain users.
5. **Configured Item-Level Targeting:** Used Item-Level Targeting to assign specific network drives based on user or security group membership.
6. **Configured Drives Using Group Policy Preferences:** Created and managed mapped network drives through Group Policy Preferences.
7. **Applied GPOs to Organizational Units:** Linked the configured Group Policy Objects to the appropriate OUs within Active Directory.
8. **Refreshed Group Policy:** Used the `gpupdate /force` command on the Windows 11 client to manually refresh Group Policy settings.
9. **Verified Group Policy Settings:** Tested the client machine to confirm that the Control Panel restriction and other configured policies were successfully applied.

## What I Learned

By completing this project, I gained hands-on experience configuring and managing Group Policy Objects (GPOs) in a Windows Server Active Directory environment.

I learned how administrators use Group Policy to enforce security requirements and control how users interact with domain computers. I practiced configuring password policies and account lockout policies to strengthen account security and help prevent unauthorized access.

I also learned how to restrict Control Panel access through Group Policy to prevent users from making unwanted changes to system settings.

Another important skill I developed was automating network drive mapping using Group Policy Preferences. I explored Item-Level Targeting, which allows administrators to assign specific network drives based on user or security group membership rather than applying the same configuration to everyone.

Finally, I learned how to link GPOs to the appropriate Organizational Units, refresh policies using `gpupdate /force`, and verify that the configurations were successfully applied to a Windows 11 client machine.

This project strengthened my understanding of Windows Server administration, Active Directory, security policy management, network resource automation, and Group Policy troubleshooting.

## Screenshot Checklist

The following screenshots document the configuration process and demonstrate that the Group Policy settings were successfully implemented.

| # | Screenshot | What It Proves |
|---|---|---|
| 01 | Configure Password Policy GPO | Shows password requirements and complexity settings configured through Group Policy. |
| 02 | Configure Account Lockout Policy | Shows the configured account lockout threshold, duration, and failed login attempt limit. |
| 03 | Restrict Control Panel | Demonstrates the Group Policy setting used to restrict Control Panel access. |
| 04 | Configure Automatic Network Drives | Shows the configuration of automatic network drive mapping for domain users. |
| 05 | Configure Network Drives Using Item-Level Targeting | Demonstrates how Item-Level Targeting assigns network drives based on specific conditions. |
| 06 | Configure Drives Using Group Policy Preferences | Shows mapped drives created and managed through Group Policy Preferences. |
| 07 | Apply GPOs to OUs | Demonstrates that the Group Policy Objects were linked to the appropriate Organizational Units. |
| 08 | Refresh Group Policy | Shows the `gpupdate /force` command used to refresh Group Policy settings. |
| 09 | Verify That GPOs Work | Demonstrates that the Control Panel restriction was successfully enforced on the Windows 11 client machine. |

## Final Verification

After configuring and applying the Group Policy Objects, I refreshed the client machine using:

```cmd
gpupdate /force
```

I then tested the Windows 11 client to verify that the configured restrictions were enforced.

The project demonstrated how Group Policy can be used to:
- Enforce password and account security requirements.
- Restrict access to Windows system settings.
- Automatically map network drives.
- Assign resources based on user and security group membership.
- Centrally manage domain user configurations.

**Project Status:** Completed
