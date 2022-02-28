AzureAD Analytics Rules

Data sources: 
- AzureAD SigninLogs

Modified policies:
| Policy  | Modified value | Justification |
| ------------- | ------------- | ------------- |
| Attempt to bypass conditional access rule in Azure AD  | "enabled": false  | Too many incidents with conditional access trusted location exclusions  |
| Successful logon from IP and failure from a different IP  | "createIncident": false  | Too many incidents |
