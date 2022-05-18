[!!Workflows](ActindoWorkFlow)

# Workflows

*Workflows > Workflows > Tab OVERVIEW*

![Overview](/Assets/Screenshots/ActindoWorkFlow/Workflows/Workflows.png "[Overview]")

The *OVERVIEW* tab displays a list of all available workflows.

- *VIEW*  
Click the drop-down list to select the view. All created views are displayed in the drop-down list. Click the ![Points](/Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *VIEW* drop-down list to display the context menu and create a view. For detailed information, see [Create a view](#create-a-view).

  - View context menu  
  Click the ![Points](/Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *View* drop-down list to display the context menu. The following menu entries are available:

    - ![create](/Assets/Icons/Plus06.png "[create]") create  
    Click this entry to create a view. The *Create view* window is displayed.

[comment]: <> (Oli: View context menu - im Moment nur Create Option. Edit und andere Optionen geplant?)

  - ![Search](/Assets/Icons/Search.png "[Search]") (Search)  
    Click this button to display the search bar and search for a workflow.

  - ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)  
    Click this button to update the list of workflows.

  - ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)  
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The x indicates the number of columns that are currently displayed in the list.

  - ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)  
    Click this button to display the filter bar and customize the active filters. The x indicates the number of filters that are currently active.

The created workflows are displayed in a column view. Depending on the settings, the displayed columns may vary. All fields are read-only.

- *Name*  
  Name of the workflow.

- *Key*  
  Key value given to the workflow.

- *Highest version*  
  Highest existing version of workflow.

- *Highest published version*  
  Highest published version of workflow.

[comment]: <> (Need a better definition of "key"!)

- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)  
Click this button to create a workflow. The *Create new workflow* window is displayed. For detailed information, see [Create a workflow](#create-a-workflow).


## Workflow versions

*Workflows > Workflows > Tab OVERVIEW > Select workflow*

![Workflow versions](/Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowVersions.png "[Workflow versions]")


The *Workflow versions* view displays a list of all available  versions of the selected workflow.

- *VIEW*  
Click the drop-down list to select the view. All created views are displayed in the drop-down list. Click the ![Points](/Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *VIEW* drop-down list to display the context menu and create a view. For detailed information, see [Create a view](#create-a-view).

  - View context menu  
  Click the ![Points](/Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *View* drop-down list to display the context menu. The following menu entries are available:

    - ![create](/Assets/Icons/Plus06.png "[create]") create  
    Click this entry to create a view. The *Create view* window is displayed.

[comment]: <> (Oli: View context menu - im Moment nur Create Option. Edit und andere Optionen geplant?)

  - ![Search](/Assets/Icons/Search.png "[Search]") (Search)  
    Click this button to display the search bar and search for a workflow.

  - ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)  
    Click this button to update the list of workflows.

  - ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)  
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The x indicates the number of columns that are currently displayed in the list.

  - ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)  
    Click this button to display the filter bar and customize the active filters. The x indicates the number of filters that are currently active.

The workflows are displayed in a column view. Depending on the settings, the displayed columns may vary. All fields are read-only.

- *Version*  
  Version number of the workflow.

- *Published*  
  - ![Check](/Assets/Icons/Check.png "[Check]") (Check) means that the workflow version is published.
  - ![Check](/Assets/Icons/Cross02.png "[Cross]") (Cross) means that the workflow version is unpublished.


- [x]  
Select the checkbox to display the editing toolbar.

[comment]: <> (Screenshot mit editing toolbar?)

- [PUBLISH]/[UNPUBLISH]  
Click this button to publish or unpublish a workflow version. For detailed information, see [Publish a workflow](/ActindoWorkFlow/Operation/01_ManageWorkflows.md#publish-a-workflow) and [Unpublish a workflow](/ActindoWorkFlow/Operation/01_ManageWorkflows.md#unpublish-a-workflow).

- [DELETE]  
Click this button to delete the selected workflow version.  

- [VIEW]  
Click this button to view the selected workflow version.

[comment]: <> (Oli: Button DELETE ist i.d.R. ein "Trash" Symbol. Button VIEW funktioniert nicht)


- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)  
Click this button to create a workflow. The *Create new workflow* window is displayed. For detailed information, see [Create a workflow](#create-a-workflow).


## Workflow editor

*Workflows > Workflows > Tab OVERVIEW > Select workflow > Select version*

![Workflow editor](/Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowEditor.png "[Workflow editor]")

- (Workflow name)

-  ![Points](/Assets/Icons/Points01.png "[Points]") (Points)  
Click the ![Points](/Assets/Icons/Points01.png "[Points]") (Points) button to the right of the workflow name to display the context menu. The following menu entries are available:

    - *Rename*  
    Click this entry to rename the workflow.

    - *Settings*

    - *Save as*

    - *Import JSON*

    - *Export JSON*

    - *Deploy*


  [comment]: <> (Context menu options not working yet. Oli: Bleiben alle Funktionen? Unterschied zwischen Deploy and Publish?)

- ![Undo](/Assets/Icons/Undo02.png "[Undo]") (Undo)

- ![Redo](/Assets/Icons/Redo.png "[Redo]") (Redo)

- ![Comment](/Assets/Icons/Comment.png "[Comment]") (Comment)

- [NEW ACTION]  
  Click this button to add a new action. For detailed information, see [Create an action](ActindoWorkFlow/Operation/01_ManageWorkflows.md#create-an-action). A window to search for an action is displayed.


## Create view

*Workflows > Workflows > Tab OVERVIEW > Button Points > Menu entry create*

![Create view](/Assets/Screenshots/ActindoWorkFlow/Workflows/CreateView.png "[Create view]")

- *Name*
Enter a name for the view.

- [CANCEL]  
Click this button to cancel creating a view. The *Create view* window is closed.

- [SAVE]  
Click this button to save the new view. The *Create view* window is closed. The view is saved and displayed in the *View* drop-down list.


## Create a workflow

*Workflows > Workflows > Tab OVERVIEW > Button Add*

![New workflow](/Assets/Screenshots/ActindoWorkFlow/Workflows/NewWorkflow.png "[New workflow]")


## Search for an action window

*Workflows > Workflows > Tab OVERVIEW > Select workflow > Select version > Button NEW ACTION*

![Search for an action](/Assets/Screenshots/ActindoWorkFlow/Workflows/SearchAction.png "[Search for an action]")
