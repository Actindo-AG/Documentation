[!!Workflows](ActindoWorkFlow)

# Overview

*Workflows > Processes > Tab OVERVIEW*

![Overview](/Assets/Screenshots/ActindoWorkFlow/Processes/Processes.png "[Overview]")

**Processes**

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
Click the drop-down list to display a specific workflow type. All workflows created in the *Workflows* menu entry are available in the list. For detailed information about creating a workflow, see [Create a workflow](/ActindoWorkFlow/Operation/01_ManageWorkflows.md#create-a-workflow).



- ![Search](/Assets/Icons/Search.png "[Search]") (Search)  
    Click this button to display the search bar and search for a workflow.  

    > [Info] The search function can be used to search for a workflow subject and name. At least 3 characters must be entered.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)  
    Click this button to update the list of workflows.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)  
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The x indicates the number of columns that are currently displayed in the list.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)  
    Click this button to display the filter bar and customize the active filters. The x indicates the number of filters that are currently active.


The list displays all processes that are matching the selected values (status and workflow type). Depending on the settings, the displayed columns may vary. All fields are read-only. Click a process in the list to display the *Process ID* view with a process diagram and detailed information about the selected process.

  - [x]  
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all processes in the list are selected.

  Depending on the process status, the editing toolbar displays the following buttons:

  - ![Abort](/Assets/Icons/Stop.png "[Abort]") (Abort)  
    Click this button to end the process. This button is displayed when the process status is *Error* or *In Progress*. When clicking this button, the process status changes to *Aborted*.
  - ![Suspend](/Assets/Icons/Pause.png "[Suspend]") (Suspend)  
    Click this button to suspend the process temporarily. This button is displayed when the process status is *In Progress*.  When clicking this button, the process status changes to *Suspended*.
  - ![Start](/Assets/Icons/Play.png "[Start]") (Start)  
    Click this button to resume the process. This button is displayed when the process status is *Suspended*. When clicking this button, process status changes again to *In Progress*.


  - *Status*  
    Status of the process. The different process statuses are displayed in different colors. The following statuses are possible:

    - Ready (light gray)
    - In Progress (blue)
    - Error (red)
    - Done (green)
    - Dead (black)
    - Suspended (dark gray)
    - Aborted (black)


  - *Suspended Actions*  
    If the process contains suspended actions, a ![Warning](/Assets/Icons/Warning.png "[Warning]") sign is displayed. Click the process to display the individual actions, see [Actions](#actions).

  - *Subject*  
    Process description.

  - *Workflow*  
    Name of the corresponding workflow.

  - *Queue Type*  
    Queue type configured in the process. This column displays the queue type name or the text "According to configuration in workflow". For detailed information about configuring the queue types, see [Configure the queue types](ActindoWorkFlow/Integration/01_ConfigureQueueTypes.md).

  - *Priority*  
    Process priority set up in the system. The higher the number, the higher the priority.

  - *Created*  
    Date and time of creation.

  - *Last activity*  
    Last date and time an activity was registered in the process.

  - *ID*  
    Process identification number. The ID number is automatically assigned by the system.

  - *Owning Module*  
    Module that has created the workflow.

    > [Info] When a workflow is manually created in the *Workflow* module, the text "ActindoWorkFlow" is displayed. A workflow can also be created automatically by a different module. In this case, the name of the corresponding module is displayed.  


  - *Created by*  
    Name and user name of the user who initiated the process.

  - *Modified by*  
    Name and user name of the user who modified the process.



## Process ID

*Workflows > Processes > Tab OVERVIEW > Select a process*

![Process ID](/Assets/Screenshots/ActindoWorkFlow/Processes/Actions.png "[Process ID]")

**Process ID**

- ![Back](/Assets/Icons/Back02.png "[Back]") (Back)  
  Click this button to close the *Process ID* view and return to the list of processes.

- *Process ID*  
  Process identification number. The ID number is automatically assigned by the system.

- *Workflow*  
  Name of the workflow.


### Actions

*Workflows > Processes > Tab OVERVIEW > Select a process > Tab Actions*

![Actions](/Assets/Screenshots/ActindoWorkFlow/Processes/Actions.png "[Actions]")

> [Info] The *Actions* tab is selected by default when selecting a process. This tab is an excerpt of the *Process Actions* menu entry, which displays a list of all process actions. When clicking an action in the *Process Actions* view, the selected action is displayed in the *Actions* tab of the corresponding *Process ID* view. For detailed information, see [Process Actions](04a_ProcessActions.md).

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
Click the drop-down list to select an action status. The following options are available:  

    - **All**  
    Select this option to display all actions, regardless of their status.

    - **In progress**  
    Select this option to display the actions that are currently active.

    - **Done**  
    Select this option to display the actions that have been already executed.  

    - **Error**  
    Select this option to display the actions that have given an error.

    - **Error; automatic retry**  
    Select this option to display the actions that have given an error but are set for automatic retry.

    - **Suspended**  
    Select this option to display the actions that have been manually paused.

    - **Process aborted**  
    Select this option to display the actions included in a process that has been manually ended.



- ![Search](/Assets/Icons/Search.png "[Search]") (Search)  
    Click this button to display the search bar and search for an action.

    > [Info] The search function can be used to search for a transition name. At least 3 characters must be entered.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)  
    Click this button to update the list of actions.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)  
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)  
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.


The list displays all executed actions that are matching the selected status. Depending on the settings, the displayed columns may vary. All fields are read-only.

  - [x]    
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all actions in the list are selected.

  Depending of the process status, the editing toolbar may display different options.

  - ![Retry](/Assets/Icons/Retry01.png "[Retry]") (Retry)  
    Click this button to retry the action. This button is displayed when the action status is *Error*.
  - ![Suspend](/Assets/Icons/Pause.png "[Suspend]") (Suspend)  
    Click this button to suspend the action temporarily. This button is displayed when the action status is *In Progress*. When clicking this button, the action status changes to *Suspended*.
  - ![Start](/Assets/Icons/Play.png "[Start]") (Start)  
    Click this button to resume the action. This button is displayed when the action status is *Suspended*. When clicking this button, the action status changes again to *In Progress*. The warning sign in the *Suspended Actions* column of the *Processes* view is no longer displayed.
  - [REMOVE DEFER TIME]  
    Click this button to skip the defer time preconfigured in the action, if any. The action is then executed immediately. This button is displayed when the action status is *In Progress*.

    > [Info] The defer time is preconfigured pro action in the system. If the defer time is removed once, the action is executed immediately. If the action gives an error again, it will be retried once that preconfigured defer time has elapsed.


  - *Status*  
  Status of the action. The different process statuses are displayed in different colors. The following statuses are possible:

    - **In progress** (blue)
    - **Done** (green)
    - **Error** (red)
    - **Error; automatic retry**  
    - **Suspended** (dark gray)
    - **Process aborted** (black)


  - *Transition*  
  Transition key.

  - *Tries*  
  Number of times the action execution has been tried.

  - *Max retries after error*  
  Number of times the action execution must be retried after error.

  > [Info] This setting depends on the transition and is usually preconfigured. In the current version, this value can be modified in the *Import JSON* window, see [Import JSON](02a_Workflows.md#import-json).


  - *Queue Type*  
  Queue type assigned to the action. By default, the *Default* queue type is assigned. For detailed information about configuring queue types, see [Configure the queue types](/ActindoWorkFlow/Integration/01_ConfigureQueueTypes.md).

  > [Info] A different queue type can be selected by editing an action in the workflow editor, see [Edit an action](/ActindoWorkFlow/Operation/01_ManageWorkflows.md#edit-an-action).

  - *Defer until*  
  Next point in time when the action is being tried.  

  > [Info] This setting depends on the action and is not available in all actions.

  - *Created*  
  Date and time of creation.

  - *Modified*  
  Date and time of modification.

  - *ID*  
  Action identification number. The ID number is automatically assigned by the system.

  - *Transition ID*  
  Transition identification number. The ID number is automatically assigned by the system.


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
  Select this option to display all logs regardless of their level.
  - **Debug**
  Select this option to display all logs with **Debug** level.
  - **Info**  
  Select this option to display all logs with **Info** level.
  - **Notice**
  Select this option to display all logs with **Notice** level.
  - **Warning**
  Select this option to display all logs with **Warning** level.
  - **Error**  
  Select this option to display all logs with **Error** level.
  - **Critical**
  Select this option to display all logs with **Critical** level.
  - **Alert**
  Select this option to display all logs with **Alert** level.
  - **Emergency**
  Select this option to display all logs with **Emergency** level.


- ![Search](/Assets/Icons/Search.png "[Search]") (Search)  
Click this button to display the search bar and search for a log.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)  
Click this button to update the list of logs.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)  
Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)  
Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.


The list displays all logs that are matching the selected log level. Depending on the settings, the displayed columns may vary. All fields are read-only. Click a log to display the *Log ID* view, see [Log ID](#Log-ID).


  - *Type*  
  Log level. The following levels can be displayed:

    - **Debug**
    - **Info**
    - **Notice**
    - **Warning**
    - **Error**
    - **Critical**
    - **Alert**
    - **Emergency**


  - *Log Message*  
  Description of the issue.

  - *Workflow*  
  Workflow to which the log message refers.

  - *Workflow ID*    
  Workflow identification number. The ID number is automatically assigned by the system.

  - *Created*  
  Date and time of creation.

  - *ID*  
  Log identification number. The ID number is automatically assigned by the system.

  - *Transition*  
  Key of the transition to which the log refers.

  - *Transition ID*  
  Identification number of the transition to which the log refers. The ID number is automatically assigned by the system.

  - *Created by*  
  Name and user name of the user who initiated the process.



### Tokens

*Workflows > Processes > Tab OVERVIEW > Select a process > Tab Tokens*

![Tokens](/Assets/Screenshots/ActindoWorkFlow/Processes/Tokens.png "[Tokens]")


- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Hide processed*  
Disable this toggle to display all tokens, including the ones that have already been processed. Enable the toggle to hide all processed tokens. By default, this toggle is enabled.

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
    Click this button to display the search bar and search for a token.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)  
    Click this button to update the list of tokens.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)  
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The x indicates the number of columns that are currently displayed in the list.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)  
    Click this button to display the filter bar and customize the active filters. The x indicates the number of filters that are currently active.


The list displays all tokens if the *Hide processed* toggle is disabled. Depending on the settings, the displayed columns may vary. All fields are read-only.

  - *Status*  
  Token status. The different statuses are displayed in different colors. The following statuses are possible:

    - *Processed* (green)
    - *Being processed* (blue)
    - *Error* (red)
    - *Unprocessed* (white)


  - *Place*  
  Name of the place where the token is currently processed.

  > [Info] The start place name is *input*, the end place name *output*.

  - *Data*  
  Type of data contained in the token.

  - *Next possible action(s)*    
  Next compatible action(s) that may consume this token.

  [comment]: <> (Anmerkung Oli: Aus früheren Zeiten -> wird ggf. gestrichen?)

  - *ID*  
  Token identification number. The ID number is automatically assigned by the system.

  - *Place ID*  
  Place identification number. The ID number is automatically assigned by the system.

  - *Process Action ID*  
  Action identification number. The ID number is automatically assigned by the system.



### Create view

*Workflows > Processes > Tab OVERVIEW > Button Points > Menu entry create*

![Create view](/Assets/Screenshots/ActindoWorkFlow/Workflows/CreateView.png "[Create view]")


- *Name*  
Enter a name for the view.

- [CANCEL]  
Click this button to cancel creating a view. The *Create view* window is closed.

- [SAVE]  
Click this button to save the new view. The *Create view* window is closed. The view is saved and displayed in the *View* drop-down list.



### Rename view

*Workflows > Processes > Tab OVERVIEW > Button Points > Menu entry rename*

![Rename view](/Assets/Screenshots/ActindoWorkFlow/Workflows/RenameView.png "[Rename view]")


- *Name*  
Click the field to edit the view name.

- [CANCEL]  
Click this button to cancel renaming a view. The *Rename view* window is closed.

- [SAVE]  
Click this button to save the changes to the view name. The *Rename view* window is closed. The new name for the view is saved and displayed in the *View* drop-down list.



#### Log ID

*Workflows > Processes > Tab OVERVIEW > Select a process > Tab Logs > Select Log Message*

![Log ID](/Assets/Screenshots/ActindoWorkFlow/Processes/LogID.png "[Log ID]")

- ![Back](/Assets/Icons/Back02.png "[Back]") (Back)  
Click this button to close the *Log ID* view and return to the *Logs* tab in the *Process ID* view.


**Log Message**  

In the *Log Message* section, detailed information about the log is displayed. All fields are read-only.

- *Log Level*  
Log level type. The following levels can be displayed:

  - **Debug**
  - **Info**
  - **Notice**
  - **Warning**
  - **Error**
  - **Critical**
  - **Alert**
  - **Emergency**


- Log message box   
  Detailed log message with further information.

  > [Info] In case of an error, detailed information is provided (stack trace) for reporting and debugging purposes.

- *Created - by*  
Date and time of creation, name and user name of the user who initiated the process.

- *Workflow*  
Workflow ID number and name.

- *Process*  
Process ID number and description.

- *Transition*  
Transition ID number and description.
