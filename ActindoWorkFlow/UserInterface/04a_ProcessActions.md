[!!Workflows](ActindoWorkFlow)

# Overview

*Workflows > Process Actions > Tab OVERVIEW*

![Actions](/Assets/Screenshots/ActindoWorkFlow/ProcessActions/ProcessActions.png "[Actions]")

**Actions**
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
Click the drop-down list to select a process status. The following statuses are available:  

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
    Click this button to display the search bar and search for an action.

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)  
    Click this button to update the list of actions.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)  
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)  
    Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.


The list displays all actions that are matching the selected status. Depending on the settings, the displayed columns may vary. All fields are read-only. Click an action to display the corresponding process in the *Process ID* view, see [Process ID](03a_Processes.md#process-id).

> [Info] When clicking an action in the *Process Actions* view, the selected action is displayed in the *Actions* tab of the corresponding *Process ID* view. The *Actions* tab of the *Process ID* view is, in fact, an excerpt of the *Process Actions* menu entry. Click the *Logs* tabs in the *Process ID* view for detailed information about the selected process actions, see [Logs](06a_Logs.md).


  - [x]    
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all actions in the list are selected.

  Depending on the action status, the editing toolbar displays the following buttons:

  - ![Retry](/Assets/Icons/Retry01.png "[Retry]") (Retry)  
    Click this button to retry the action. This button is displayed when the action status is *Error*.
  - ![Suspend](/Assets/Icons/Pause.png "[Suspend]") (Suspend)  
    Click this button to suspend the action temporarily. This button is displayed when the action status is *In Progress*. When clicking this button, the action status changes to *Suspended*.
  - ![Start](/Assets/Icons/Play.png "[Start]") (Start)  
    Click this button to resume the action. This button is displayed when the action status is *Suspended*. When clicking this button, the action status changes again to *In Progress*. The warning sign in the *Suspended Actions* column of the *Processes* view is no longer displayed.
  - [REMOVE DEFER TIME]  
    Click this button to skip the defer time preconfigured in the action, if any. The action is then executed immediately. This button is displayed when the action status is *In Progress*.

  [comment]: <> (Oli: Stimmt das so? Wird die Zeit zum Ausführen der Aktion einmalig vorgezogen? Und wenn es dann aber wieder nicht klappt, greift wieder die eingestellte defer time? Oder was passiert dann?)


  - *Status*  
  Status of the action. The different process statuses are displayed in different colors. The following statuses are possible:

    - *Active*  
    - *Done*  
    - *Error*  
    - *Error; automatic retry*  
    - *Suspended*  
    - *Process aborted*  

  [comment]: <> (Oli: Farbe bestätigen? Alternativ, abwarten auf endgültige UI von Ina?)
  [comment]: <> (Add color code and sign! Auch andere Dateien.)

  - *Transition*  
  Action key.

  - *Tries*  
  Number of times the action execution has been tried.

  - *Max retries after error*  
  Number of times the action execution must be retried after error.

  > [Info] This setting depends on the action and is usually preconfigured.

[comment]: <> (Question pending for OLI)

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

  [comment]: <> (Oli fragen)

  - *Transition ID*  
  Action identification number. The ID number is automatically assigned by the system.


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
