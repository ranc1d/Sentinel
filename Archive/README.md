# Modifications and watchlists

Modified policies:
| Policy  | Modified value | Justification |
| ------------- | ------------- | ------------- |
| RDP Nesting | Query | JumpHosts watchlist exclusions integration |
| Rare RDP Connections | Query | JumpHosts watchlist exclusions integration |
| Non Domain Controller Active Directory Replication | Query | NonDomainControllerReplicationExclusion watchlist exclusions integration |
| Multiple Password Reset by user | "createIncident": false  | Too many incidents, but alerts are of interest on demand |
| AD user enabled and password not set within 48 hours | "createIncident": false  | Too many incidents, but alerts are of interest on demand |
| SecurityEvent - Multiple authentication failures followed by a success | "createIncident": false  | Too many incidents, but alerts are of interest on demand |
| SharePointFileOperation via devices with previously unseen user agents | "createIncident": false  | Too many incidents, but alerts are of interest on demand |
| SharePointFileOperation via previously unseen IPs | "createIncident": false  | Too many incidents, but alerts are of interest on demand |
| Attempt to bypass conditional access rule in Azure AD | "enabled": false  | Too many incidents with conditional access trusted location exclusions  |
| Successful logon from IP and failure from a different IP | "createIncident": false  | Too many incidents, but alerts are of interest on demand |
| Failed host logons but success logon to AzureAD | "createIncident": false  | Too many incidents, but alerts are of interest on demand |
| Failed AzureAD logons but success logon to host | "createIncident": false  | Too many incidents, but alerts are of interest on demand |
| User Assigned Privileged Role | "createIncident": false  | Managed via PIM Mails, but alerts are of interest on demand |
| User added to Azure Active Directory Privileged Groups | "createIncident": false  | Managed via PIM Mails, but alerts are of interest on demand |
| Mails containing malicious urls | Query | external watchlist |
| Missing Domain Controller Heartbeat | Query | DomainControllers watchlist integration |
| Failed logon attempts by valid accounts within 10 mins | Query | FailedLogonExclusions watchlist integration |
| Exchange workflow MailItemsAccessed operation anomaly | Query | ExchangeWorkflowAnomalyExclusions watchlist integration |
| Non Domain Controller Active Directory Replication | "queryPeriod": "P1D" | Opening incidents for old events |
| Mass secret retrieval from Azure Key Vault | Query | MassSecretRetrievalExclusions watchlist integration |
| User account added to built in domain local or global group | Query | MAC-address exclusion and AccountAddedToBuildinGroupOuExclusion watchlist integration |

Watchlists:
| Policy  | Watchlist | SearchKey | value type |
| ------------- | ------------- | ------------- | ------------- |
| Non Domain Controller Active Directory Replication | NonDomainControllerReplicationExclusion | NonDomainControllerReplicationExclusion | excluded user upn |
| RDP Nesting | JumpHosts | JumpHosts | excluded hosts fqdn |
| Rare RDP Connections | JumpHosts | JumpHosts | excluded hosts fqdn |
| Break the glass admin account used for signin | BreakGlassAccounts | BreakGlassAccounts | admin upn |
| Missing Domain Controller Heartbeat | DomainControllers | DomainControllers | domain controller fqdn |
| Failed logon attempts by valid accounts within 10 mins | FailedLogonExclusions | Computername | end device fqdn |
| Exchange workflow MailItemsAccessed operation anomaly | ExchangeWorkflowAnomalyExclusions | UserId | excluded user upn |
| Mass secret retrieval from Azure Key Vault | MassSecretRetrievalExclusions | AppId | excluded azure app id |
| User account added to built in domain local or global group | AccountAddedToBuildinGroupOuExclusion | OuDistinguishedName | distinguished name of excluded ou |
