# aws-iam-user-management

# What it does ?
- This will allow users to access AWS resources only if we authenticate through MFA
- Each user will not able to change another user's "login credentials", so that he cannot do any illegial activities on another user account
- Each user cannot able to create any group, user, role, policies. So that he cannot modify his permission as admin and do any illegal activities

# What we need to do ?
Create group called "CustomizedAdminAccess"
Under this group attach below two policies
- admin-access-to-all-services-except-usergroups-and-users
- all-users-force-mfa
