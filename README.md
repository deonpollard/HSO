# HSO: High Speed Offloader/Onloader for Smartsheet
The bulk data movement solution for efficiently moving bulk data in and out of Smartsheet, effortlessly overcoming the platform's inherent 100-item limitation.

When used in conjunction with SmartBackup, HSO increases accuracy, mitigates risks, and helps with compliance requirements. In stand-alone mode, HSO excels as a bulk data migrator, take-on engine, or solution duplicator.

## Features

1. **Inter Region** Operate and move data accross Smartsheet regions, something [not possible](https://help.smartsheet.com/articles/2482447-migrating-data-across-regions) natively from Smartsheet
2. **Intra Region** Data can be copied/moved based on Workspace/s or User/s or Account, something not possible using Smartsheet DataShuttle which only operate at sheet level.
3. Package as part of the **SmartBackup** suite, now comprising of:
   - Backup
   - Archive
   - Export
   - Offload
  
## When to use

| Use Case      | Description   |
| ------------- |:-------------:|
| Data Center Migration | HSO enables organizations to migrate Account data between Smartsheet Regions, overcoming a challenge that is nearly impossible to address within the current Smartsheet environment. | 
| Offline Backups | When used together with SmartBackup, HSO can provide complete, full offline backup copies of all your Smartsheet data, for long-term storage in a secure offline location, while SmartBackup backs up and exports your recently used sheets and dashboards. | 
| Daily Solution copies | Leverage HSO to generate daily snapshot copies and offloads of your critical projects and solutions. This feature ensures comprehensive audit tracking and facilitates seamless data restoration when needed. | 
| Data Center Migration | HSO enables organizations to migrate Account data between Smartsheet Regions, overcoming a challenge that is nearly impossible to address within the current Smartsheet environment. | 
| Data Center Migration | HSO enables organizations to migrate Account data between Smartsheet Regions, overcoming a challenge that is nearly impossible to address within the current Smartsheet environment. | 
| Data Center Migration | HSO enables organizations to migrate Account data between Smartsheet Regions, overcoming a challenge that is nearly impossible to address within the current Smartsheet environment. | 
| Data Center Migration | HSO enables organizations to migrate Account data between Smartsheet Regions, overcoming a challenge that is nearly impossible to address within the current Smartsheet environment. | 
| Data Center Migration | HSO enables organizations to migrate Account data between Smartsheet Regions, overcoming a challenge that is nearly impossible to address within the current Smartsheet environment. | 

### Data Center Migration
1. HSO enables organizations to migrate Account data between Smartsheet Regions, overcoming a challenge that is nearly impossible to address within the current Smartsheet environment.

    
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


