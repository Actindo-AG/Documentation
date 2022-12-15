[!!Tag](../Integration/0X_tobecompleted.md)
[!!Tag](../Integration/0X_tobecompleted.md)


# Log

*Omni-Channel > Logging > Tab LOG*

[comment]: <> (Datei Fulfillment/UserInterface/02a_Connections.md als Referenz. Ggf. Änderungen konsistent in beiden Dateien übernehmen. Event log hier zu intent genädert)

[comment]: <> (Keine Logs im Sandbox. Info und Screenshots aus NoE test account -> Vorsicht: in Detail log message Kundenname -> anonymisieren!)

![List of intents](../../Assets/Screenshots/Channels/Logging/ListIntents02.png "[List of intents]")


**List of intents**

- *VIEW*  
  Click the drop-down list to select the view. All created views are displayed in the drop-down list. Click the ![Points](../../Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *VIEW* drop-down list to display the context menu and create a view. For detailed information, see [Create view](#create-view).

  - ![Points](../../Assets/Icons/Points01.png "[Points]") (Points)      
    Click this button to the right of the *View* drop-down list to display the context menu. The following menu entries are available:

    - ![Create](../../Assets/Icons/Plus06.png "[Create]") create  
      Click this entry to create a view. The *Create view* window is displayed.

    - ![Rename](../../Assets/Icons/Edit02.png "[Rename]") rename  
      Click this entry to rename the selected view. The *Rename view* window is displayed. This menu entry is only displayed if a view has been selected.

    - ![Reset](../../Assets/Icons/Reset.png "[Reset]") reset  
      Click this entry to reset all unsaved changes to the settings of the selected view. This menu entry is only displayed if a view has been selected and any changes have been made to the view settings.

    - ![Publish](../../Assets/Icons/Publish.png "[Publish]") publish  
      Click this entry to publish the view. This menu entry is only displayed if a view has been selected and unpublished.

    - ![Unpublish](../../Assets/Icons/Unpublish.png "[Unpublish]") private view  
      Click this entry to unpublish the view. This menu entry is only displayed if a view has been selected and published.

    - ![Save](../../Assets/Icons/Save.png "[Save]") save  
      Click this entry to save the current view settings in the selected view. This menu entry is only displayed if a view has been selected.

      > [Info] When the settings of a view have been changed, an asterisk is displayed next to the view name. The asterisk is hidden as soon as the changes have been saved.

    - ![Delete](../../Assets/Icons/Trash01.png "[Delete]") delete  
      Click this entry to delete the selected view. A confirmation window to confirm the deletion is displayed. This menu entry is only displayed if a view has been selected.


- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for en intent.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of intents.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to display the editing toolbar. Only one intent can be selected at a time.

- [SHOW MESSAGE]  
  Click this button to display the selected intent. This button is only displayed if the checkbox of an intent is selected. Alternatively, you can click directly a row in the list to view an intent. The *List of messages* view is displayed.


The list displays all intents. Depending on the settings, the displayed columns may vary. All fields are read-only.

- *Name*  
  Description of log.

[comment]: <> (oder Description of intent? Unsicher über Terminologie)

- *Number of messages*  
  Number of messages contained in the log.

- *Created on*  
  Date and time of the creation.

- *Created by*  
  Name and username of the user who created the log.  

[comment]: <> (generated statt created? Muss nicht eine Person/ein Benutzer sein, es wird nicht manuell gemacht, sonder automatisch)

- *Max log level of message*  
  Maximal log level type of the message(s) contained in the intent. The following levels are available:
  - **Debug**
  - **Info**
  - **Notice**
  - **Warning**
  - **Error**
  - **Critical**
  - **Alert**
  - **Emergency**

[comment]: <> (Icons hinzufügen?)  

- *ID*  
  Log identification number. The ID number is automatically assigned by the system.

- *Preview*  
  Preview of log details.

- *Short preview*  
  Short preview of log details.


## List of messages

*Omni-Channel > Logging > Tab LOG > Select an intent*

![List of messages](../../Assets/Screenshots/Channels/Logging/ListMessages.png "[List of messages]")

**List of messages**

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *List of messages* view and return to the list of intents.

- ![Unpublish](../../Assets/Icons/Unpublish02.png "[Unpublish]") (Unpublish)  

  Click this to unpublish the log message.

[comment]: <> (Unpublish oder private view? Bedeutung?)

- ![View](../../Assets/Icons/Eye02.png "[View]") (Eye)    
  Click this button to view the log message details.


The list displays all messages contained in the selected intent. Depending on the settings, the displayed columns may vary. All fields are read-only.

- *Title*  
  Description of the log message.

- *Log level*  
  Log level type. The following levels are available:
  - **Debug**
  - **Info**
  - **Notice**
  - **Warning**
  - **Error**
  - **Critical**
  - **Alert**
  - **Emergency**

[comment]: <> (Icons hinzufügen?)

- *Created on*  
  Date and time of the creation.

- *Created by*  
  Name and username of the user who created the intent.

[comment]: <> (Or who created/generated the log message?)

- *Message*  
  Details of the log message.

- *ID*  
  Log message identification number. The ID number is automatically assigned by the system.


### Detail of log message "Log message name"

*Omni-Channel > Logging > Tab LOG > Select an intent > Select a log message*

![List of messages](../../Assets/Screenshots/Channels/Logging/DetailLogMessageAttributes.png "[List of messages]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *Detail of log message "Log message name"* view and return to the list of messages.

- [CANCEL]  
  Click this button to close the *Detail of log message "Log message name"* view and return to the list of messages.

[comment]: <> (Beide tun praktisch das gleiche)

- Message  
  Short description of the log message.

- *Message:*  
  Short description of the log message.

[comment]: <> (Hier Info wiederholt sich. Report als Bug?)


### Detail of log message "Log message name" &ndash; Attributes

*Omni-Channel > Logging > Tab LOG > Select an intent > Select a log message > Tab Attributes*

![Detail Log Message Attributes](../../Assets/Screenshots/Channels/Logging/DetailLogMessageAttributes.png "[Detail Log Message Attributes]")

The *Attributes* tab displays further details of the selected log message. Depending on the message title, the assigned attributes, and therefore the fields displayed, may vary. All fields are read-only.

By default, the following fields are displayed:

[comment]: <> (Felder ändern sich abhängig von Title - vgl. NotFoundException und updateDeliveryStatus? Vermutlich abhängig von Attributes, also Standardsatz dazu und keine Felder? Oder gibt es Standardfelder?)


- *Error code*  
  Error code number.

- *File*  
  File where the error has occurred.

- *Line*  
  Line where the error has occurred.

- *Exception class*  

- *Trace as string*  

- *Exception*

[comment]: <> (Further info needed)

### Detail of log message "Log message name" &ndash; Dependencies

*Omni-Channel > Logging > Tab LOG > Select an intent > Select a log message > Tab Dependencies*

![List of messages](../../Assets/Screenshots/Channels/Logging/DetailLogMessageDependencies.png "[List of messages]")

This tab has no function in the *Omni-Channel* module, since log messages have no dependent entities. The notice *No other entities depend on this entity* is displayed.

[comment]: <> (Könnte es Dependencies geben?)


## Create view

*Omni-Channel > Logging > Tab LOG > Button Points > Menu entry create*

![Create view](../../Assets/Screenshots/Channels/CreateView.png "[Create view]")

For a detailed description of this window and the corresponding functions, see [Create view](./02a_Offers.md#create-view).

## Rename view

*Omni-Channel > Logging > Tab log > Button Points > Menu entry rename*

![Rename view](../../Assets/Screenshots/Channels/RenameView.png "[Rename view]")

For a detailed description of this window and the corresponding functions, see [Rename view](./02a_Offers.md#rename-view).
