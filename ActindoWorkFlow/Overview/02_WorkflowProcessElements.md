[!!Workflows](ActindoWorkFlow)

# Workflow and process elements

![Workflow](/Assets/Screenshots/ActindoWorkFlow/Workflows/Workflow.png "[Workflow]")

The *Workflows* module allows customers to model their own processes to match their companies structure. Such a workflow consists of a number of fixed elements that are chained together, each of them having specific characteristics. These elements are used to design the workflow, which can be edited as necessary according to customer needs. For detailed information, see [Manage workflows](/ActindoWorkFlow/Operation/01_ManageWorkflows.md).

A workflow runs from a fixed start point to a fixed end point, which can be in turn linked to another workflow. A workflow must contain at least one action between the start and the end point, which are a special type of places. The actions are linked through places with each other, connecting the corresponding action input and output ports. All these elements are described more in detail below.

The *Workflows* module is linked to different system modules and plugins, such as *Invoicing*, *Email*, *OmniChannels*, *Tasks*, among others. The actions available to create workflows depend on the modules installed in the system.

Since business processes, and the workflows that map them, evolve over time, workflows can be versioned. While every workflow can be uniquely identified through its key, there may be any number of versions of it. However, at a given point in time, only **one** of those versions may be published. When a process for a given workflow is to be started, that published version of the workflow is used. This allows to keep modelling a certain workflow without interrupting the daily business.


[comment]: <> (Relevante Info? This module is programmed on the basis of the Petri-Net modelling language. + kleine Erklärung? Hier oder in Overview Datei?)



## Places

![Place](/Assets/Screenshots/ActindoWorkFlow/Workflows/Place.png "[Place]")

A place is an intermediate stage in the workflow and is represented by circle, usually provided with inward and/or outward arcs.

Places serve as link between two actions, joining an output port from the previous action to the corresponding input port of the following action. Places linking mandatory input/output ports are displayed by default and cannot be deleted. Additional places can be added by clicking on the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button next to the optional input/output port. For detailed information about the types of input/output ports, see [Input and output ports](#input-and-output-ports).

A place can hold any number of tokens, including none. A token is a container carrying data, which are needed to execute a subsequent action. The place data type is always defined, more of less specifically, so it is possible to recognize the kind of data that flow through it. For detailed information, see [Tokens](#tokens).

Special types of places are the start and end point. Every workflow starts with a single place and ends with a single place. For detailed information, see [Start and end point](#start-and-end-point).


When clicking a place, it becomes highlighted and the corresponding element settings are displayed in the settings side bar.

![Settings side bar](/Assets/Screenshots/ActindoWorkFlow/Workflows/SettingsSideBar01.png "[Settings side bar]")

The place settings side bar is located to the right of the workspace and allows to define the place settings. The following fields are displayed:

  - *Key*  
  Place key. This field is read-only. The key is required for API access and must be system wide unique.

  - *Data container*  
  Use this field to define the data type to be used in the place. If necessary, click the ![Delete](/Assets/Icons/Cross02.png "[Delete]") (Delete) button to display the whole list of available data types. Enter a search text for the desired data type. The list of actions is filtered for your search text as you type. Select the ![Radio button](/Assets/Icons/Radiobutton.png "[Radio button]") (Radio button) corresponding to the appropriate option.



## Actions

![Action](/Assets/Screenshots/ActindoWorkFlow/Workflows/AddAction.png "[Action]")

Actions are the individual activities being executed in the workflow and are represented by a rectangle. Actions serve as building blocks, which are chained together through places, to configure a workflow.

All actions contain a certain, predefined number of input and output ports, at least 1 of each, which can be mandatory or optional. For detailed information about the types of input/output ports, see [Input and output ports](#input-and-output-ports). For an action to be executable, all **connected** inputs and outputs, mandatory or optional, must be fed with data.

The actions available to create workflows depend on the modules installed in the system. Every API end point of the modules automatically becomes available as an action and can be used in any workflow. However, you can also build your own actions independent from the API.

[comment]: <> (Ich finde die Benennung API endpoint etwas verwirrend hier, denn wir haben soeben über start/end point als start/end place gesprochen. Alternative Bennenung?)

It must be differentiated between a workflow action and a process action. A workflow action acts as a building block to create a workflow to model a company process, whereas a process action is the actual execution of the configured workflow action. As such, a process action can be successful or erroneous depending on its execution. If an error occurs, a process action can be retried if the underlying cause has been fixed, which results in a new process action. If multiple tokens move through the workflow, every token is processed in its own process action. As a result, any workflow action can be associated with multiple process actions, depending of the number of tokens running through it.

[commment]: <> (Evtl. kürzer/weniger Details?)

When adding a new action, all compatible input and output ports are included. Mandatory input ports are already displayed and linked to a place, whereas optional ones are displayed with a ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button.


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
  Depending on the action, there might be configuration options, for instance, defining an email where a receipt or document must be sent. Editing the action configuration may require basic programming knowledge.

  > [Info] Most actions are preconfigured and do not include configuration options. In this case, the *Configuration* section is not displayed.

  - *Static inputs*  
  All unlinked inputs are listed in this section. Static inputs can be used to configure static values for certain inputs. They can be defined by the user clicking the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button. Only valid JSON values are accepted. When edited, static inputs display a small arc without a place in front of them in the workflow diagram.

  > [Info] Normally, all tokens for the action execution are taken from the places connected to its input ports. However, static values can be configured for certain inputs. This way, if an action has configured a static input on one or more of its input ports, it will behave as if there was a place connected to that input port that always contains one token (containing whatever value is statically configured). Nevertheless, it is still necessary to have **at least one** "actual" place with an "actual" token in order to make that action executable.


## Arcs

![Arcs](/Assets/Screenshots/ActindoWorkFlow/Workflows/ArrowInput.png "[Arcs]")

The arcs are the arrows connecting a place with the input and output port(s) of a action to model the flow of information.


## Input and output ports

![Input and output ports](/Assets/Screenshots/ActindoWorkFlow/Workflows/NewPlace.png "[Input and output ports]")

All actions contain a certain, predefined number of input and output ports, at least one of each. They are defined with a descriptive name, such as origin, data or destination.

Input ports are positioned to the left of the action and output ports are positioned to the right of the action. Both are represented by a square.

Both input and output ports can be of two types:

- **Mandatory**  
  Mandatory ports must be linked to a place, which in turn must be linked to an action. Places linked to a mandatory port cannot be deleted or removed. When adding a new action, mandatory input/output places are already displayed.

- **Optional**  
 Optional ports are displayed with a ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button next to each of them. By clicking the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button a new place is added, which can in turn be linked to a new action. For detailed information about adding new actions, see [Create an action](/ActindoWorkFlow/Operation/01_ManageWorkflows.md#create-an-action).



## Tokens

![Tokens](/Assets/Screenshots/ActindoWorkFlow/Workflows/Tokens.png "[Tokens]")

[comment]: <> (Token belongs in Processes - Rename file to WorkflowProcessesElements?)

A token is a container carrying data needed to execute an action, for example a number or a document.

The *Processes* menu entry displays a read-only view of any process taking place in real time and a list of all actions being executed in the selected process. For detailed information about tracking a workflow process, see [Track workflow process](/ActindoWorkFlow/Operation/02_TrackWorkflowProcess.md).

A process is started with a single token at the start point, which will be input in an action to be executed. In turn, an action may output several tokens, which will become inputs for subsequent actions. It is therefore possible that a place contains several tokens, for example, several delivery notes issued for different parts of a same order. Each token will then be processed separately, that means, that the subsequent actions will be executed once for each token available.

[comment]: <> (Prozess wird gestartet mit einem einzigen Initialtoken - Wissentransfer ca. 0:44:45)

The workflow process view displays the actions in different colours depending on their current status:

  - *Ready*
  - *In Progress*
  - *Error*
  - *Done*
  - *Dead*
  - *Suspended*
  - *Aborted*

[comment]: <> (Colour coding changing here too?)

For detailed information about the different status meaning, see [Processes](/ActindoWorkFlow/UserInterface/03a_Processes.md).

[comment]: <> (Evtl. genaueres Link?)

Next to the status of each action, a number is displayed. This number refers to the number of tokens processed in this action, and it depends on the action status and the number of tokens received. For example, if an action displays the message *Done 1*, this means that the action has already been executed and that 1 token has been processed.

A place can also contain a black square displaying a number. This number specifies the number of tokens waiting to be processed at that place. This could happen, for example, because a token running in parallel has not been received at a particular stage of the process, but also because all tokens have been processed and are waiting for further action at the end point.

[comment]: <> (Review!)

## Start and end point

![Start and end point](/Assets/Screenshots/ActindoWorkFlow/Workflows/Workflow.png "[Start and end point]")

Every workflow starts with a single start point and ends with a single end point, which are a special type of places.

The start point can only hold one token. A token is a container carrying data, which are needed to execute a subsequent action. The place data type is always defined, more of less specifically, so it is possible to recognize the kind of data that flow through it. For detailed information, see [Tokens](#tokens).

The end point is the final result of all actions executed in the workflow and can contain any number of tokens, but at least one. A new subprocess can be linked subsequently to the end point. For detailed information about creating the start and end points, see [Create a workflow](/ActindoWorkFlow/Operation/01_ManageWorkflows.md#create-a-workflow).


### Start point

![Start point](/Assets/Screenshots/ActindoWorkFlow/Workflows/StartPoint.png "[Start point]")

The start point is the initial stage of the workflow. It is represented by a circle with an outward arc pointing towards an input port of the first action. Similarly to a place, when clicking it, the start point becomes highlighted and the corresponding element settings are displayed in the settings side bar.

The start point settings side bar is located to the right of the workspace and allows to define the start point settings. The following fields are displayed:

  - *Key*  
  Start point key. This field is read-only. The key is required for API access and must be system wide unique.

  - *Data container*  
  Use this field to define the data type to be used in the start point. If necessary, click the ![Delete](/Assets/Icons/Cross02.png "[Delete]") (Delete) button to display the whole list of available data types. Enter a search text for the desired data type. The list of actions is filtered for your search text as you type. Select the ![Radio button](/Assets/Icons/Radiobutton.png "[Radio button]") (Radio button) corresponding to the appropriate option.


### End point

![End point](/Assets/Screenshots/ActindoWorkFlow/Workflows/EndPoint.png "[End point]")

The end point is the final stage of the workflow. It is represented by a circle with a inward arrow coming from one or more actions being executed in the last stage(s) of the workflow. Similarly to a place, when clicking it, the start point becomes highlighted and the corresponding element settings are displayed in the settings side bar.

The end point settings side bar is located to the right of the workspace and allows to define the end point settings. The following fields are displayed:

  - *Key*  
  End point key. This field is read-only. The key is required for API access and must be system wide unique.

  - *Data container*  
  Use this field to define the data type to be used in the end point. If necessary, click the ![Delete](/Assets/Icons/Cross02.png "[Delete]") (Delete) button to display the whole list of available data types. Enter a search text for the desired data type. The list of actions is filtered for your search text as you type. Select the ![Radio button](/Assets/Icons/Radiobutton.png "[Radio button]") (Radio button) corresponding to the appropriate option.