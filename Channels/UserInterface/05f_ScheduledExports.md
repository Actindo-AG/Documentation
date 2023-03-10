[!!Manage the orders and returns](../Operation/04_ManageOrdersReturns.md)
[!!User interface Log](./06a_Log.md)

# Scheduled exports

*Omni-Channel > Orders and returns > Tab SCHEDULED EXPORTS*

![Scheduled exports](../../Assets/Screenshots/Channels/OrdersReturns/ScheduledExports/ScheduledExports.png "[Scheduled exports]")

**Scheduled exports**

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of scheduled exports.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all orders in the list are selected.

- [SHOW LOG]  
    Click this button to display the details of the log message. This button is only displayed if a single checkbox of a faulty export in the list of scheduled exports is selected. The *Detail of log message "Log message title"* view is displayed, see [Detail of log message "Log message title"](#detail-of-log-message-log-message-title).

- [RETRY EXPORT]  
    Click this button to retry the selected scheduled export(s). This button is only displayed if the checkbox of at least one faulty scheduled export is selected.

[comment]: <> (prüfen, ob irgendein pop-up window angezeigt wird. -> aktuell keine Testdaten oder Fehlermeldung)

The list displays all scheduled exports. Depending on the settings, the displayed columns may vary. All fields are read-only. 

- *ID*  
    Export identification number. The ID number is automatically assigned by the system.

- *Error message*  
    Error log message if an error has occurred. If no error has occurred, this field is empty.

- *Status*   
    Status of the scheduled export. The following options are available:
    - **Pending**  
        The export is pending.
    - **Finally failed**  
        The export has failed.

- *Connection*  
    Name of the connection via which the export will be performed.

- *Order/Return ID*  
    Order or return identification number. The ID number is automatically assigned by the system.
    
- *Order/Return*  
    Indication where the error has occurred. The following options are available:
    - **Order**   
        The error has occurred in an order.
    - **Return**
        The error has occurred in a return.


## Detail of log message "Log message title"

*Omni-Channel > Orders and returns > Tab SCHEDULED EXPORTS > Select checkbox of a faulty export > Button SHOW LOG*

![Detail of log message](../../Assets/Screenshots/Channels/OrdersReturns/ScheduledExports/DetailLogMessageAttributes.png "[Detail of log message]")

For a detailed description of this view and the corresponding functions, see [LOG](./06a_Log.md#detail-of-log-message-log-message-title).

