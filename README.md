# Mini Project- Secure User Access Management in Linux 

This mini project focuses on implementing secure user and group-based access control in a Linux environment using system commands and Access Control Lists (ACL). It simulates real-world identity and access management (IAM) practices in two practical lab scenarios, emphasizing permission control, user isolation, and compliance with security policies.

📁 Lab 1: User-Specific File Access Control
Objective: Ensure only the CTO, Mr. Penny Johnson (pjohnson), has access to a confidential file.

Created user pjohnson and project directory.

Moved noida.txt to the directory and set restrictive permissions.

Used setfacl to grant pjohnson exclusive read/write/execute rights.

Verified that no other user could access the file.

Key Commands Used:

adduser, mkdir, cp, chmod, setfacl, su

📁 Lab 2: Multi-User and Group-Based Permission Management
Objective: Manage access rights for users from three Indian states (Goa, Delhi, Gujarat) using ACLs and group settings.

Created users: stefi, aravind, and jignesh, and group: citizen.

Assigned tailored permissions on extracted folders from government.zip:

Gujarat: Full access to jignesh, read/execute only for aravind.

Delhi: Denied all access to stefi.

Goa:

anjuna.txt: stefi can write, aravind can read.

candolim.txt: jignesh can write, stefi can read.

Validated all permission restrictions using su and command-line checks.

Key Concepts Applied:

Linux file permissions and ACLs

User and group management

Fine-grained access enforcement

Security validation with multi-user simulation

🛠️ Tools & Techniques
Linux CLI (Ubuntu/Debian)

adduser, usermod, chmod, setfacl, getfacl

Group management and permission verification

🎯 Purpose
To strengthen practical understanding of user identity and access management in Linux systems. This project demonstrates how to securely assign and verify user-level access to sensitive files, which is crucial in organizational and governmental IT infrastructures.

