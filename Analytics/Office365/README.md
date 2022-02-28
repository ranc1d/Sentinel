Office365 Analytics Rules

Data sources: 
- Office362 Activity Logs

Modified policies:
| Policy  | Modified value | Justification |
| ------------- | ------------- | ------------- |
| SharePointFileOperation via devices with previously unseen user agents | "createIncident": false  | Too many incidents, but alerts are of interest on demand |
