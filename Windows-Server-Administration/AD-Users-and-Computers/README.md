# Project: Creating Active Directory Users, Groups, and Organizational Units (OUs)

## Objective
Organize Active Directory users and computers into separate departments to simplify user management, group administration, and Group Policy implementation.

## Project Overview
In this project, I created a structured company environment in Active Directory using Organizational Units (OUs), domain user accounts, and security groups.

I established a company OU named `LexCorp` and created three departmental OUs: HR, IT, and Sales. I then created domain users, departmental security groups, and folder access groups for each department.

I also implemented nested security groups using the AGDLP model to separate user identities from resource permissions. This approach allows administrators to manage access to shared resources more efficiently without assigning permissions to individual user accounts.

## Tools & Technologies Used
- **Windows Server:** Hosted and managed the Active Directory environment.
- **Active Directory Domain Services (AD DS):** Provided centralized user and group management.
- **Active Directory Users and Computers (ADUC):** Created and managed users, groups, and Organizational Units.
- **Organizational Units (OUs):** Organized users and groups by department.
- **Active Directory Security Groups:** Managed departmental membership and resource access.
- **AGDLP:** Used nested security groups to organize permissions and manage access to shared resources.

## What I Did

1. **Created the Company OU:** Opened Active Directory Users and Computers (ADUC) and created a company Organizational Unit named `LexCorp`.
2. **Created Departmental OUs:** Established three departmental OUs under LexCorp: HR, IT, and Sales.
3. **Created Departmental Security Groups:** Created security groups for each department to organize employee accounts.
4. **Created Folder Access Groups:** Created separate groups to manage access to departmental shared folders and resources.
5. **Created Domain Users:** Created employee accounts for each department and organized them within their respective OUs.
6. **Configured Nested Groups:** Added users to their departmental security groups and nested those groups inside the appropriate folder access groups.
7. **Established a Structured Directory:** Organized users and groups to simplify account administration, resource management, and future Group Policy configuration.

## Group Management: Understanding AGDLP

I used the AGDLP model to organize security groups and manage access to shared resources.

AGDLP stands for:

- **A – Accounts:** Individual domain user accounts.
- **G – Global Groups:** Groups that organize users based on their department or job responsibilities.
- **DL – Domain Local Groups:** Groups used to assign permissions to specific domain resources.
- **P – Permissions:** Access rights assigned to resources such as shared folders.

### Example: HR Department

The following structure demonstrates how an HR employee receives access to departmental resources:

```text
HR Employee Account
        |
        v
HR Global Security Group
        |
        v
HR Folder Access Group
(Domain Local Group)
        |
        v
HR Shared Folder Permissions
```

This structure separates employee accounts from resource permissions.

Instead of assigning folder permissions to individual employees, administrators assign permissions to the Folder Access Group. Users receive access through their group memberships.

The same structure can be applied to the IT and Sales departments.

## What I Learned

Through this project, I gained hands-on experience creating and organizing a company structure in Active Directory using Organizational Units (OUs).

I learned how to create a company OU named LexCorp and establish separate departmental OUs for HR, IT, and Sales. This helped me understand how administrators organize domain users and groups to make account management easier.

I also learned how to create domain user accounts, departmental security groups, and Folder Access Groups for each department.

One of the most important concepts I practiced was nested group management using the AGDLP model. I learned how to add users to their departmental security groups and nest those groups inside Folder Access Groups. This allows administrators to manage resource permissions through groups rather than assigning permissions to individual users.

Finally, I learned how a properly structured Active Directory environment makes it easier to manage employees, assign shared folder permissions, and apply Group Policy to specific departments.

This project strengthened my understanding of Active Directory administration, Organizational Units, security group management, nested groups, and centralized access control.

## Screenshot Checklist

The following screenshots document the Active Directory configuration process and demonstrate how the company directory was organized.

| # | Screenshot | What It Proves |
|---|---|---|
| 01 | Create Company OU | Shows the creation of the main company Organizational Unit named LexCorp. |
| 02 | Create Three Departmental OUs | Demonstrates the creation of HR, IT, and Sales Organizational Units under LexCorp. |
| 03 | Create Groups for Each Department | Shows the creation of departmental security groups and Folder Access Groups. |
| 04 | Configure Nested Groups | Demonstrates how departmental security groups
