SecurityEvents Analytics Rules

Data sources: 
- Windows and Linux Security Event Logs

Modified policies:
| Policy  | Modified value | Justification |
| ------------- | ------------- | ------------- |
| RDP Nesting | Query | JumpHosts watchlist exclusions integration |
| Rare RDP Connections | Query | JumpHosts watchlist exclusions integration |
| Non Domain Controller Active Directory Replication | Query | NonDomainControllerReplicationExclusion watchlist exclusions integration |
| Multiple Password Reset by user | "createIncident": false  | Too many incidents, but alerts are of interest on demand |

Watchlists:
| Policy  | Watchlist | SearchKey | value type |
| ------------- | ------------- | ------------- | ------------- |
| Non Domain Controller Active Directory Replication | NonDomainControllerReplicationExclusion | NonDomainControllerReplicationExclusion | excluded user upn |
| RDP Nesting | JumpHosts | JumpHosts | excluded hosts fqdn |
| Rare RDP Connections | JumpHosts | JumpHosts | excluded hosts fqdn |

