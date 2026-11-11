# Configuring Shared Folder Permissions
Objective: Create shared folders and assign permissions to control which users can access, view, and modify department files.

What I did:
- Created shared folders for different departments.
- Configured folder sharing and security permissions.
- Assigned appropriate access permissions to department security groups.
- Grant each department full control share and NTFS permissions. 
- Tested folder access to make sure users had the correct level of access.

### Scenario 1:
A HR Intern needs access to the HR Team shared drive folders to view contents but should not modify or delete files. 

How I resolved it: 
- Created an HR Intern Group and added users.
- Give HR Interns users access to the shared drive.
- Configure the HR Folder share and NTFS permission to only allow read access for HR Interns Group.
- Verify the permission using HR Intern credentials on client machine.

### Scenario 2: 
In the IT Department, all techs need access to the Software Repository folder called Software, but only senior IT staff should be able to access the "Licenses" subfolder

How I resolved it: 
- Created Senior IT Staff Group.
- Created the Licenses subfolder
- Only grant Senior IT Staff full control for both share and NTFS permissions.
- Test a non-Senior IT Staff account to access the Licenses subfolder.

What I Learned: 
Through these scenarios, I learned how to manage access to shared folders in a Windows Server environment using Active Directory security groups, Share Permissions, and NTFS Permissions.

In Scenario 1, I created an HR Intern security group and assigned users to it. I configured both Share and NTFS permissions to provide read-only access. I then tested the permissions by attempting to delete files and create new folders. These tests helped me understand how permissions restrict users from making unauthorized changes to shared resources.

In Scenario 2, I created an IT-SeniorStaff security group and a separate Licenses folder for senior IT employees. I configured Share and NTFS permissions to give the IT-SeniorStaff group full control while removing the Everyone group from the share permissions. I also tested access using a non-IT-SeniorStaff account to confirm that unauthorized users could not access the restricted folder.

These exercises helped me understand how IT administrators use security groups and folder permissions to protect company information and ensure employees only access resources they are authorized to use.
