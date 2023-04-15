# Connections (Logging)

*Fulfillment > Logging > Tab CONNECTIONS*

![List of intents](../../Assets/Screenshots/Fulfillment/Logging/ListIntents.png "[List of intents]")


**List of intents**

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
    Click this button to display the search bar and search for an intent.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of intents.

- *VIEW*  
    Click the drop-down list to select the view. All created views are displayed in the drop-down list. Click the ![Points](../../Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *VIEW* drop-down list to display the context menu and create a view.   

    - ![Points](../../Assets/Icons/Points01.png "[Points]") (Points)      
        Click this button to the right of the *View* drop-down list to display the context menu. The following menu entries are available:

        - ![Create](../../Assets/Icons/Plus06.png "[Create]") create  
            Click this entry to create a view. The *Create view* window is displayed, see [Create view](#create-view).

        - ![Rename](../../Assets/Icons/Edit02.png "[Rename]") rename  
            Click this entry to rename the selected view. The *Rename view* window is displayed, see [Rename view](#rename-view). This menu entry is only displayed if a view has been selected.

        - ![Reset](../../Assets/Icons/Reset.png "[Reset]") reset  
            Click this entry to reset all unsaved changes to the settings of the selected view. This menu entry is only displayed if a view has been selected and any changes have been made to the view settings.

        - ![Publish](../../Assets/Icons/Publish.png "[Publish]") publish  
            Click this entry to publish the view. This menu entry is only displayed if a view has been selected and unpublished.

        - ![Unpublish](../../Assets/Icons/Unpublish.png "[Unpublish]") unpublish  
            Click this entry to unpublish the view. This menu entry is only displayed if a view has been selected and published.

        - ![Save](../../Assets/Icons/Save.png "[Save]") save  
            Click this entry to save the current view settings in the selected view. This menu entry is only displayed if a view has been selected.

            > [Info] When the settings of a view have been changed, an asterisk is displayed next to the view name. The asterisk is hidden as soon as the changes have been saved.

        - ![Delete](../../Assets/Icons/Trash01.png "[Delete]") delete  
            Click this entry to delete the selected view. A confirmation window to confirm the deletion is displayed. This menu entry is only displayed if a view has been selected.


- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
    Select the checkbox to display the editing toolbar. You can only select one checkbox at a time.

- [![Show message](../../Assets/Icons/ShowMessage.png "[Show message]") SHOW MESSAGE]  
    Click this button to display the message(s) contained in the selected intent. This button is only displayed if a single checkbox in the list of intents is selected. Alternatively, you can click directly a row in the list to display an intent. The *List of messages* view is displayed, see [List of messages](#list-of-messages).


The list displays all intents. Depending on the settings, the displayed columns may vary. All fields are read-only.

- *Name*  
    Description of the intent.

- *Number of messages*  
    Number of messages contained in the intent.

- *Created at*  
    Date and time of the creation.

- *Created by*  
    Name and username of the user that initiated the action leading to the intent. If the intent was created automatically by the system, this field is empty. 

- *Max log level of message*  
    Maximum log level type of the message(s) contained in the intent. The following levels are available:
  - **Debug**
  - **Info**
  - **Notice**
  - **Warning**
  - **Error**
  - **Critical**
  - **Alert**
  - **Emergency**

- *ID*  
    Intent identification number. The ID number is automatically assigned by the system.

- *Short preview*  
    First 30 characters of the log message.

- *Preview*  
    Complete log message.


## List of messages

*Fulfillment > Logging > Tab CONNECTIONS > Select an intent*

![List of messages](../../Assets/Screenshots/Fulfillment/Logging/ListMessages.png "[List of messages]")

**List of messages**

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *List of messages* view and return to the list of intents. All changes are rejected.

- ![Unpublish](../../Assets/Icons/Unpublish02.png "[Unpublish]") (Download)  
    Click this button to download the displayed log message.

[comment]: <> (Bug gemeldet. Wird rausgenommen.)

- ![View](../../Assets/Icons/Eye02.png "[View]")  (View)   
    Click this button to display the details of the log message. Alternatively, you can click directly a row in the list to display the details of the log message. The *Detail of log message "Log message title"* view is displayed, see [Detail of log message "Log message title"](#detail-of-log-message-log-message-title). 


The list displays all log messages of the selected intent. Depending on the settings, the displayed columns may vary. All fields are read-only.

- *Title*  
    Title of the log message.

- *Log level*  
    Log level type. The following options are available:
    - **Debug**
    - **Info**
    - **Notice**
    - **Warning**
    - **Error**
    - **Critical**
    - **Alert**
    - **Emergency**

- *Created at*  
    Date and time of the creation.

- *Created by*  
    Name and username of the user that initiated the action leading to the log message. If the log message was created automatically by the system, this field is empty. 

- *Message*  
    Detailed log message to the intent.

- *ID*  
    Log message identification number. The ID number is automatically assigned by the system.


### Detail of log message "Log message title"

*Fulfillment > Logging > Tab CONNECTIONS > Select an intent > Select a log message*

![List of messages](../../Assets/Screenshots/Fulfillment/Logging/DetailLogMessageAttributes.png "[List of messages]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *Detail of log message "Log message title"* view and return to the list of messages. All changes are rejected.

- [CANCEL]  
    Click this button to close the *Detail of log message "Log message title"* view.

- *Message*    
    Description of the log message.


### Detail of log message "Log message title" &ndash; Attributes

*Fulfillment > Logging > Tab CONNECTIONS > Select an intent > Select a log message > Tab Attributes*

![Detail Log Message Attributes](../../Assets/Screenshots/Fulfillment/Logging/DetailLogMessageAttributes.png "[Detail Log Message Attributes]")

The *Attributes* tab displays further details of the selected log message. Depending on the attribute set of the log message, the displayed fields vary. All fields are read-only.

In general, the most common attribute sets are the standard error log message attribute set and the API communication attribute set. The fields of these sets are described in the following. Furthermore, it is possible to create a custom log message attribute set with different fields.

**Standard error log message attribute set**

- *Error code*  
    Error code number.

- *File*  
    Path of the file where the error has occurred.

- *Line*  
    Line in the file where the error has occurred.

- *Exception class*   
    Class name of the error. The error class describes the type of error that has occurred.

- *Trace as string*   
    Stack trace until the error has occurred. The stack trace lists the code until the error has occurred and is used to track the error.

- *Exception*   
    Detailed description of the error.

**API communication attribute set**

- *Code*   
    Http response status code. For detailed information about the http status codes, see [http status codes](https://www.rfc-editor.org/rfc/rfc9110#section-15).

- *Endpoint and method*   
    Http method of the API request and url endpoint to which the request was sent.

- *Request*   
    Http header and body of the request.

- *Response*   
    Http header and body of the response.

- *Exception*   
    Description of the error. An exception is only displayed if an error has occurred and a http status code of the **4xx** class, for instance a **404** code has been returned.


### Detail of log message "Log message title" &ndash; Dependencies

*Fulfillment > Logging > Tab CONNECTIONS > Select an intent > Select a log message > Tab Dependencies*

![List of messages](../../Assets/Screenshots/Fulfillment/Logging/DetailLogMessageDependencies02.png "[List of messages]")

**Dependencies**

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of the log message dependencies.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
    Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all dependent entities in the list are selected. 

The list displays all dependencies of the selected log message. Depending on the settings, the displayed columns may vary. All fields are read-only.   
If no dependent entities exist, the *No other entities depend on this entity* notice is displayed.

- *Dependent entity ID*   
    Identification number of the dependent entity. The ID number is automatically assigned by the system. 

- *Dependent entity type*   
    Type of the dependent entity. 

- *Change tracking mode*   
    Change tracking mode (ETL mode) of the dependent entity. The following options are available:
    - **Manual**
    - **Semi-automatic**
    - **Semi-automatic, changes must be confirmed by another user**   
    - **Automatic**

- *Dependent entity friendly identifier*   
    Further, more descriptive identifier of the dependent entity, for instance a reference number or an SKU.

- [RERUN MAPPING]   
    Click this button to rerun the mapping of the selected entity. This button is only displayed if the checkbox of at least one dependency is selected.	

   


## Create view

*Fulfillment > Logging > Tab CONNECTIONS > Button Points > Menu entry create*

![Create view](../../Assets/Screenshots/Fulfillment/DispatchNotes/CreateView.png "[Create view]")

For a detailed description of this window and the corresponding functions, see [Create view](./01a_List.md#create-view).

## Rename view

*Fulfillment > Logging > Tab CONNECTIONS > Button Points > Menu entry rename*

![Rename view](../../Assets/Screenshots/Fulfillment/DispatchNotes/RenameView.png "[Rename view]")

For a detailed description of this window and the corresponding functions, see [Rename view](./01a_List.md#rename-view).
