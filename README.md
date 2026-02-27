# HSO: High Speed Offloader/Onloader for Smartsheet
The bulk data movement solution for efficiently moving bulk data in and out of Smartsheet, effortlessly overcoming the platform's inherent 100-item limitation.

## Features

1. **Inter Region** Operate and move data accross Smartsheet regions, [not possible]: [https://github.com](https://help.smartsheet.com/articles/2482447-migrating-data-across-regions) natively from Smartsheet
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
| when to use   | incrementals cannot maintain high attachment ratios   | high speed snapshots or bulk offloads of attachments |
| Input format  | Sheets, Attachments, Reports, Dashboards, Folders | Attachments |
| Output format | ZIP file for every sheet                          | Flat folder |


## Operations

1. Offload behaviour is driven from a YML configuration file.  If none specified it assume there will be a config file called `dmp_config.yml` in the runtime folder. 
   If not processing will stop with an error.
2. Optionally a YML configuration file can be selected by specifying a run-time paramater and path to the file `-c="c:\path\myconfig.yml"`
   This way every runtime instance can be driven from different parameters
   
### configuration file


