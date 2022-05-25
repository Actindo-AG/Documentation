[!!Workflows](ActindoWorkFlow)

# Processes

*Workflows > Processes > Tab OVERVIEW*

![Overview](/Assets/Screenshots/ActindoWorkFlow/Processes/Processes.png "[Overview]")


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


- *Status*  
Click the drop-down list to select a process status. The following options are available:  

    - **All**  
    Select this option to display all processes, regardless of their status.

    - **Ready**  
    Select this option to display the processes that have just been initiated.

    - **In Progress**  
    Select this option to display the processes that are currently active (first action is already executed).

    - **Error**  
    Select this option to display the processes that have given an error (a process action has given an error).

    - **Done**  
    Select this option to display the processes that have been completely executed (end place has been reached).  

    - **Dead**  
    Select this option to display the processes that have automatically stopped due to a missing input. A dead process cannot be retried. It can only be aborted, that is, manually ended, and reinitiated.

    - **Suspended**  
    Select this option to display the processes that have been manually paused. The remaining process actions are temporarily stopped.

    - **Aborted**  
    Select this option to display the processes that have been manually ended. All process actions currently running are stopped and no longer executed.


- *Workflow*  
Click the drop-down list to display a specific workflow type. The workflows created in the *Workflows* menu entry are listed here. For detailed information about creating a workflow, see [Create a workflow](ActindoWorkFlow/Operation/01_ManageWorkflows.md#create-a-workflow).



- ![Search](/Assets/Icons/Search.png "[Search]") (Search)  
    Click this button to display the search bar and search for a workflow.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)  
    Click this button to update the list of workflows.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)  
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The x indicates the number of columns that are currently displayed in the list.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)  
    Click this button to display the filter bar and customize the active filters. The x indicates the number of filters that are currently active.


The list displays all processes. Depending on the settings, the displayed columns may vary. All fields are read-only.

  - [x]  
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all processes in the list are selected.

  Depending of the process status, the editing toolbar may display different buttons.

    - ![Abort](/Assets/Icons/Stop.png "[Abort]") (Abort)  
    Click this button to end the process. This button is displayed when the process status is *Error* or *In Progress*. When clicking this button, the process status changes to *Aborted*.
    - ![Suspend](/Assets/Icons/Pause.png "[Suspend]") (Suspend)  
    Click this button to suspend the process temporarily. This button is displayed when the process status is *In Progress*.  When clicking this button, the process status changes to *Suspended*.
    - ![Start](/Assets/Icons/Play.png "[Start]") (Start)  
    Click this button to resume the process. This button is displayed when the process status is *Suspended*. When clicking this button, process status changes again to *In Progress*.


  - *Status*  
  Status of the process. The different process statuses are displayed in different colours. The following statuses are possible:

    - *Ready*
    - *In Progress*
    - *Error*
    - *Done*
    - *Dead*
    - *Suspended*
    - *Aborted*

[comment]: <> (Repeat or leave it out? Add colour code?)

  - *Suspended Actions*  
  If the process contains suspended actions, a ![Warning](/Assets/Icons/Warning.png "[Warning]") sign is displayed. Click the process to display the individual actions, see [Actions](#actions).

  - *Subject*  
  Process description.

  - *Workflow*  
  Name of the workflow.

  - *Queue Type*  
  Queue type configured in the workflow. For detailed information about configuring the queue types, see [Configure the queue types](ActindoWorkFlow/Integration/01_ConfigureQueueTypes.md).

  - *Priority*

  [comment]: <> (Oli fragen)

  - *Created*  
  Date and time of creation.

  - *Last activity*  
  Last date and time an activity was registered in the process.

  - *ID*  
  Process ID.

  - *Owning Module*  
  Module where the process is integrated.

  - *Created by*  
  Name and user ID of the person who initiated the process.

  - *Modified by*  
  Name and user ID of the person who modified the process.



## Process ID

*Workflows > Processes > Tab OVERVIEW > Select a process*

![Process ID](/Assets/Screenshots/ActindoWorkFlow/Processes/Actions.png "[Process ID]")

- ![Back](/Assets/Icons/Back02.png "[Back]") (Back)  
Click this button to close the *Process ID* view and return to the *Processes* view.

- *Process ID*  
Process ID number.

- *Workflow*  
Name of the workflow.

- ![Settings](/Assets/Icons/Settings01.png "[Settings]") (Settings)  
Click this button to display the editing options.

- [SAVE]  
Click this button to save any changes made.

- [RESET]  
Click this button to reset layout.

[comment]: <> (Ist es möglich, hier was zu ändern? Check Wissentranfer!)

- ![Cancel](/Assets/Icons/Cross02.png "[Cancel]") (Cancel)  
Click this button to cancel editing and discard changes.


[comment]: <> (The *Process ID* view displays a diagram of the selected process including all places and actions. Further details about the process actions included in the diagram as well as about the logs and tokens are displayed in separate tabs in the bottom part of the *Process ID* view. For detailed information, see...?)

[comment]: <> (For detailed information about checking the process action status, see ...)


### Actions

*Workflows > Processes > Tab OVERVIEW > Select a process*

![Actions](/Assets/Screenshots/ActindoWorkFlow/Processes/Actions.png "[Actions]")

> [Info] The *Actions* tab is selected by default when selecting a process.

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


- *Status*  
Click the drop-down list to select a process status. The following options are available:  

    - **All**  
    Select this option to display all actions, regardless of their status.

    - **Active**  
    Select this option to display the actions that are currently active.

    - **Done**  
    Select this option to display the actions that have been already executed.  

    - **Error**  
    Select this option to display the actions that have given an error.

    - **Error; automatic retry**  
    Select this option to display the actions that have given an error but are set for automatic retry.

    > [Info] This setting depends on the action and is usually preconfigured.

    - **Suspended**  
    Select this option to display the actions that have been manually paused.

    - **Process aborted**  
    Select this option to display the actions included in a process that has been manually ended.



- ![Search](/Assets/Icons/Search.png "[Search]") (Search)  
    Click this button to display the search bar and search for a workflow.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)  
    Click this button to update the list of workflows.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)  
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The x indicates the number of columns that are currently displayed in the list.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)  
    Click this button to display the filter bar and customize the active filters. The x indicates the number of filters that are currently active.


The list displays all actions. Depending on the settings, the displayed columns may vary. All fields are read-only.

  - [x]    
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all actions in the list are selected.

  Depending of the process status, the editing toolbar may display different options.

    - ![Retry](/Assets/Icons/Retry01.png "[Retry]") (Retry)  
    Click this button to retry the action. This button is displayed when the action status is *Error*.
    - ![Suspend](/Assets/Icons/Pause.png "[Suspend]") (Suspend)  
    Click this button to suspend the action temporarily. This button is displayed when the action status is *In Progress*. When clicking this button, the action status changes to *Suspended*.
    - ![Start](/Assets/Icons/Play.png "[Start]") (Start)  
    Click this button to resume the action. This button is displayed when the action status is *In Progress*. When clicking this button, the action status changes again to *In Progress*. The warning sign in the *Suspended Actions* column of the *Processes* view is no longer displayed.
    - [REMOVE DEFER TIME]  
    Click this button to eliminate the defer time preconfigured in the action, if any. The action is then executed immediately. This button is displayed when the action status is *In Progress*.


  - *Status*  
  Status of the action. The different process statuses are displayed in different colours. The following statuses are possible:

    - *Active*  
    - *Done*  
    - *Error*  
    - *Error; automatic retry*  
    - *Suspended*  
    - *Process aborted*  

[comment]: <> (Repeat here or leave it out? Add colour code?)

  - *Transition*  
  Transition executed in the course of the selected action.

  - *Tries*  
  Number of times an action has been tried.

  - *Max retries after error*  
  Number of times an action must be retried after error.

  > [Info] This setting depends on the action and is usually preconfigured.

[comment]: <> (Question pending for OLI)

  - *Queue Type*  
  The *Default* queue type is normally selected. For detailed information about configuring queue types, see [Configure the queue types](01_ConfigureQueueTypes.md).

  > [Info] A different queue type can be selected by editing an action, see [Edit an action](01_ManageWorkflows.md#edit-an-action).

  - *Defer until*  
  Next point in time when the action is being tried.  

  > [Info] This setting depends on the action and is not available in all actions.

  - *Created*  
  Date of creation.

  - *Modified*  
  Date of modification.

  - *ID*  
  Action ID number.

  [comment]: <> (Oli fragen)

  - *Transition ID*  
  Transition ID number.


### Logs

*Workflows > Processes > Tab OVERVIEW > Select a process > Tab Logs*

![Logs](/Assets/Screenshots/ActindoWorkFlow/Processes/Logs.png "[Logs]")

[comment]: <> (The *Logs* tab displays a list of all log messages produced in the course of a process. Logs refer to the execution of process actions. Click on a log message for further details. The *Log ID* view is displayed.)


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
    Select this option to display all logs, regardless of their status.

    - **Debug**

    - **Info**  
    Select this option to display all logs simply providing information.

    - **Notice**

    - **Warning**

    - **Error**  
    Select this option to display all logs specifying an error.

    - **Critical**

    - **Alert**

    - **Emergency**

[comment]: <> (Log status durchgehen?)


- ![Search](/Assets/Icons/Search.png "[Search]") (Search)  
Click this button to display the search bar and search for a workflow.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)  
Click this button to update the list of workflows.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)  
Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The x indicates the number of columns that are currently displayed in the list.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)  
Click this button to display the filter bar and customize the active filters. The x indicates the number of filters that are currently active.


The list displays all logs. Depending on the settings, the displayed columns may vary. All fields are read-only.

  - [x]    
  Select the checkbox to display the editing toolbar.

  - *Type*  
  Log level type. The different log level types are displayed in different colours. The following types are possible:

    - *Debug*
    - *Info*
    - *Notice*
    - *Warning*
    - *Error*
    - *Critical*
    - *Alert*
    - *Emergency*

[comment]: <> (Repeat here or leave it out? Add colour code?)

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



### Tokens

*Workflows > Processes > Tab OVERVIEW > Select a process > Tab Tokens*

![Tokens](/Assets/Screenshots/ActindoWorkFlow/Processes/Tokens.png "[Tokens]")


- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Hide processed*  
Disable this toggle to display all tokens, including the ones that have already been processed.

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


- ![Search](/Assets/Icons/Search.png "[Search]") (Search)  
    Click this button to display the search bar and search for a workflow.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)  
    Click this button to update the list of workflows.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)  
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The x indicates the number of columns that are currently displayed in the list.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)  
    Click this button to display the filter bar and customize the active filters. The x indicates the number of filters that are currently active.


The list displays all tokens if the ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Hide processed* toggle is disabled. Depending on the settings, the displayed columns may vary. All fields are read-only.

  - *Status*  
  Token status. The different statuses are displayed in different colours. The following statuses are possible:

    - *Ready*
    - *Processed*
    - *Being processed*
    - *Error*

[comment]: <> (Tokens kann auch als "Ready", "Being processed", "Error" im Status vorkommen. So gemeint oder nur Processed/Unprocessed? Add colour code?)

  - *Place*  
  Place where the token has been input.

  - *Data*  
  Type of data contained in the token.

  - *Next possible action(s)*    
  Next compatible action(s) where the token can be input.

  - *ID*  
  Token ID number.  

  [comment]: <> (Oli fragen)

  - *Place ID*  
  Place ID number.

  - *Process Action ID*  
  Process action ID number.

  [comment]: <> (Oli fragen. Null wenn am end place?)



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

  - *Debug*
  - *Info*
  - *Notice*
  - *Warning*
  - *Error*
  - *Critical*
  - *Alert*
  - *Emergency*


- *Created - by*  
Date and time of creation, name and user ID of the person who created the process.

[comment]: <> (Ich gehe davon aus, dass Log ist automatisch vom System erstellt, daher "process creator", oder ist es "workflow creator"?)

- *Workflow*  
Workflow ID number and name.

- *Process*  
Process ID number and description.

- *Transition*  
Transition ID number and description.
