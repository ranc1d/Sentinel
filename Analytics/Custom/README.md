Custom Analytics Rules

Data sources: 
- Windows and Linux Security Event Logs

Modified policies:
| Policy  | Modified value | Justification |
| ------------- | ------------- | ------------- |
| Mails containing malicious urls | Query | external watchlist |

Watchlists:
| Policy  | Watchlist | SearchKey | value type |
| ------------- | ------------- | ------------- | ------------- |
| Break the glass admin account used for signin | BreakGlassAccounts | BreakGlassAccounts | admin upn |
