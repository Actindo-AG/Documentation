[!!DataHub](DataHub)
[!!Omni-Channel](Channels)

# Manage the ETL processes

When an ETL attribute mapping has been triggered, the corresponding ETL processes are displayed in the *ETL PROCESSES* tab. You can check the status of a current ETL process, confirm a pending ETL process and restart a faulty ETL process.  


## Check the ETL process status

After an ETL process has been triggered, the current status is displayed in the *ETL PROCESSES* tab. An ETL process can have the following statuses:
- Todo
- Error
- Done
- Destination frozen
- Awaiting confirmation
- Synchronous
- Awaiting confirmation different user
- Semi-automatic accepted
You can check the current status of an ETL process to approve that any changes are applied or if any further actions are required.  

### Prerequisites

An ETL process has been triggered, for instance by a rerun of mapping, see [Rerun an ETL mapping](01_ManageETLMappings.md#rerun-an-etl-mapping).

### Procedure
*DataHub > Settings > Tab ETL PROCESSES*

![ETL processes](/Assets/Screenshots/DataHub/Settings/ETLProcesses/ETLProcesses.png "[ETL processes]")

1. Check the list for the appropriate ETL process and note its status.

2. Click the *Status Filter* drop-down list and select the status of the respective ETL process in the list. The following statuses are available in the list:
  - **Todo**: All pending ETL processes are displayed.
  - **Error**: All faulty ETL processes are displayed.
  - **Done**: All completed ETL processes are displayed.
  - **Destination frozen**: All ETL processes, whose destination attribute is blocked because the corresponding entity is opened by a user, are displayed.
  - **Awaiting confirmation**: All ETL processes that must be confirmed are displayed.
  - **Synchronous**: All ETL processes that are executed synchronously are displayed for the duration of processing.
  - **Awaiting confirmation different user**: All ETL processes that must be confirmed by another user than the creator are displayed.
  - **Semi-automatic accepted**: All ETL processes have been confirmed are displayed.   

  All ETL processes of the selected status are displayed.

3. Depending on the status of the ETL process, continue with one of the following actions:
  - [Confirm an ETL process](#confirm-an-etl-process)
  - [Retry a faulty ETL process](#retry-a-faulty-etl-process)
  - [Return to the ETL Mapping](01_ManageETLMappings.md)

### Next steps

- [Confirm an ETL process](#confirm-an-etl-process)
- [Retry a faulty ETL process](#retry-a-faulty-etl-process)
- [Manage the HTML templates](03_ManageHTMLTemplates.md)
- [Manage the dashboards](04_ManageDashboards.md)

### See also

- [User Interface DataHub](/DataHub/UserInterface/00_UserInterface.md)
- [Manage the ETL mappings](01_ManageETLMappings.md)



## Confirm an ETL process

If the selected change tracking mode of an ETL mapping equals **semi-automatic** or **semi-automatic, changes must be confirmed by another user**, the ETL process has to be confirmed before the mapping can be rerun.

### Prerequisites

- An ETL process has been triggered, for instance by a rerun of mapping, see [Rerun an ETL mapping](01_ManageETLMappings.md#rerun-an-etl-mapping).
- At least one of the triggered ETL processes has the change tracking mode **semi-automatic** or **semi-automatic, changes must be confirmed by another user**.

### Procedure
*DataHub > Settings > Tab ETL PROCESSES*

![ETL processes](/Assets/Screenshots/DataHub/Settings/ETLProcesses/ETLProcesses.png "[ETL processes]")

1. Check the list for the appropriate ETL process to make sure that the ETL process has been triggered.

  > [Info] ETL processes whose mappings have a **semi-automatic** change tracking mode are listed with the *Awaiting confirmation* status, those having a **semi-automatic, changes must be confirmed by another user** change tracking mode are listed with the *Awaiting confirmation different user* status.

2. Switch to the *Omni-Channel* module: *Omni-Channel > Offers > Tab SEMI AUTOMATIC MAPPING* .      
  The *SEMI AUTOMATIC MAPPING* tab is displayed.

3. Click the ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button to update the list of pending mappings.   
  The list is updated and all pending mappings are displayed.

  ![Semi automatic mapping](/Assets/Screenshots/Channels/Offers/SemiAutomaticMapping/SemiAutomaticMapping.png "[Semi automatic mapping]")

4. Select the checkboxes of the mappings in the list, you want to confirm.   
  The editing toolbar is displayed above the list.

5. Click the [CONFIRM] button in the editing toolbar.   
  The selected mappings are removed from the list. The mappings are applied. The confirmed mappings are displayed in the *ETL PROCESSES* tab of the *Datahub* module with the **Semi-automatic accepted** status.

  > [Info] If the ETL mappings should not be applied, click the [REJECT] button in the editing toolbar instead. The selected mappings are removed from the list without being rerun.

[comment]: <> (doesn't work for me. Why not displayed in the accepted list in datahub?)

### Next steps

- [Retry a faulty ETL process](#retry-a-faulty-etl-process)
- [Manage the HTML templates](03_ManageHTMLTemplates.md)
- [Manage the dashboards](04_ManageDashboards.md)

### See also

- [User Interface DataHub](/DataHub/UserInterface/00_UserInterface.md)
- [User Interface Omni-Channel](/Channels/UserInterface/00_UserInterface.md)
- [Check the ETL process status](#check-the-etl-process-status)
- [Manage the ETL mappings](01_ManageETLMappings.md)



## Retry a faulty ETL process

If an ETL process has been canceled because of an error, the respective process is displayed in the *ETL PROCESSES* tab with the **Error** status.

### Prerequisites

An ETL process has been canceled because of an error. When the error has been fixed, you can restart the ETL process to rerun the corresponding mapping.

### Procedure
*DataHub > Settings > Tab ETL PROCESSES*

![ETL processes](/Assets/Screenshots/DataHub/Settings/ETLProcesses/ETLProcesses.png "[ETL processes]")

1. Click the *Status Filter* drop-down list and select the **Error** status in the list.
  All ETL processes with the **Error** status are displayed.

  ![Error processes](/Assets/Screenshots/DataHub/Settings/ETLProcesses/Error.png "[Error processes]")

2. Select the checkbox of the mapping you want to restart.   
  The editing toolbar is displayed above the list.

  [comment]: <> (why can I only select one mapping and not several mappings at a time?)

3. Click the [RETRY] button in the editing toolbar.   
  The selected mapping is restarted. The pop-up window *Process will be retried shortly* is displayed.

  ![Process retried](/Assets/Screenshots/DataHub/Settings/ETLProcesses/ProcessRetried.png "[Process retried]")

  If the rerun is successful, the mapping status changes to **Done** and it is removed from the list of mappings with the **Error** status.

### Next steps

- [Manage the HTML templates](03_ManageHTMLTemplates.md)
- [Manage the dashboards](04_ManageDashboards.md)

### See also

- [User Interface DataHub](/DataHub/UserInterface/00_UserInterface.md)
- [Check the ETL process status](#check-the-etl-process-status)
- [Confirm an ETL process](#confirm-an-etl-process)
- [Manage the ETL mappings](01_ManageETLMappings.md)
