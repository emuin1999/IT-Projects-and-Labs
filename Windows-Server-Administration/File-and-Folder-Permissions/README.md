# Project: Configuring Shared Folder Permissions

## Objective
Create shared folders and assign permissions to control which users can access, view, modify, and manage department files in a Windows Server Active Directory environment.

## Project Overview
In this project, I created shared folders for different departments and configured Share and NTFS permissions to control access to company resources.

I used Active Directory security groups to assign permissions based on employee roles and responsibilities. I completed two scenarios involving restricted access to department folders.

- **Scenario 1:** Configure read-only access for HR Interns so they can view HR department files without modifying or deleting them.
- **Scenario 2:** Restrict access to the IT Department's Licenses subfolder so that only senior IT staff can access it.

I tested both scenarios using different domain user accounts to verify that permissions were working as expected.

## Tools & Technologies Used
- **Windows Server:** Hosted and managed shared department folders.
- **Active Directory Users and Computers (ADUC):** Created and managed security groups and user accounts.
- **Active Directory Security Groups:** Assigned folder permissions based on employee roles.
- **Share Permissions:** Controlled access to shared folders over the network.
- **NTFS Permissions:** Controlled access to files and folders, including read, modify, and full control.
- **Windows 11:** Client machine used to test folder access with different domain accounts.

---

## Scenario 1: HR Intern Read-Only Access

### Objective
An HR Intern needs access to the HR Team shared drive to view department files but should not be able to modify, delete, or create files and folders.

### How I Resolved It

1. **Created an HR Intern Security Group:** Created an Active Directory security group named HR Interns and added the appropriate users.
2. **Configured Share Permissions:** Granted the HR Interns group read-only access to the HR shared folder.
3. **Configured NTFS Permissions:** Assigned read-only NTFS permissions to the HR Interns group.
4. **Tested Folder Access:** Logged into the Windows 11 client using HR Intern credentials.
5. **Verified Restrictions:** Attempted to delete existing files and create new folders to confirm that the read-only restrictions were enforced.

### Expected Result
HR Interns can access and view HR department files but cannot modify, delete, or create files and folders.

---

## Scenario 2: Restrict Access to the IT Licenses Folder

### Objective
All IT technicians need access to the Software Repository folder named `Software`, but only senior IT staff should be able to access the `Licenses` subfolder.

### How I Resolved It

1. **Created a Senior IT Security Group:** Created an Active Directory security group named IT-SeniorStaff.
2. **Created the Licenses Subfolder:** Created a separate `Licenses` subfolder inside the IT Software Repository.
3. **Configured Share Permissions:** Granted the IT-SeniorStaff group Full Control on the shared resource and removed the Everyone group from the share permissions.
4. **Configured NTFS Permissions:** Assigned Full Control to the IT-SeniorStaff group on the Licenses subfolder.
5. **Tested Restricted Access:** Used a non-IT-SeniorStaff domain account to attempt to access the Licenses folder.
6. **Verified Permissions:** Confirmed that users outside the IT-SeniorStaff group could not access the restricted folder.

### Expected Result
All authorized IT technicians can access the Software Repository, but only members of IT-SeniorStaff can access the Licenses subfolder.

---

## What I Learned

Through these scenarios, I gained hands-on experience managing shared folder access in a Windows Server environment using Active Directory security groups, Share Permissions, and NTFS Permissions.

In Scenario 1, I learned how to create an Active Directory security group and assign read-only access to department resources. I configured both Share and NTFS permissions for HR Interns and tested their access using a domain account. By attempting to delete files and create new folders, I verified that users could view the contents without making unauthorized changes.

In Scenario 2, I learned how to create restricted subfolders and use security groups to control access to sensitive department information. I created the IT-SeniorStaff group and configured the Licenses folder so that only senior IT employees had Full Control. I also tested access using a regular IT account to verify that users outside the authorized group could not access the restricted folder.

An important lesson from this project was understanding the relationship between Share Permissions and NTFS Permissions. When users access folders over the network, both permission sets apply, and the more restrictive effective permissions determine what users can do.

These exercises helped me understand how IT administrators use security groups and folder permissions to protect company information, enforce least-privilege access, and ensure employees only access resources required for their job responsibilities.

---

## Screenshot Checklist

The following screenshots document both scenarios and demonstrate that the folder permissions were configured and tested successfully.

### Scenario 1: HR Intern Read-Only Access

| # | Screenshot | What It Proves |
|---|---|---|
| 01 | Create HR Intern Group | Shows the creation of the HR Interns security group and the addition of users. |
| 02 | HR Intern Share Permissions | Demonstrates that the HR Interns group was assigned Read-only Share Permissions. |
| 03 | HR Intern NTFS Permissions | Shows Read-only NTFS permissions assigned to the HR Interns group. |
| 04 | HR Intern Delete Action Denied | Demonstrates that HR Interns cannot delete existing files. |
| 05 | HR Intern Modify Folder Denied | Demonstrates that HR Interns cannot create new folders or modify existing content. |

### Scenario 2: Restrict Access to the IT Licenses Folder

| # | Screenshot | What It Proves |
|---|---|---|
| 06 | Created IT Senior Group | Shows the creation of the IT-SeniorStaff security group for senior IT employees. |
| 07 | Created Licenses Folder | Demonstrates the creation of the restricted Licenses subfolder inside the Software Repository. |
| 08 | IT Senior Group Share Permissions | Shows Full Control Share Permissions assigned to IT-SeniorStaff and the removal of Everyone. |
| 09 | IT Senior Group NTFS Permissions | Demonstrates Full Control NTFS permissions assigned to IT-SeniorStaff on the Licenses folder. |
| 10 | Non-IT-SeniorStaff Folder Access Denied | Shows an access-denied result when a user outside the IT-SeniorStaff group attempts to access the Licenses folder. |

---

## Final Verification

After configuring the permissions, I tested both scenarios using different domain user accounts on the Windows 11 client machine.

**Scenario 1 Results:**
- HR Interns could access and view HR department files.
- HR Interns could not delete files or create new folders.

**Scenario 2 Results:**
- Regular IT technicians could access the Software Repository.
- Only IT-SeniorStaff members could access the restricted Licenses folder.
- Unauthorized users were denied access to the restricted subfolder.

The results demonstrated how Active Directory security groups, Share Permissions, and NTFS Permissions can work together to control access to company resources.

**Project Status:** Completed
