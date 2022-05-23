[!!Workflows](ActindoWorkFlow)

# Processes

*Workflows > Processes > Tab OVERVIEW*

![Overview](/Assets/Screenshots/ActindoWorkFlow/Processes/Processes.png "[Overview]")

The *Processes* view displays a list of all available processes. Click on a process for further details. The *Process ID* view is displayed.

- *VIEW*  
Click the drop-down list to select the view. All created views are displayed in the drop-down list. Click the ![Points](/Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *VIEW* drop-down list to display the context menu and create a view. For detailed information, see [Create a view](#create-a-view).

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

    - ![Save](/Assets/Icons/Save.png "[Save]") create  
    Click this entry to save the current view settings in the selected view. This menu entry is only displayed when a view is selected.

     > [Info] When the settings of a view have been changed, an asterisk is displayed behind the views name. The asterisk is hidden as soon as the changes have been saved.

    - ![Delete](/Assets/Icons/Trash01.png "[Delete]") delete  
    Click this entry to delete the selected view. A confirmation window to confirm the deletion is displayed. This menu entry is only displayed when a view is selected.


- *Status*  
Click the drop-down list to select a process status. The following options are available:  

    - **All**  
    Select this option to display all processes, regardless of their status.

    - **Ready**  
    Select this option to display the processes that have just been initiated.

    - **In progress**  
    Select this option to display the processes that are currently active.

    - **Error**  
    Select this option to display the processes that have given an error.

    - **Done**  
    Select this option to display the processes that have been completely executed.  

    - **Dead**  
    Select this option to display the processes that have automatically stopped due to a missing input.

    - **Suspended**  
    Select this option to display the processes that have been manually paused.

    - **Aborted**  
    Select this option to display the processes that have been manually stopped.


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


The processes are displayed in a column view. Depending on the settings, the displayed columns may vary. All fields are read-only.

  - [x]  
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all processes in the list are selected.

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

  - *Suspended actions*  

  - *Subject*  

  - *Workflow*  
  Name of the workflow.

  - *Queue Type*  
  Queue type configured in the workflow. For detailed information about configuring the queue types, see [Configure the queue types](ActindoWorkFlow/Integration/01_ConfigureQueueTypes.md).

  - *Priority*

  - *Created*  
  Date of creation.

  - *Last activity*  
  Last time an activity has been registered in the process.



## Process ID

*Workflows > Processes > Tab OVERVIEW > Select a process*

![Process ID](/Assets/Screenshots/ActindoWorkFlow/Processes/Actions.png "[Process ID]")

The *Process ID* view displays a diagram of the selected process including all places and actions. Further details about the process actions included in the diagram as well as about the logs and tokens are displayed in separate tabs in the bottom part of the *Process ID* view. For detailed information, see [Actions](#actions), [Logs](#logs) and [Tokens](#tokens).

[comment]: <> (Intro probably to be changed. Taken from 02_TrackWorfklowProcess.md)

For detailed information about checking the process action status, see [Check the process action status](ActindoWorkFlow/Operation/02_TrackWorfklowProcess.md#check-process-action-status).


### Actions

*Workflows > Processes > Tab OVERVIEW > Select a process*

![Actions](/Assets/Screenshots/ActindoWorkFlow/Processes/Actions.png "[Actions]")

> [Info] The *Actions* tab is selected by default when selecting a process.

- *VIEW*  
Click the drop-down list to select the view. All created views are displayed in the drop-down list. Click the ![Points](/Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *VIEW* drop-down list to display the context menu and create a view. For detailed information, see [Create a view](#create-a-view).

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

    - ![Save](/Assets/Icons/Save.png "[Save]") create  
    Click this entry to save the current view settings in the selected view. This menu entry is only displayed when a view is selected.

     > [Info] When the settings of a view have been changed, an asterisk is displayed behind the views name. The asterisk is hidden as soon as the changes have been saved.

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

    - **Error, automatic retry**  
    Select this option to display the actions that have given an error but are set for automatic retry.

    > [Info] This setting depends on the action and is usually preconfigured.

    - **Suspended**  
    Select this option to display the actions that have been manually paused.

    - **Process aborted**  
    Select this option to display the actions included in a process that has been manually stopped.



- ![Search](/Assets/Icons/Search.png "[Search]") (Search)  
    Click this button to display the search bar and search for a workflow.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)  
    Click this button to update the list of workflows.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)  
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The x indicates the number of columns that are currently displayed in the list.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)  
    Click this button to display the filter bar and customize the active filters. The x indicates the number of filters that are currently active.


The actions are displayed in a column view. Depending on the settings, the displayed columns may vary. All fields are read-only.

  - [x]    
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all actions in the list are selected.

  - *Status*  
  Status of the process. The different process statuses are displayed in different colours. The following statuses are possible:

    - *Active*  
    - *Done*  
    - *Error*  
    - *Error, automatic retry*  
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

  - *Queue type*  
  The *Default* queue type is normally selected. For detailed information about configuring queue types, see [Configure the queue types](01_ConfigureQueueTypes.md).

  > [Info] A different queue type can be selected by editing an action, see [Edit an action](01_ManageWorkflows.md#edit-an-action).

  - *Defer until*  
  Next point in time when the action is being tried.

  [comment]: <> (Configurable? Check Wissentranfer)

  - *Created*  
  Date of creation.

  - *Modified*  
  Date of modification.

[comment]: <> (Editing tool bar - icons Pause/Stop?)


### Logs

*Workflows > Processes > Tab OVERVIEW > Select a process > Tab Logs*

![Logs](/Assets/Screenshots/ActindoWorkFlow/Processes/Logs.png "[Logs]")

The *Logs* tab displays a list of all log messages produced in the course of the process. Click on a log message for further details. The *Process ID* view is displayed.


- *VIEW*  
Click the drop-down list to select the view. All created views are displayed in the drop-down list. Click the ![Points](/Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *VIEW* drop-down list to display the context menu and create a view. For detailed information, see [Create a view](#create-a-view).

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

    - ![Save](/Assets/Icons/Save.png "[Save]") create  
    Click this entry to save the current view settings in the selected view. This menu entry is only displayed when a view is selected.

     > [Info] When the settings of a view have been changed, an asterisk is displayed behind the views name. The asterisk is hidden as soon as the changes have been saved.

    - ![Delete](/Assets/Icons/Trash01.png "[Delete]") delete  
    Click this entry to delete the selected view. A confirmation window to confirm the deletion is displayed. This menu entry is only displayed when a view is selected.


- *Log Level*  
Click the drop-down list to select a log level. The following options are available:  

    - **All**  
    Select this option to display all logs, regardless of their status.

    - **Debug**

    - **Info**

    - **Notice**

    - **Warning**

    - **Error**

    - **Critical**

    - **Alert**

    - **Emergency**



- ![Search](/Assets/Icons/Search.png "[Search]") (Search)  
Click this button to display the search bar and search for a workflow.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)  
Click this button to update the list of workflows.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)  
Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The x indicates the number of columns that are currently displayed in the list.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)  
Click this button to display the filter bar and customize the active filters. The x indicates the number of filters that are currently active.


The actions are displayed in a column view. Depending on the settings, the displayed columns may vary. All fields are read-only.

  - [x]    
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all actions in the list are selected.

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
  Brief description of the issue.

  - *Workflow*  
  Workflow which the log message refers to.

  - *Workflow ID*    
  Workflow ID number.

  - *Created*  
  Date of creation.


### Tokens

*Workflows > Processes > Tab OVERVIEW > Select a process > Tab Tokens*

![Tokens](/Assets/Screenshots/ActindoWorkFlow/Processes/Tokens.png "[Tokens]")


- ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Hide processed*  
Disable this toggle to display all tokens, including the ones that have already been processed.

- *VIEW*  
Click the drop-down list to select the view. All created views are displayed in the drop-down list. Click the ![Points](/Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *VIEW* drop-down list to display the context menu and create a view. For detailed information, see [Create a view](#create-a-view).

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

    - ![Save](/Assets/Icons/Save.png "[Save]") create  
    Click this entry to save the current view settings in the selected view. This menu entry is only displayed when a view is selected.

     > [Info] When the settings of a view have been changed, an asterisk is displayed behind the views name. The asterisk is hidden as soon as the changes have been saved.

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


The tokens are displayed in a column view. Depending on the settings, the displayed columns may vary. All fields are read-only.

  - *Status*  
  Token status. The different statuses are displayed in different colours. The following types are possible:

    - *Ready*
    - *Processed*
    - *Being processed*
    - *Error*

[comment]: <> (Other? Check Wissentransfer? Repeat here or leave it out? Add colour code?)

  - *Place*  
  Place where the token has been input.

  - *Data*  
  Type of data contained in the token.

  - *Next possible action(s)*    
  Next compatible action(s) where the token can be input.



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
