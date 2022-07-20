[!!Workflows](ActindoWorkFlow)

# Manage the workflows

The *Workflows* module allows the customers to define their own business processes, such as orders, shipments, returns, etc.
The workflows can be created individually in the workflow editor, they can be edited subsequently and by publishing and unpublishing a workflow, the usage can be controlled. Further, obsolete workflows can be deleted.


## Create a workflow

Create a workflow to define a new process.

### Prerequisites

No prerequisites to fulfill.

### Procedure

*Workflows > Workflows > Tab OVERVIEW*

![Workflows](/Assets/Screenshots/ActindoWorkFlow/Workflows/Workflows.png "[Workflows]")

1. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The *New Workflow* window is displayed.

  ![New workflow](/Assets/Screenshots/ActindoWorkFlow/Workflows/NewWorkflow.png "[New workflow]")

2. Enter a name for the new workflow in the *Select a name for your new workflow* field.

3. Enter a key for the workflow in the *Select a unique key for your new workflow* field. The key is required for API access and must be unique within the workflow version.

4. Click the *Choose the data type of your start place* field and enter the name of the place or a keyword you are searching for.

  > [Info] The list of places is filtered for your keyword as you type.

5. Click the start place you want to add in the list of places.    

6. Click the *Choose the data type of your end place* field and enter the name of the place or a keyword you are searching for.

  > [Info] The list of places is filtered for your keyword as you type.

7. Click the end place you want to add in the list of places.  

8. Click the [CREATE] button in the bottom right corner.   
  The new workflow is created. The *New Workflow* window is closed. The workflow editor with the defined start and end places is displayed.  

  ![Workflow editor new](/Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowEditorNew.png "[Workflow editor new]")

#### Create an action

1. Click the ![Add](/Assets/Icons/Plus04.png "[Add]") (Add) button next to the place or click the [NEW ACTION] button on the right hand above the workflow editor.     
  A window to search for an action is displayed.

  ![Search action](/Assets/Screenshots/ActindoWorkFlow/Workflows/SearchAction.png "[Search action]")

2. Click the *search for an action* field and enter the name of the action or a keyword you are searching for. If you have clicked the ![Add](/Assets/Icons/Plus04.png "[Add]") (Add) button next to a place, only those actions that are compatible with the data type of the place are displayed in the list.

  > [Info] The list of actions is filtered for your keyword as you type.

3. Click the action you want to add in the list of actions.
  The action is added to the workflow. If the action was added from a place which requires a certain input data type, the arc from the place is automatically connected to the corresponding input port of the action.

  ![First action](/Assets/Screenshots/ActindoWorkFlow/Workflows/FirstAction.png "[First action]")

  > [Info] If any input port or output port of the new action is mandatory, an arc and a place are automatically displayed with the corresponding action.


#### Connect the action

1. Click the ![Add](/Assets/Icons/Plus04.png "[Add]") (Add) button next to an output port of the action.    
  A new place connected with an arc to the selected output port is displayed.

  ![First place](/Assets/Screenshots/ActindoWorkFlow/Workflows/FirstPlace.png "[First place]")

2. Add further actions by following the procedure [Create an action](#create-an-action) or connect the place with the end place as described in the following step.

  > [Info] A workflow must contain at least one action and can contain an unlimited number of actions.

3. Click the place, drag it over the place to which you want to connect it and drop it.     
  The places are merged and the new connection is created.


### Next steps

- [Edit a workflow](#edit-a-workflow)
- [Publish a workflow](#publish-a-workflow)
- [Unpublish a workflow](#unpublish-a-workflow)
- [Delete a workflow](#delete-a-workflow)
- [Track a workflow process](02_TrackProcesses.md)

### See also

- [User Interface workflows](/ActindoWorkFlow/UserInterface/00_UserInterface.md)
- [Workflow and process elements](/ActindoWorkFlow/Overview/02_WorkflowProcessElements.md)



## Edit a workflow

Edit a workflow to modify elements within the workflow, to extend the workflow by adding further actions or to reduce the workflow by removing actions.

### Prerequisites

- At least one workflow is created, see [Create a workflow](#create-a-workflow).
- You have the required rights to edit a workflow.

### Procedure

*Workflows > Workflows > Tab OVERVIEW*

![Workflows](/Assets/Screenshots/ActindoWorkFlow/Workflows/Workflows.png "[Workflows]")

1. Click the workflow you want to edit in the list of workflows.   
  The *Workflow Versions* view with all versions of the selected workflow is displayed.

  ![Workflow versions](/Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowVersions.png "[Workflow versions]")

2. Click the workflow version you want to edit in the list of workflow versions.  
The workflow editor is displayed in the workspace.

[comment]: <> (Step 2 as well as the screenshot workflow versions is possibly not needed in the next workflows version as the version view will disappear and clicking the workflow will take you to the editor directly, check next time)

  ![Workflow editor](/Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowEditor.png "[Workflow editor]")

3. Make the desired changes in the workflow. The following procedures are described in detail below:
  - [Edit the place data type](#edit-the-place-data-type)
  - [Change the place ports](#change-the-place-ports)
  - [Add an action](#add-an-action)
  - [Edit an action](#edit-an-action)


#### Edit the place data type

1. Click the place you want to edit.    
  The place is highlighted and its settings are displayed in the settings side bar on the right.

  ![Place](/Assets/Screenshots/ActindoWorkFlow/Workflows/Place.png "[Place]")

2. Click the *Data Container* field in the settings side bar and select the appropriate data type in the list of data types.

  > [Info] Only values of those data types that match with the connected output and input port of the selected place are displayed in the list.     


#### Change the place ports

1. Navigate to the place whose input or output port you want to edit.  

2. Click the arc right or left to the place to change the input or output port. To change the input port, click the arc right to the place, to change the output port, click the arc left to the place.   
The selected arc is highlighted.

  ![Input](/Assets/Screenshots/ActindoWorkFlow/Workflows/ArrowInput.png "[Input]")

3. Press **BackSpace** or **Delete** to remove the selected arc.    
  The selected arc between the place and the port is deleted.

  > [Info] If the port whose connection is deleted is mandatory, a new place connected to this port is automatically displayed.

4. Click the ![Add](/Assets/Icons/Plus04.png "[Add]") (Add) button next to the port you want to connect the place with.    
  A new place with a connection to the selected port is displayed.

5. Click the new place, drag it over the place whose connection you have deleted and drop it.     
  The places are merged and the new connection is created.


#### Delete a place

1. Navigate to the place you want to delete.  

2. Click the place to be deleted.   
  The selected place is highlighted.

  ![Input](/Assets/Screenshots/ActindoWorkFlow/Workflows/Place.png "[Input]")

3. Press **Delete** to remove the selected place.    
  The selected place and its arcs are deleted.

  > [Info] If a one of the arcs has been connected to a mandatory input or output port, a new place connected to this port is automatically displayed.



#### Add an action

1. Navigate to the part in the workflow where you want to add an action.  

2. Click the ![Add](/Assets/Icons/Plus04.png "[Add]") (Add) button next to the output port to which you want to connect a new action.     
A new place connected to the selected output port is displayed.

  > [Info] If a place to the output port already exists, for instance because it is mandatory, you can skip the step **2**.                                                                 .

  ![New place](/Assets/Screenshots/ActindoWorkFlow/Workflows/NewPlace.png "[New place]")

3. Click the ![Add](/Assets/Icons/Plus04.png "[Add]") (Add) button right to the new place.    
  A window to search for an action is displayed.

  ![Search action](/Assets/Screenshots/ActindoWorkFlow/Workflows/SearchAction.png "[Search action]")

4. Click the *search for an action* field and enter the name of the action or a keyword you are searching for.

  > [Info] The list of actions is filtered for your keyword as you type.

5. Click the action you want to add in the list of actions.    
  The action is added to the workflow and connected to the selected place.

  ![Add action](/Assets/Screenshots/ActindoWorkFlow/Workflows/AddAction.png "[Add action]")


#### Edit an action

1. Click the action you want to edit.  
  The action is highlighted and its settings are displayed in the settings side bar on the right.

  ![Action](/Assets/Screenshots/ActindoWorkFlow/Workflows/Action.png "[Action]")

  > [Info] The settings displayed in the settings side bar may differ depending on the respective action. The sections *Configuration* and *Static Inputs* are only available for certain actions.     


2. Edit the settings field in the settings side bar. You can change the label, the queue type, the task event, the configuration and the static inputs as described below:

  + Click the *Label* field and edit the name of the action displayed in the workflow editor.

  + Click the *Queue Type* drop-down list and select the appropriate queue type for the action. All available queue types are displayed in the drop-down list. By default the *Default* queue type is selected. You can define a different queue type for each action within the workflow.   
  For detailed information about the queue types, see [Configure the queue types](/ActindoWorkFlow/Integration/01_WConfigureQueueTypes.md).

  + Click the *Task Event* drop-down list and select an event connected to the action. The event is triggered and the corresponding task is assigned when the process action is failed. All available task events are displayed in the drop-down list. By default, the *ActindoWorkflow Process Execution Failed* event is preselected. The drop-down list is only displayed when the *Task* module is installed and the current user has the required rights to configure it.

  + Edit the field(s) in the *Configuration* section to define further configuration settings to the selected action. This section is only displayed for certain actions. The fields displayed in the *Configuration* section depend on the selected action.

  + Click the ![Add](/Assets/Icons/Plus04.png "[Add]") (Add) button right to an input name in the *Static Inputs* section to add a static data value to the corresponding input. All input ports that are not yet connected to a place are displayed in this section. Enter the appropriate value in the text field below the input name. The value entered must be a valid JSON value. Click the ![Delete](/Assets/Icons/Trash07.png "[Delete]") (Delete) button right to a value to delete it. This section is only displayed for certain actions.

  > [Info] Input ports with an static input value cannot be connected to a place. Therefore, a small arrow without a place is displayed in front of an input port with a static input value. Delete the static input value from the port to be able to connect it with a place.     

[comment]: <> (Check the design of static input before next version is released; design possibly changes)
[comment]: <> (Add a link to the Tasks module/task events when documented)

### Next steps

- [Publish a workflow](#publish-a-workflow)
- [Unpublish a workflow](#unpublish-a-workflow)
- [Delete a workflow](#delete-a-workflow)
- [Track a workflow process](02_TrackProcesses.md)

### See also

- [User Interface workflows](/ActindoWorkFlow/UserInterface/00_UserInterface.md)
- [Create a workflow](#create-a-workflow)
- [Workflow and process elements](/ActindoWorkFlow/Overview/02_WorkflowProcessElements.md)



[comment]: <> (add information or delete the publish/unpublish workflow chapters)

## Publish a workflow

Workflows overview (manager?) -> List of all existing workflows

Workflows can have different versions e.g. if you want to add/remove steps in a particular version, for testing purposes before publishing, etc. It is possible to change between versions. Versions can be published/unpublished. Per default, the last published version is used.

- Unpublish a workflow

Workflows > Workflows > Tab OVERVIEW > Select checkbox > Button [VERÖFFENTLICHUNG ZURÜCKZIEHEN]

### Prerequisites

### Procedure

### Next steps

- [Unpublish a workflow](#unpublish-a-workflow)
- [Delete a workflow](#delete-a-workflow)
- [Track a workflow process](02_TrackProcesses.md)

### See also

- [User Interface workflows](/ActindoWorkFlow/UserInterface/00_UserInterface.md)
- [Create a workflow](#create-a-workflow)
- [Edit a workflow](#edit-a-workflow)
- [Workflow and process elements](/ActindoWorkFlow/Overview/02_WorkflowProcessElements.md)



## Unpublish a workflow

Workflows overview (manager?) -> List of all existing workflows

Workflows can have different versions e.g. if you want to add/remove steps in a particular version, for testing purposes before publishing, etc. It is possible to change between versions. Versions can be published/unpublished. Per default, the last published version is used.


- Unpublish a workflow

Workflows > Workflows > Tab OVERVIEW > Select checkbox > Button [VERÖFFENTLICHUNG ZURÜCKZIEHEN]

### Prerequisites

### Procedure

### Next steps

- [Delete a workflow](#delete-a-workflow)
- [Track a workflow process](02_TrackProcesses.md)

### See also

- [User Interface workflows](/ActindoWorkFlow/UserInterface/00_UserInterface.md)
- [Publish a workflow](#publish-a-workflow)
- [Create a workflow](#create-a-workflow)
- [Edit a workflow](#edit-a-workflow)
- [Workflow and process elements](/ActindoWorkFlow/Overview/02_WorkflowProcessElements.md)



## Delete a workflow

You can delete a workflow version that is obsolete. To prevent any problems, it is strongly recommended not to delete a workflow. Instead, you can unpublish a workflow.

### Prerequisites

At least one workflow is created, see [Create a workflow](#create-a-workflow).

### Procedure

*Workflows > Workflows > Tab OVERVIEW*

![Workflows](/Assets/Screenshots/ActindoWorkFlow/Workflows/Workflows.png "[Workflows]")

1. Click the workflow whose version you want to delete in the list of workflows.   
  The *Workflow Versions* view with all versions of the selected workflow is displayed.

  ![Workflow versions](/Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowVersions.png "[Workflow versions]")

2. Select the checkbox of the workflow version you want to delete in the list of workflow versions.  
The editing toolbar is displayed above the workflow versions list.

3. Click the ![Delete](/Assets/Icons/Trash03.png "[Delete]") (Delete) button in the toolbar.
The workflow is deleted.

[comment]: <> (Prüfen, ob das richtig und vollständig ist)

### Next steps

- [Track a workflow process](02_TrackProcesses.md)

### See also

- [User Interface workflows](/ActindoWorkFlow/UserInterface/00_UserInterface.md)
- [Unpublish a workflow](#unpublish-a-workflow)
- [Publish a workflow](#publish-a-workflow)
- [Create a workflow](#create-a-workflow)
- [Edit a workflow](#edit-a-workflow)
- [Workflow and process elements](/ActindoWorkFlow/Overview/02_WorkflowProcessElements.md)
