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
- Configure the HR Folder share and NTFS permission to only allow read access.
- Verify the permission using HR Intern credentials on client machine.  
