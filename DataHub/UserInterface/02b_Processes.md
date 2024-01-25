[!!Manage the ETL processes](../Operation/02_ManageETLProcesses.md)
[!!Retry a faulty ETL process](../Troubleshooting/01_RetryFaultyETLProcess.md)

# Processes

*DataHub > ETL > Tab PROCESSES*

![ETL processes](../../Assets/Screenshots/DataHub/Settings/ETLProcesses/ETLProcesses.png "[ETL processes]")

**ETL processes**

Depending on the selection in the *Status filter* drop-down list, the ETL processes list displays all processes with the selected status. Depending on the settings, the displayed columns may vary. All fields are read-only.

- *Status filter*   
    Click the drop-down list to filter the ETL processes for a certain status. The following options are available:
    - **All**   
        All ETL processes are displayed. By default, this mode is selected.
    - **Todo**   
        All pending ETL processes are displayed.
    - **Error**  
        All faulty ETL processes are displayed.
    - **Done**   
        All completed ETL processes are displayed.
    - **Destination frozen**   
        All ETL processes whose destination attribute is blocked because the corresponding entity is opened by a user are displayed.
    - **Awaiting confirmation**   
        All ETL processes that must be confirmed are displayed.
    - **Synchronous**   
        All ETL processes that are executed synchronously are displayed for the duration of processing.
    - **Awaiting confirmation different user**   
        All ETL processes that must be confirmed by a user other than the creator are displayed.
    - **Semiautomatic accepted**   
        All ETL processes that have been confirmed are displayed.

The following functions are available for the editing toolbar:

- [x]     
    Select the checkbox to display the editing toolbar. Alternatively, you can click directly a row in the list to select the corresponding checkbox and display the editing toolbar. You cannot select multiple checkboxes at once.

- [RETRY]   
    Click this button to restart the selected ETL process. This button is only displayed if a single checkbox of an ETL process with the **Error** status is selected. The *Process will be retried shortly* pop-up window is displayed in the upper right corner.

    ![ETL processes](../../Assets/Screenshots/DataHub/Settings/ETLProcesses/ProcessRetried.png "[ETL processes]")

The following functions and fields are available in this view:

- *Status*   
    Status of the ETL process. The following statuses are available:
    - **Todo**
    - **Error**
    - **Done**
    - **Destination frozen**
    - **Awaiting confirmation**
    - **Synchronous**
    - **Awaiting confirmation diff. user**
    - **Semiautomatic accepted**  

- *From-to*   
    Name of the source and the destination entity. The SKUs of the entities are indicated in brackets after the names.  

- *Source attribute*   
    Source attribute name.

- *Destination attribute*   
    Destination attribute name.

- *Error*   
    Error message. This field is only displayed for ETL processes where an error has occurred.

- *ID*   
    Process identification number. The ID number is automatically assigned by the system when the product is created.

- *Destination language*   
    Destination language to which the process is mapped.

- *Destination scope*   
    Destination scope to which the process is mapped.

- *Accepted on*   
    Date and time of the confirmation. This field is only displayed for ETL processes with the **Semiautomatic accepted** status.

- *Accepted by*   
    Name and username of the user who confirmed the process. This field is only displayed for ETL processes with the **Semiautomatic accepted** status.

- *Created by*   
    ID of the user who created the process.



