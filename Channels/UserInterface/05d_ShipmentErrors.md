[!!Manage the orders and returns](../Operation/04_ManageOrdersReturns.md)
[!!User interface Log](./06a_Log.md)

# Shipment errors

*Omni-Channel > Orders and returns > Tab SHIPMENT ERRORS*

![Shipment errors](../../Assets/Screenshots/Channels/OrdersReturns/ShipmentErrors/ShipmentErrors.png "[Shipment errors]")

**Error list**	

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
    Click this button to display the search bar and search for a shipment error.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of shipment errors.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all shipment errors in the list are selected.

- [SHOW LOG]  
    Click this button to display the details of the shipment error log message. This button is only displayed if a single checkbox in the list of shipment errors is selected. Alternatively, you can click directly a row in the list to display the details of the shipment error log message. The *Detail of log message "Log message title"* view is displayed, see [Detail of log message](#detail-of-log-message).

The list displays all errors to the shipments. Depending on the settings, the displayed columns may vary. All fields are read-only. If no error has occurred, the *There are currently no errors* notice is displayed.

- *Connection*  
    Name of the connection where the shipment error has occurred.

- *Type*  
    Shipment error type. The following options are available:   
    - **Import from channel**  
        The shipment error has occurred while importing the order from the marketplace.   
    - **Export to channel**  
        The shipment error has occurred while exporting the order to the marketplace.  
    - **Export to OMS**  
        The shipment error has occurred while exporting the order to the *Order management* module.

- *ID in shop*  
    Identification number of the order in the marketplace. 

- *Message*  
    Log message to the shipment error.  

- *Shipment*  
    Shipment identification number. The ID number is automatically assigned by the system.

- *Last modified*  
    Date and time of the last modification.

- *Editor*  
    Name and username of the user who modified the error.  

- *ID*  
    Shipment error identification number. The ID number is automatically assigned by the system.

- *Created*  
    Date and time of the creation.

- *Creator*  
    Name and username of the user who created the shipment error.


## Detail of log message

*Omni-Channel > Orders and returns > Tab SHIPMENT ERRORS > Select shipment error*

![Detail of log message](../../Assets/Screenshots/Channels/OrdersReturns/ShipmentErrors/DetailLogMessageAttributes.png "[Detail of log message]")

For a detailed description of this view and the corresponding functions, see [LOG](./06a_Log.md#detail-of-log-message).