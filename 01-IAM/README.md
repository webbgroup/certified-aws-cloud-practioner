## IAM stands for Identity Access Management
It is Global - you do not need to specify a region when dealing with IAM. When you create a user or group it is GLOBAL

Access the platform 3 ways
* Via the Console
* Programmatically via command line
* Using the Software Developers Kit

Root account is used to set up Access for others.
Secure it via multi-factor auth

Group is where you store your users
Apply Policies to the Group, and Policies are in JSON Notation.
 {"name":"A Cloud Guru"}


## IAM Best Practices

- Root Account - Only use root account to create the AWS account. Do not use it to login.
- Users - One user account should equal one real human being. No phantom users.
- User Group Policies - Always place users in groups, and then apply policies to the groups. This makes management easier.
- Password Policies - Have a strong password rotation policy
- MFA - Always enable MFA wherever possible
- Roles - Use roles to access various other AWS services.
- Access Keys - Use access keys for programmatic access to AWS.
- IAM Credential Report - Use IAM credential reports to audit the permissions of your users/accounts.

## IAM Credential Reports

If you have a large amount of users and what password policies are turned on and how to export it.
Audit or Export it is to use the credential report.
Passwords, Access Keys, and MFA



