[!!User Interface Workflows](../UserInterface/02a_Workflows.md)
[!!Workflow and process elements](../Overview/04_WorkflowProcessElements.md)
[!!Track a workflow process](./02_TrackWorkflowProcess.md)


# Manage the triggers

When designing a workflow to map a business process, the *Triggers* function allows the user to determine the specific events that will start an action within the workflow. Any event can trigger an action, for instance a change in a product or a product attribute, and multiple conditions and variables can be set.

[comment]: <> (event here misleading, as Event already used in New trigger definition with possible values "After creation" and "After saving")

Triggers can be created, edited or deleted in the workflow editor.

## Create a trigger

Create a trigger to determine a new event to start an action.

#### Prerequisites

- At least one workflow has been created, see [Create a workflow](./01_ManageWorkflows.md#create-a-workflow).
- You have the required rights to edit a workflow.

[comment]: <> (The workflow has to be created before you can add the trigger? Or can your add triggers while you create the workflow? Triggers come first in the workflow versions...)

[comment]: <> (Add triggers info to Workflow process elements and UI)

#### Procedure

*Workflows > Workflows > Tab OVERVIEW*

![Workflows](../../Assets/Screenshots/ActindoWorkFlow/Workflows/Workflows.png "[Workflows]")

1. Select a workflow from the *Workflows* list.  
The *Workflow versions* view with all versions of the selected workflow is displayed.

  ![Workflow versions](../../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowVersions.png "[Workflow versions]")

2. Select the workflow version where the trigger is to be added.  
The workflow editor is displayed.

[comment]: <> (Evtl. 1 + 2 als prereq)

3. Click the ![Points](../../Assets/Icons/Points02.png "[Points]") (Points) button in the upper left corner next to the workflow name.   
  The workflow context menu is displayed.

  ![Context menu](../../Assets/Screenshots/ActindoWorkFlow/Workflows/ContextMenu02.png "[Context menu]")

4. Click the *Triggers* menu option.  
The *Edit trigger for workflow name* window is displayed.

  ![Edit trigger](../../Assets/Screenshots/ActindoWorkFlow/Workflows/EditTrigger01.png "[Edit trigger]")

5. Click the ![Add](../../Assets/Icons/Plus04.png "[Add]") (Add) button to create a trigger.  
A *New trigger* input line is displayed.

6. Follow the steps below to add a new trigger:
  - Enter a description in the *Name* field.  
  - Enter the applicable data model that will trigger the new action in the *Model* field, for example a PIM product.  
  - Click the drop-down list and select the appropriate option.   The following options are available:
    - After creation   
    Select this option if the model
    - After saving   



6.





## Edit a trigger

#### Prerequisites

No prerequisites to fulfill.

#### Procedure

*Workflows > Workflows > Tab OVERVIEW*

![Triggers](../../Assets/Screenshots/ActindoWorkFlow/Workflows/.png "[Triggers]")



## Delete a trigger

#### Prerequisites

No prerequisites to fulfill.

#### Procedure

*Workflows > Workflows > Tab OVERVIEW*

![Triggers](../../Assets/Screenshots/ActindoWorkFlow/Workflows/.png "[Triggers]")
