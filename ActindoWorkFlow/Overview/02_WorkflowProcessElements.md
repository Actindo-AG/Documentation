[!!Workflows](ActindoWorkFlow)

# Workflow and process elements

![Workflow](/Assets/Screenshots/ActindoWorkFlow/Workflows/Workflow.png "[Workflow]")

The *Workflows* module allows customers to model their own processes to match their companies structure. Such a workflow consists of a number of fixed elements that are chained together, each of them having specific characteristics. These elements are used to design the workflow, which can be edited as necessary according to customer needs. For detailed information, see [Manage workflows](/ActindoWorkFlow/Operation/01_ManageWorkflows.md).

A workflow runs from a fixed start place to a fixed end place, which can be in turn linked to another workflow. A workflow must contain at least one transition between the start and the end place, which are a special type of places. The transitions are linked through places with each other, connecting the corresponding transition input and output ports. All these elements are described more in detail below.

The *Workflows* module is linked to different system modules and plugins, such as *Invoicing*, *Email*, *OmniChannels*, *Tasks*, among others. The transitions available to create workflows depend on the modules installed in the system.

Since business processes, and the workflows that map them, evolve over time, workflows can be versioned. While every workflow can be uniquely identified through its key, there may be any number of versions of it. However, at a given point in time, only one of those versions may be published. When a process for a given workflow is to be started, that published version of the workflow is used. This allows to keep modelling a certain workflow without interrupting the daily business.



## Transitions

![Transition](/Assets/Screenshots/ActindoWorkFlow/Workflows/Action.png "[Transition]")

The transitions act as building blocks that are chained together through places to configure a workflow. They are represented by a rectangle.

All transitions contain a certain, predefined number of input and output ports, at least 1 of each, which can be mandatory or optional. For detailed information about the types of input/output ports, see [Input and output ports](#input-and-output-ports). For a transition to be executable in a workflow process, all connected inputs and outputs, mandatory or optional, must be fed with data.

The transitions available to create workflows depend on the modules installed in the system. Every API end point of the modules automatically becomes available as a transition and can be used in any workflow. However, you can also build your own transitions independent from the API. Some transition may have configuration options, but most of them do not.

When a transition is executed in a workflow process, it is called action or process action, that is, an action is the actual execution of a configured transition. As a result, one transition may be associated with multiple process actions. For detailed information, see [Actions](#actions).


When adding a new transition, places for mandatory input ports are automatically inserted, whereas optional input ports are displayed with a ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button.


When clicking a transition, it becomes highlighted and the corresponding element settings are displayed in the settings side bar.

![Settings side bar](/Assets/Screenshots/ActindoWorkFlow/Workflows/SettingsSideBar02.png "[Settings side bar]")

The transition settings side bar is located to the right of the workspace and allows to define the transition settings. The following fields are displayed:


- *Key*  
Action key. This field is read-only. The key is required for API access and must be unique within the workflow version.

- *Label*  
Action label defined by the user. It can be used to specify or simplify the transition name. When editing the transition label, it is changed both at the top of the settings side bar and in the action rectangle in the diagram.

- *Queue type*  
Click the drop-down list to select the applicable queue type. For detailed information about queue types, see [Configure the queue types](/ActindoWorkFlow/Integration/01_ConfigureQueueTypes.md).

- *Task event*  
Click the drop-down list and select the applicable task event. All available task events are displayed. This option is linked to the *Tasks* module. The drop-down list is only displayed if the *Tasks* module is installed and the user has the necessary rights.

 > [Info] The *ActindoWorkflow Process Execution Failed* task is preconfigured by default. A list of all existing task events is displayed in the *Events* menu entry of the *Tasks* module.

- *Configuration*  
Depending on the transition, there might be configuration options, for instance, defining an email where a receipt or document must be sent. Editing the transition configuration may require basic programming knowledge.

  > [Info] Most transitions are preconfigured and do not include configuration options. In this case, the *Configuration* section is not displayed.

- *Static inputs*  
All unlinked input ports are listed in this section. Static inputs can be used to configure static values for certain inputs. They can be defined by the user clicking the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button. Only valid JSON values are accepted. When used, static inputs are displayed by a small arrow in front of the input ports in the workflow diagram. This section is only displayed, if the selected transition has at least one unlinked input port.

  > [Info] Normally, all tokens for the transition execution, that is an action, are taken from the places connected to its input ports. However, static values can be configured for certain inputs. This way, if a transition has configured a static input on one or more of its input ports, it will behave as if there was a place connected to that input port that always contains one token (containing whatever value is statically configured). Nevertheless, it is still necessary to have at least one "actual" place with an "actual" token in order to make that transition executable.



## Places

![Place](/Assets/Screenshots/ActindoWorkFlow/Workflows/Place.png "[Place]")

A place is an intermediate stage in the workflow and is represented by a circle, usually provided with incoming and/or outcoming arcs.

Places serve as link between two transitions, joining an output port from the previous transition to the corresponding input port of the following transition. Places linking mandatory input/output ports are displayed by default and cannot be deleted. Additional places can be added by clicking on the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button next to the optional input/output port. For detailed information about the types of input/output ports, see [Input and output ports](#input-and-output-ports). All places included in a process must be linked to input/output ports. Otherwise, the process cannot be initiated (an error is displayed in the workflow editor).

A place can hold any number of tokens, including none. A token is a container carrying data, which is needed to execute a subsequent action. The place data type is always defined, more or less specifically, so it is possible to recognize the kind of data that flows through it. For detailed information, see [Tokens](#tokens).

Special types of places are the start and end place. Every workflow starts with a single place and ends with a single place. For detailed information, see [Start and end place](#start-and-end-place).


When clicking a place, it becomes highlighted and the corresponding element settings are displayed in the settings side bar.

![Settings side bar](/Assets/Screenshots/ActindoWorkFlow/Workflows/SettingsSideBar01.png "[Settings side bar]")

The place settings side bar is located to the right of the workspace and allows to define the place settings. The following fields are displayed:

  - *Key*  
  Place key. This field is read-only. The key is required for API access and must be unique within the workflow version.

  - *Data container*  
  Use this field to define the data type to be used in the place. If necessary, click the ![Delete](/Assets/Icons/Cross02.png "[Delete]") (Delete) button to display the whole list of available data types. Enter a search text for the desired data type. The list of actions is filtered for your search text as you type. Select the ![Radio button](/Assets/Icons/Radiobutton.png "[Radio button]") (Radio button) corresponding to the appropriate option.


## Arcs

![Arcs](/Assets/Screenshots/ActindoWorkFlow/Workflows/ArrowInput.png "[Arcs]")

The arcs are the links connecting a place with the input and output port(s) of a transition to model the flow of information. The arcs are represented by arrows. Arcs connecting a place to an input port are called *incoming arcs*, arc connecting an output port to a place are called *outcoming arcs*.


## Input and output ports

![Input and output ports](/Assets/Screenshots/ActindoWorkFlow/Workflows/NewPlace.png "[Input and output ports]")

All transitions contain a certain, predefined number of input and output ports, at least one of each. They are defined with a descriptive name, such as origin, data or destination.

Input ports are positioned to the left of the transition and output ports are positioned to the right of the transition. Both are represented by a square.

Both, input and output ports, can be of two types:

- **Mandatory**  
  Mandatory ports must be linked to a place, which in turn must be linked to a transition. Places linked to a mandatory port cannot be deleted or removed. When adding a new transition, all places linked to a mandatory input/output are already displayed.

- **Optional**  
 Optional ports are displayed with a ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button next to each of them. By clicking the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button a new place is added, which can in turn be linked to a new transition. For detailed information about adding new actions, see [Create an action](/ActindoWorkFlow/Operation/01_ManageWorkflows.md#create-an-action).



## Actions

![Action](/Assets/Screenshots/ActindoWorkFlow/Workflows/AddAction.png "[Action]")

Actions, or process actions, are the individual activities being executed in the workflow process and are represented by a rectangle.

A process action is the actual execution of a transition  configured in a workflow. As such, a process action can be successful or faulty depending on its execution. If an error occurs, a process action can be retried if the underlying cause has been fixed, which results in a re-execution of the process action. Moreover, if multiple tokens move through the workflow, every token is processed in its own process action. As a result, a transition can be associated with multiple process actions, depending of the number of tokens running through it.



## Tokens

![Tokens](/Assets/Screenshots/ActindoWorkFlow/Workflows/Tokens.png "[Tokens]")


A token is a container carrying data needed to execute an action, for example a number or a document.

The *Processes* menu entry displays a diagram of any process taking place in real time and a list of all actions being executed in the selected process. For detailed information about tracking a workflow process, see [Track workflow process](/ActindoWorkFlow/Operation/02_TrackWorkflowProcess.md).

A process is started with a single token at the start place, which will be input in an action to be executed. In turn, an action may output several tokens, which will become inputs for subsequent actions. It is therefore possible that a place contains several tokens, for example, several delivery notes issued for different parts of a same order. Each token will then be processed separately, that means, that the subsequent actions will be executed once for each token available.


The workflow process view displays the actions in different colors depending on their current status:

  - *Ready*
  - *In Progress*
  - *Error*
  - *Done*
  - *Dead*
  - *Suspended*
  - *Aborted*

For detailed information about the process actions, see [Process actions](/ActindoWorkFlow/UserInterface/04a_ProcessActions.md).

Next to the status of each action, a number is displayed. This number refers to the number of tokens processed in this action, and it depends on the action status and the number of tokens received. For example, if an action displays the message *Done 1*, this means that the action has already been executed and that 1 token has been processed.

A place can also contain a black square displaying a number. This number specifies the number of tokens waiting to be processed at that place. This could happen, for example, because a token running in parallel has not been received at a particular stage of the process, but also because all tokens have been processed and are waiting for further action at the end place.


## Start and end place

![Start and end place](/Assets/Screenshots/ActindoWorkFlow/Workflows/Workflow.png "[Start and end place]")

Every workflow starts with a single start place and ends with a single end place, which are a special type of places.

The start place can only hold one token. A token is a container carrying data, which is needed to execute a subsequent action. The place data type is always defined, more or less specifically, so it is possible to recognize the kind of data that flows through it. For detailed information, see [Tokens](#tokens).

The end place is the final result of all actions executed in the workflow and can contain any number of tokens, but at least one. A process is marked as *Done* when all tokens have reached the end place. For detailed information about creating the start and end places, see [Create a workflow](/ActindoWorkFlow/Operation/01_ManageWorkflows.md#create-a-workflow).


### Start place

![Start place](/Assets/Screenshots/ActindoWorkFlow/Workflows/StartPlace.png "[Start place]")

The start place is the initial stage of the workflow. It is represented by a circle with an incoming arc pointing towards an input port of the first action. Similarly to a place, when clicking it, the start place becomes highlighted and the corresponding element settings are displayed in the settings side bar.

The start place settings side bar is located to the right of the workspace and allows to define the start place settings. The following fields are displayed:

  - *Key*  
  Start place key. This field is read-only. The key is required for API access and must be unique within the workflow version.

  - *Data container*  
  Use this field to define the data type to be used in the start place. If necessary, click the ![Delete](/Assets/Icons/Cross02.png "[Delete]") (Delete) button to display the whole list of available data types. Enter a search text for the desired data type. The list of actions is filtered for your search text as you type. Select the ![Radio button](/Assets/Icons/Radiobutton.png "[Radio button]") (Radio button) corresponding to the appropriate option.


### End place

![End place](/Assets/Screenshots/ActindoWorkFlow/Workflows/EndPlace.png "[End place]")

The end place is the final stage of the workflow. It is represented by a circle with an outcoming arrow coming from one or more actions being executed in the last stage(s) of the workflow. Similarly to a place, when clicking it, the end place becomes highlighted and the corresponding element settings are displayed in the settings side bar.

The end place settings side bar is located to the right of the workspace and allows to define the end place settings. The following fields are displayed:

  - *Key*  
  End place key. This field is read-only. The key is required for API access and must be unique within the workflow version.

  - *Data container*  
  Use this field to define the data type to be used in the end place. If necessary, click the ![Delete](/Assets/Icons/Cross02.png "[Delete]") (Delete) button to display the whole list of available data types. Enter a search text for the desired data type. The list of actions is filtered for your search text as you type. Select the ![Radio button](/Assets/Icons/Radiobutton.png "[Radio button]") (Radio button) corresponding to the appropriate option.
