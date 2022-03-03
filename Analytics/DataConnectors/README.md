Data Connectors Analytics Rules

Data sources: 
- Heartbeat

Modified policies:
| Policy  | Modified value | Justification |
| ------------- | ------------- | ------------- |
| Missing Domain Controller Heartbeat | Query | DomainControllers watchlist integration |

Watchlists:
| Policy  | Watchlist | SearchKey | value type |
| ------------- | ------------- | ------------- | ------------- |
| Missing Domain Controller Heartbeat | DomainControllers | DomainControllers | domain controller fqdn |
