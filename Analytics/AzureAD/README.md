AzureAD Analytics Rules

Data sources: 
- AzureAD SigninLogs

Modified policies:
| Policy  | Modified value | Justification |
| ------------- | ------------- | ------------- |
| Attempt to bypass conditional access rule in Azure AD  | "enabled": false  | Too many incidents with conditional access trusted location exclusions  |
| Successful logon from IP and failure from a different IP  | "createIncident": false  | Too many incidents, but alerts are of interest on demand |
| User Assigned Privileged Role | "createIncident": false  | Managed via PIM Mails, but alerts are of interest on demand |
| User added to Azure Active Directory Privileged Groups | "createIncident": false  | Managed via PIM Mails, but alerts are of interest on demand |
