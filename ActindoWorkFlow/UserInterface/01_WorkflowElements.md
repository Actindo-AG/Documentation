[!!Workflows](ActindoWorkFlow)

# Workflow elements

![Workflow](/Assets/Screenshots/ActindoWorkFlow/Workflows/Workflow.png "[Workflow]")

A workflow is represented with a number of fixed elements, each of them having specific characteristics. These elements are used to design the workflow, which can be edited as necessary according to customer needs. For detailed information, see [Manage workflows](/ActindoWorkFlow/Operation/01_ManageWorkflows.md).

A workflow runs from left to right, from a start point to an end point, which can be in turn linked to another workflow. A workflow must contain at least one action between the start and the end point, which are special types of places. The actions are linked through places with each other, connecting the corresponding actions input and output ports. All these elements are described more in detail below.

> [Info] The *Workflows* module is linked to different system modules and plugins, such as *Invoicing*, *Email*, *OmniChannels*, *Tasks*, among others. The actions available to create workflows depend on the modules installed in the system.

[comment]: <> (Processes - The data input at the start point, for example a document, goes through the different workflow stages -places and actions- until it reaches the end point. The process is than completed.)



## Places

![Place](/Assets/Screenshots/ActindoWorkFlow/Workflows/Place.png "[Place]")

A place is a step in the workflow and is represented by circle, usually provided with inward and outward arcs. Places serve as link between two actions, joining an output port from the previous action to the corresponding input port of the following action. Places linking mandatory input/output ports are displayed by default and cannot be deleted. Additional places can be added by clicking on the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button next to the optional input/output port. For detailed information about the types of input/output ports, see [Input and output ports](#input-and-output-ports).

When clicking a place, it becomes highlighted and the corresponding element settings are displayed in the settings side bar.

![Settings side bar](/Assets/Screenshots/ActindoWorkFlow/Workflows/SettingsSideBar01.png "[Settings side bar]")

The place settings side bar is located to the right of the workspace and allows to define the place settings. The following fields are displayed:

  - *Key*  
  Place key. This field is read-only. The key is required for API access and must be system wide unique.

  - *Data container*  
  Use this field to define the data type to be used in the place. If necessary, click the ![Delete](/Assets/Icons/Cross02.png "[Delete]") (Delete) button to display the whole list of available data types. Enter a search text for the desired data type. The list of actions is filtered for your search text as you type. Select the ![Radio button](/Assets/Icons/Radiobutton.png "[Radio button]") (Radio button) corresponding to the appropriate option.



## Actions

![Action](/Assets/Screenshots/ActindoWorkFlow/Workflows/AddAction.png "[Action]")

Actions are the individual activities being executed in the workflow and are represented by a rectangle.

All actions contain a certain, predefined number of input and output ports, which can be mandatory or optional. For detailed information about the types of input/output ports, see [Input and output ports](#input-and-output-ports).

 When adding a new action, all compatible input and output ports are included. Mandatory input ports are already displayed and linked to a place, whereas optional ones are displayed with a ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button.

 [comment]: <> (Processes - All places linked to inputs and outputs ports must be provided with one or more pieces of data, also known as tokens, for the actions to be executed and the workflow to be completed. Otherwise, the workflow stops at the point where tokens are missing. Once an action is executed, one or more output data, or tokens, are generated, which in turn become/s input data, or tokens, for the next action. For detailed information about tokens, see...)

When clicking an action, it becomes highlighted and the corresponding element settings are displayed in the settings side bar.

![Settings side bar](/Assets/Screenshots/ActindoWorkFlow/Workflows/SettingsSideBar02.png "[Settings side bar]")

The action settings side bar is located to the right of the workspace and allows to define the action settings. The following fields are displayed:

  - (Action label and name)  
  The action label is an action identification tag and can be defined by user. The action name is a system wide predefined denomination of the activity to be performed and is read-only.

  - *Key*  
   Action key. This field is read-only. The key is required for API access and must be system wide unique.

  - *Label*  
  Action label. Click this field to edit the action label. The action label is changed both in the settings side bar and in the diagram.

  - *Queue type*  
  Click the drop-down list to select the applicable queue type. For detailed information about queue types, see [Configure the queue types](/ActindoWorkFlow/Integration/01_ConfigureQueueTypes.md).

  - *Task event*  
  Click the drop-down list to select the applicable task event.

  > [Info] This option is linked to the *Tasks* module. It is only displayed if the *Tasks* module is installed and the user has the necessary rights. The *ActindoWorkflow Process Execution Failed* task is preconfigured by default. A list of all existing task events is displayed in the *Events* menu entry of the *Tasks* module.

  - *Configuration*  
  Depending on the action, there might be configuration options, for instance, defining an email where a receipt or document must be sent. Editing the action configuration requires advanced programming knowledge.

  > [Info] Not all actions have configuration options. In this case, the *Configuration* section is not displayed.

  - *Static inputs*  
  All unlinked inputs are listed in this section. The static inputs determine the data type that can be input. They are preconfigured but can be further configured by the user clicking the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button. Only JSON values are accepted. When being edited, static inputs display a small arc without a place infront of them in the workflow diagram.

[comment]: <> (Unsure! Check Wissentransfer!)


## Input and output ports

![Input and output ports](/Assets/Screenshots/ActindoWorkFlow/Workflows/NewPlace.png "[Input and output ports]")

All actions contain a certain, predefined number of input and output ports. They are defined with a descriptive name, such as origin, data or destination.

Input ports are positioned to the left of the action and output ports are positioned to the right of the action. Both are represented by a square.

Both input and output ports can be of two types:

- **Mandatory**  
  Mandatory ports must be linked to a place, which in turn must be linked to an action. Places linked to a mandatory port cannot be deleted or removed. When adding a new action, mandatory input/output places are already displayed.

[comment]: <> (Processes - Otherwise, the workflow stops and shows an error. )

- **Optional**  
 Optional ports are displayed with a ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button next to each of them. By clicking the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button a new place is added. which can in turn be linked to a new action. For detailed information about adding new actions, see [Create an action](/ActindoWorkFlow/Operation/01_ManageWorkflows.md#create-an-action).



## Tokens

![Tokens](/Assets/Screenshots/ActindoWorkFlow/Workflows/Tokens.png "[Tokens]")

[comment]: <> (Token belongs in Processes)

A token is a piece of data needed to complete an action, for example a document.

The *Processes* menu entry displays a read-only view of any process taking place in real time and a list of all actions being executed in the selected process. For detailed information about tracking a workflow process, see [Track workflow process](/ActindoWorkFlow/Operation/02_TrackWorkflowProcess.md).

A process is started with one token at the start point, which will be input in an action to be executed. In turn, an action can output several tokens, which will become inputs for subsequent actions. It is therefore possible that a place contains several tokens, for example, several delivery notes issued for different parts of a same order. Each token will then be processed separately, that means, that the subsequent actions will be executed once for each token available.

The workflow process view displays the actions in different colours depending on their current status:

  - Ready
  - In Progress
  - Error
  - Done
  - Dead
  - Suspended
  - Aborted

[comment]: <> (Colour coding changing here too?)

For detailed information about the different status meaning, see [Link](#to-be-determined).

Next to the status of each action, a number is displayed. This number refers to the number of tokens processed in this action, and depends on the action status.  

[comment]: <> (Further info? Check Wissentransfer!)

If a token is missing at some point, for example, if a document has not been received, the action cannot be executed and the process stops at the point where data are missing. In this case, a black square is displayed on the place specifying the number of tokens waiting to be processed.

[comment]: <> (Further info needed! Check Wissentransfer!)



## Start and end point

![Start and end point](/Assets/Screenshots/ActindoWorkFlow/Workflows/Workflow.png "[Start and end point]")


A workflow must have a start and an end point, which are a special type of places. The end point is the final result of all actions executed in the workflow. A new subprocess can be linked subsequently to the end point. For detailed information about creating the start and end points, see [Create a workflow](/ActindoWorkFlow/Operation/01_ManageWorkflows.md#create-a-workflow).

[comment]: <> (Processes - A piece of data, or token, initiates the workflow at the start point and goes through all stages -places and actions- until it reaches the end point)


### Start point

The start point is the initial stage of the workflow. It is represented by a circle with an outward arc pointing towards an input port of the first action. Similarly to a place, when clicking it, the start point becomes highlighted and the corresponding element settings are displayed in the settings side bar.

![Start point](/Assets/Screenshots/ActindoWorkFlow/Workflows/StartPoint.png "[Start point]")


The start point settings side bar is located to the right of the workspace and allows to define the start point settings. The following fields are displayed:

  - *Key*  
  Start point key. This field is read-only. The key is required for API access and must be system wide unique.

  - *Data container*  
  Use this field to define the data type to be used in the start point. If necessary, click the ![Delete](/Assets/Icons/Cross02.png "[Delete]") (Delete) button to display the whole list of available data types. Enter a search text for the desired data type. The list of actions is filtered for your search text as you type. Select the ![Radio button](/Assets/Icons/Radiobutton.png "[Radio button]") (Radio button) corresponding to the appropriate option.


### End point

The end point is the final stage of the workflow. It is represented by a circle with a inward arrow coming from one or more actions being executed in the last stage(s) of the workflow. Similarly to a place, when clicking it, the start point becomes highlighted and the corresponding element settings are displayed in the settings side bar.

![End point](/Assets/Screenshots/ActindoWorkFlow/Workflows/EndPoint.png "[End point]")

The end point settings side bar is located to the right of the workspace and allows to define the end point settings. The following fields are displayed:

  - *Key*  
  End point key. This field is read-only. The key is required for API access and must be system wide unique.

  - *Data container*  
  Use this field to define the data type to be used in the end point. If necessary, click the ![Delete](/Assets/Icons/Cross02.png "[Delete]") (Delete) button to display the whole list of available data types. Enter a search text for the desired data type. The list of actions is filtered for your search text as you type. Select the ![Radio button](/Assets/Icons/Radiobutton.png "[Radio button]") (Radio button) corresponding to the appropriate option.
