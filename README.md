# Offload
High speed Smartsheet offload facility catering for Sheet Attachments.  Capability allows one to *offload* all
or selected attachments for one or more Users from Smartsheet to local storage.

## Early Positioning

1. Initially called **DUMP** whilst in early Beta
2. Leaning towards the name **OFFLOAD**, sounds better, more valuable
3. Package as part of the **SmartBackup** suite, now comprising of:
   - Backup
   - Archive
   - Export
   - Offload 
    
Although Export and Offload functionally appears to do the same thing they are build for different outcomes

| Synopsis       | Export        | Offload  |
| ------------- |:-------------:| -----:|
| Function      | Copies data from Smartsheet to local storage | Copies data from Smartsheet to local storage | 
| Input format  | Sheets, Attachments, Reports, Dashboards, Folders | Attachments |
| Output format | ZIP file for every sheet                          | Flat folder |

