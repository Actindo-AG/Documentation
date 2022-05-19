[!!Workflows](ActindoWorkFlow)

# Workflows

*Workflows > Workflows > Tab OVERVIEW*

![Overview](/Assets/Screenshots/ActindoWorkFlow/Workflows/Workflows.png "[Overview]")

The *Workflows* view displays a list of all available workflows.

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

[comment]: <> (OLI: ADD FILTER button funktioniert noch nicht?)

The created workflows are displayed in a column view. Depending on the settings, the displayed columns may vary. All fields are read-only.

- *Name*  
  Name of the workflow.

- *Key*  
  Key value given to the workflow.

- *Highest version*  
  Highest existing version of the workflow.

- *Highest published version*  
  Highest published version of the workflow.

[comment]: <> (OLI: Was ist ein "Key"? Wie kann man es kurz beschreiben/definieren? Unterschied zu Name?)

- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)  
Click this button to create a workflow. The *New Workflow* window is displayed, see [New Workflow](#new-workflow). For detailed information, see [Create a workflow](#create-a-workflow).



## Workflow versions

*Workflows > Workflows > Tab OVERVIEW > Select workflow*

![Workflow versions](/Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowVersions.png "[Workflow versions]")


The *Workflow versions* view displays a list of all available  versions of the selected workflow.

- ![Back](/Assets/Icons/Back02.png "[Back]") (Back)  
Click this button to close the *Workflow versions* view and return to the *Workflows* view.

- *VIEW*  
Click the drop-down list to select the view. All created views are displayed in the drop-down list. Click the ![Points](/Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *VIEW* drop-down list to display the context menu and create a view. For detailed information, see [Create a view](#create-a-view).

  - View context menu  
  Click the ![Points](/Assets/Icons/Points01.png "[Points]") (Points) button to the right of the *View* drop-down list to display the context menu. The following menu entries are available:

    - ![create](/Assets/Icons/Plus06.png "[create]") create  
    Click this entry to create a view. The *Create view* window is displayed.

[comment]: <> (Oli: View context menu - im Moment nur Create Option. Edit und andere Optionen geplant?)

  - ![Search](/Assets/Icons/Search.png "[Search]") (Search)  
    Click this button to display the search bar and search for a workflow version.

  [comment]: <> (Oli: Dafür gedacht? Scheint nicht wirklich zu funktionieren)

  - ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)  
    Click this button to update the list of workflow versions.

  - ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)  
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The x indicates the number of columns that are currently displayed in the list.

  - ![Filter](/Assets/Icons/Filter.png "[Filter]") Filter (x)  
    Click this button to display the filter bar and customize the active filters. The x indicates the number of filters that are currently active.

The workflow versions are displayed in a column view. Depending on the settings, the displayed columns may vary. All fields are read-only.

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

  > [Info] To prevent any problems, it is strongly recommended not to delete a workflow. For detailed information, see [Delete a workflow](ActindoWorkFlow/Operation/01_ManageWorkflows.md#delete-a-workflow).

- [VIEW]  
Click this button to view the selected workflow version.

[comment]: <> (Oli: Button DELETE ist i.d.R. ein "Trash" Symbol. Button VIEW funktioniert nicht)


- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)  
Click this button to create a workflow version. For detailed information about creating a workflow version, see [Create a workflow version](#to-be-completed).

[comment]: <> (Oli: Add button in Workflow versions funktioniert nicht. Bug, kommt noch oder so gemeint? New workflow Fenster nach klicken angezeigt? Anderes Fenster? Prozedur genauso wie Create worflow? Vgl. Workflow anklicken > Version anklicken > Änderungen in workflow editor > Points button > Deploy -> Neue "published" Version erstellt?)



## Workflow editor

*Workflows > Workflows > Tab OVERVIEW > Select workflow > Select version*

![Workflow editor](/Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowEditor.png "[Workflow editor]")

- ![Back](/Assets/Icons/Back02.png "[Back]") (Back)  
Click this button to close the workflow editor and return to the *Workflows* view.

[comment]: <> (Oli: Back button, oben links, nachdem man eine Workflow version ausgewählt hat: Sollte es nicht zurück zu Workflows versions gehen?)

- (Workflow name)

-  ![Points](/Assets/Icons/Points02.png "[Points]") (Points)  
Click the ![Points](/Assets/Icons/Points02.png "[Points]") (Points) button to the right of the workflow name to display the context menu. The following menu entries are available:

    - *Rename*  
    Click this entry to rename the workflow.

    - *Settings*

    - *Save as*

    - *Import JSON*  
    Click this entry to import data in JSON format. A new window is displayed.

    - *Export JSON*  
    Click this entry to export data in JSON format. A new window is displayed.

    - *Deploy*  
    Click this button to publish a workflow version.


  [comment]: <> (Oli: Context menu options not working yet, except for Import/Export JSON. Beim klicken wird eine Datei in einer neuen Fenster  angezeigt. Bleiben alle Funktionen? JSON Fenster beschrieben? Kann der User da was einstellen? Unterschied zwischen Deploy und Publish?)

- ![Undo](/Assets/Icons/Undo02.png "[Undo]") (Undo)  
  Click this button to undo any changes made.

- ![Redo](/Assets/Icons/Redo.png "[Redo]") (Redo)  
  Click this button to redo any undone changes.

- ![Comment](/Assets/Icons/Comment.png "[Comment]") (Comment)

[comment]: <> (OLI: "Comment" button? Was macht es?)

- [NEW ACTION]  
  Click this button to add a new action. A window to search for an action is displayed, see [Search for an action](#search-for-an-action). For detailed information about creating an action, see [Create an action](ActindoWorkFlow/Operation/01_ManageWorkflows.md#create-an-action).


The workflow diagram is displayed in the workflow editor. For detailed information about the workflow elements, see [Workflow elements](01_WorkflowElements.md).



## Create view

*Workflows > Workflows > Tab OVERVIEW > Button Points > Menu entry create*

![Create view](/Assets/Screenshots/ActindoWorkFlow/Workflows/CreateView.png "[Create view]")


- *Name*  
Enter a name for the view.

- [CANCEL]  
Click this button to cancel creating a view. The *Create view* window is closed.

- [SAVE]  
Click this button to save the new view. The *Create view* window is closed. The view is saved and displayed in the *View* drop-down list.



## New Workflow

*Workflows > Workflows > Tab OVERVIEW > Button Add*

![New workflow](/Assets/Screenshots/ActindoWorkFlow/Workflows/NewWorkflow.png "[New workflow]")


- *Select a name for your new workflow*  
Click this field to enter a name for the new workflow.

- *Select a unique key for your new workflow*  
Click this field to enter a key for the workflow.

- *Choose the data type of your start place*  
Click this field (search bar) to enter the name of the start place or a keyword to search for.

  > [Info] The list of places is filtered for your keyword as you type.

- ![Delete](/Assets/Icons/Cross02.png "[Delete]") (Delete)  
  Click this button to delete the keyword and clear the search bar.

- *Choose the data type of your end place*  
Click this field (search bar) to enter the name of the end place or a keyword to search for.

  > [Info] The list of places is filtered for your keyword as you type.

- ![Delete](/Assets/Icons/Cross02.png "[Delete]") (Delete)  
    Click this button to delete the keyword and clear the search bar.

- [CANCEL]  
Click this button to cancel creating a new workflow. The *New Workflow* window is closed.

- [CREATE]  
Click this button to create a new workflow. The workflow editor with the defined start and end places is displayed.



## Search for an action

*Workflows > Workflows > Tab OVERVIEW > Select workflow > Select version > Button NEW ACTION*

![Search for an action](/Assets/Screenshots/ActindoWorkFlow/Workflows/SearchAction.png "[Search for an action]")

The *Search for an action* window displays a list of all compatible actions for the selected place.


- *Search for an action* (Search bar)
Click this field (search bar) to enter the name of the action or a keyword to search for.

  > [Info] The list of actions is filtered for your keyword as you type.

- ![Delete](/Assets/Icons/Cross02.png "[Delete]") (Delete)  
Click this button to delete the keyword and clear the search bar.
