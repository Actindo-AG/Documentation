[!!Workflows](ActindoWorkFlow)

# Logs

*Workflows > Logs*

![Logs](/Assets/Screenshots/ActindoWorkFlow/Logs/Logs.png "[Logs]")


- *VIEW*  
Click the drop-down list to select the view. All created views are displayed in the drop-down list. Click the ![Points](/Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *VIEW* drop-down list to display the context menu and create a view. For detailed information, see [Create view](#create-view).

  - View context menu  
  Click the ![Points](/Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *View* drop-down list to display the context menu. The following menu entries are available:

    - ![Create](/Assets/Icons/Plus06.png "[create]") create  
    Click this entry to create a view. The *Create view* window is displayed.

    - ![Rename](/Assets/Icons/Edit02.png "[Rename]") rename  
    Click this entry to rename the selected view. The *Rename view* window is displayed. This menu entry is only displayed when a view is selected.

    - ![Reset](/Assets/Icons/Reset.png "[Reset]") reset  
    Click this entry to reset the view to the selected views settings. This menu entry is only displayed when a view is selected and any changes are made to the views settings.

    - ![Publish](/Assets/Icons/Publish.png "[Publish]") publish  
    Click this entry to publish the view. This menu entry is only displayed when a view is selected and unpublished.

    - ![Unpublish](/Assets/Icons/Unpublish.png "[Unpublish]") unpublish  
    Click this entry to unpublish the view. This menu entry is only displayed when a view is selected and published.

    - ![Save](/Assets/Icons/Save.png "[Save]") save  
    Click this entry to save the current view settings in the selected view. This menu entry is only displayed when a view is selected.

     > [Info] When the settings of a view have been changed, an asterisk is displayed behind the view name. The asterisk is hidden as soon as the changes have been saved.

    - ![Delete](/Assets/Icons/Trash01.png "[Delete]") delete  
    Click this entry to delete the selected view. A confirmation window to confirm the deletion is displayed. This menu entry is only displayed when a view is selected.


- *Log Level*     
  Click the drop-down list to select a log level. The following options are available:  

    - **All**  
      Select this option to display all logs regardless of their type.
    - **Debug**
      Select this option to display all logs of the **Debug** type.
    - **Info**  
      Select this option to display all logs of the **Info** type.
    - **Notice**
      Select this option to display all logs of the **Notice** type.
    - **Warning**
      Select this option to display all logs of the **Warning** type.
    - **Error**  
      Select this option to display all logs of the **Error** type.
    - **Critical**
      Select this option to display all logs of the **Critical** type.
    - **Alert**
      Select this option to display all logs of the **Alert** type.
    - **Emergency**
      Select this option to display all logs of the **Emergency** type.

[comment]: <> (Log status durchgehen?)

- ![Search](/Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for a workflow.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)    
  Click this button to update the list of workflows.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)    
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The x indicates the number of columns that are currently displayed in the list.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)    
  Click this button to display the filter bar and customize the active filters. The x indicates the number of filters that are currently active.


The list displays all logs. Depending on the settings, the displayed columns may vary. All fields are read-only. When clicking a log, the *Log ID* view is displayed, see [Log ID](#Log-ID).

- [x]    
  Select the checkbox to display the editing toolbar.

- *Type*  
  Log level type. The different log level types are displayed in different colors. The following types are possible:
  - **Debug**
  - **Info**
  - **Notice**
  - **Warning**
  - **Error**
  - **Critical**
  - **Alert**
  - **Emergency**

[comment]: <> (Repeat here or leave it out? Add color code?)

- *Log Message*   
  Description of the issue.

- *Workflow*   
  Workflow which the log message refers to.

- *Workflow ID*       
  Workflow ID number.

- *Search String*    
  [comment]: <> (Oli fragen)

- *Created*   
  Date of creation.

- *ID*   
  Log ID number.

- *Process*   
  Process specification.

- *Process ID*   
  Process ID number.

- *Transition*   
  Transition specification.

- *Transition ID*   
  Transition ID number.

- *Created by*   
  Name and user ID of person who created the process.



## Create view

*Workflows > Processes > Tab OVERVIEW > Button Points > Menu entry create*

![Create view](/Assets/Screenshots/ActindoWorkFlow/Workflows/CreateView.png "[Create view]")


- *Name*    
  Enter a name for the view.

- [CANCEL]   
  Click this button to cancel creating a view. The *Create view* window is closed.

- [SAVE]   
  Click this button to save the new view. The *Create view* window is closed. The view is saved and displayed in the *View* drop-down list.



## Rename view

*Workflows > Processes > Tab OVERVIEW > Button Points > Menu entry rename*

![Rename view](/Assets/Screenshots/ActindoWorkFlow/Workflows/RenameView.png "[Rename view]")


- *Name*   
  Click the field to edit the view name.

- [CANCEL]   
  Click this button to cancel renaming a view. The *Rename view* window is closed.

- [SAVE]   
  Click this button to save the changes to the view name. The *Rename view* window is closed. The new name for the view is saved and displayed in the *View* drop-down list.



## Log ID

*Workflows > Processes > Tab OVERVIEW > Select a process > Tab Logs > Select Log Message*

![Log ID](/Assets/Screenshots/ActindoWorkFlow/Processes/LogID.png "[Log ID]")

- ![Back](/Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *Log ID* view and return to the *Logs* tab.

- *Log ID (x)*   
  Log ID number.

- *Log Message*    
  A description of the issue is displayed in the text box. This box is read-only.  

  > [Info] In case of an error, detailed information is provided (stack trace) for reporting and debugging purposes.

[comment]: <> (Diesen Text kann man rauskopieren, um ein Ticket zu erstellen o.ä. Erwähnen? Nützlich für Kunden?)

- *Log Level*    
Description of log level. The following levels are available:
  - **Debug**
  - **Info**
  - **Notice**
  - **Warning**
  - **Error**
  - **Critical**
  - **Alert**
  - **Emergency**


- *Created - by*    
  Date and time of creation, name and user ID of the person who created the process.

[comment]: <> (Ich gehe davon aus, dass Log ist automatisch vom System erstellt, daher "process creator", oder ist es "workflow creator"?)

- *Workflow*    
  Workflow ID number and name.

- *Process*    
  Process ID number and description.

- *Transition*     
  Transition ID number and description.