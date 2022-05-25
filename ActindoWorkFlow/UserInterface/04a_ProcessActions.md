[!!Workflows](ActindoWorkFlow)

# Process Actions

*Workflows > Process Actions*

![Actions](/Assets/Screenshots/ActindoWorkFlow/ProcessActions/ProcessActions.png "[Actions]")


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


The list displays all process actions. Depending on the settings, the displayed columns may vary. All fields are read-only. When clicking a process action, the *Actions* tab of the corresponding process is displayed, see [Actions](03a_Processes.md#actions).

[comment]: <> (Jetzt etwas verwirrt zu den Verweisen: Auf Actions oder auf Proces ID verweisen? Wenn ich hier an andere Datei verweise, könnte ich genauso machen mit Create view and Rename view, oder? Das gilt auch für 06a_Logs.md mit den Verweisen auf Create / Rename view und Log ID).

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

[comment]: <> (Editing tool bar - icons Pause/Stop?)

  - *ID*  
  Action ID number.

  [comment]: <> (Oli fragen)

  - *Transition ID*  
  Transition ID number.


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
