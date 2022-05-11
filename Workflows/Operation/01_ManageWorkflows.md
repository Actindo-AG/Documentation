[!!Workflows](Workflows)

# Manage the workflows

The *Workflows* module allows the customers to define their own business processes, such as orders, shipments, returns, etc.
The workflows can be created individually in the workflow editor, they cna be edited subsequently and by publishing and npublishing a workflow, the usage can be controlled. Further, obsolete workflows can be deleted.

## Create a workflow

### Prerequisites

### Procedure

*Workflows > Workflows > Tab OVERVIEW*

Zoom in / out with mouse wheel or Ctrl +/-, move around with drag and drop (mouse link click and moving mouse in desired direction) in Workflow editor.

To link/join nodes together, drag and drop.

### Next steps

- [Edit a workflow](#edit-a-workflow)
- [Publish a workflow](#publish-a-workflow)
- [Unpublish a workflow](#unpublish-a-workflow)
- [Delete a workflow](#delete-a-workflow)

### See also



## Edit a workflow

### Prerequisites

At least one workflow is created, see [Create a workflow](#create-a-workflow).

### Procedure

*Workflows > Workflows > Tab OVERVIEW*

![Workflows](/Assets/Screenshots/Workflows/Workflows/Workflows.png "[Workflows]")

1. Click the workflow you want to edit in the list of workflows.   
  The *Workflow Versions* view with all versions of the selected workflow is displayed.

  ![Workflow versions](/Assets/Screenshots/Workflows/Workflows/WorkflowVersions.png "[Workflow versions]")

2. Click the workflow version you want to edit in the list of workflow versions.  
The workflow editor is displayed in the workspace.

  ![Workflow editor](/Assets/Screenshots/Workflows/Workflows/WorkflowEditor.png "[Workflow editor]")

3. Make the desired changes in the workflow. The following procedures are described in detail below:
  - [Edit the place data type](#edit-the-place-data-type)
  - [Change the place ports](#change-the-place-ports)
  - [Create an action](#create-an-action)
  - [Edit an action](#edit-an-action)


#### Edit the place data type

1. Click the place you want to edit.    
  The place is highlighted and its settings are displayed in the settings side bar on the right.

  ![Place](/Assets/Screenshots/Workflows/Workflows/Place.png "[Place]")

2. Click the *Data Container* field in the settings side bar and select the appropriate data type in the list of data types.

  > [Info] Only values of those data types that matches with the connected output and input port of the selected place are displayed in the list.     


#### Change the place ports

1. Navigate to the place whose input or output port you want to edit.  

2. Click the arrow right or left to the place to change the input or output port. To change the input port, click the arrow right to the place, to change the output port, click the arrow left to the place.   
The selected arrow is highlighted.

  ![Input](/Assets/Screenshots/Workflows/Workflows/ArrowInput.png "[Input]")

3. Press **BackSpace** or **Delete** to remove the selected connection.    
  The selected connection between the place and the port is deleted.

  > [Info] If the port whose connection is deleted is mandatory, a new place connected to this port is automatically displayed.

4. Click the ![Add](/Assets/Icons/Plus04.png "[Add]") (Add) button next to the port you want to connect the place with.    
  A new place with a connection to the selected port is displayed.

5. Click the new place, drag it over the place whose connection you have deleted and drop it.     
  The places are merged and the new connection is created.


#### Create an action

1. Navigate to the part in the workflow where you want to add an action.  

2. Click the ![Add](/Assets/Icons/Plus04.png "[Add]") (Add) button next to the output port to which you want to connect a new action.     
A new place connected to the selected output port is displayed.

  > [Info] If a place to the output port already exists, for instance because it is mandatory, you can skip the step **2**.                                                                 .

  ![New place](/Assets/Screenshots/Workflows/Workflows/NewPlace.png "[New place]")

3. Click the ![Add](/Assets/Icons/Plus04.png "[Add]") (Add) button right to the new place.    
  A window to search for an action is displayed.

  ![Search action](/Assets/Screenshots/Workflows/Workflows/SearchAction.png "[Search action]")

4. Enter the name of the action or a keyword you are searching for in the *search for an action* bar.

  > [Info] The list of actions is filtered for your keyword as you type.

5. Click the action you want to add in the list of actions.    
  The action is added to the workflow and connected to the selected place.

  ![Add action](/Assets/Screenshots/Workflows/Workflows/AddAction.png "[Add action]")



#### Edit an action

1. Click the action you want to edit.  
  The action is highlighted and its settings are displayed in the settings side bar on the right.

  ![Action](/Assets/Screenshots/Workflows/Workflows/Action.png "[Action]")

  > [Info] The settings displayed in the settings side bar may differ depending on the respective action. The sections *Configuration* and *Static Inputs* are only available for certain actions.     


2. Click the settings field you want to edit in the settings side bar. You can change the label, the queue type, the task event,  the configuration and the static inputs as described below:

  + Click the *Label* field and edit the name of the action displayed in the workflow editor.

  + Click the *Queue Type* drop-down list and select the appropriate queue type for the action. All available queue types are displayed in the drop-down list. By default the *Default* queue type is selected. You can define a different queue type for each action within the workflow.

  + Click the *Task Event* drop-down list and select an event connected to the action. The event is triggered and the corresponding task is assigned when the action is executed within a process. All available task events are displayed in the drop-down list. By default, no event is selected.

  + Click the *PHP Code* text area in the *Configuration* section to add further configuration settings to the selected action. This section is only displayed for certain actions.

  + Click the ![Add](/Assets/Icons/Plus04.png "[Add]") (Add) button right to an input name in the *Static Inputs* section to add a value to the input. Enter the appropriate value in the text field below the input name. Click the ![Delete](/Assets/Icons/Trash07.png "[Delete]") (Delete) button right to an input value to delete it. This section is only displayed for certain actions.

  > [Info] The value to be entered in quotation marks must be a valid JSON data type. The following data types are defined:
  - string
  - number
  - object
  - array
  - true
  - false
  - null

[comment]: <> (Task Event: was ist das - welche tasks werden angezeigt? Configuration: Wann, was? Static Inputs: Was mache ich hier? JSON value = data type)   



### Next steps

- [Publish a workflow](#publish-a-workflow)
- [Unpublish a workflow](#unpublish-a-workflow)
- [Delete a workflow](#delete-a-workflow)

### See also

- [Create a workflow](#create-a-workflow)


## Delete a workflow

### Prerequisites

### Procedure

### Next steps

- [Delete a workflow](#delete-a-workflow)
- [Publish/unpublish a workflow](#publish-unpublish-a-workflow)

### See also



## Publish/Unpublish a workflow

Workflows overview (manager?) -> List of all existing workflows

Workflows can have different versions e.g. if you want to add/remove steps in a particular version, for testing purposes before publishing, etc. It is possible to change between versions. Versions can be published/unpublished. Per default, the last published version is used.


- Unpublish a workflow

Workflows > Workflows > Tab OVERVIEW > Select checkbox > Button [VERÖFFENTLICHUNG ZURÜCKZIEHEN]

### Prerequisites

### Procedure

### Next steps

- [Delete a workflow](#delete-a-workflow)
- [Publish/unpublish a workflow](#publish-unpublish-a-workflow)

### See also
