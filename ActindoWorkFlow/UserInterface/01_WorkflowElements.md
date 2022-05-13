[!!Workflows](ActindoWorkFlow)

# Workflow elements

*Workflows > Menu entry Workflows > Tab OVERVIEW > Select workflow > Select workflow version*

![Workflow](/Assets/Screenshots/ActindoWorkFlow/Workflows/Workflow.png "[Workflow]")

A workflow is represented with a number of fixed elements, each of them having specific characteristics. These elements are used to design the workflow, which
can be edited as necessary according to customer needs. For detailed information, see [Manage workflows](#01_ManageWorkflows.md).

A workflow runs from left to right, from a start point to an end point, which can be in turn linked to another workflow. The data input at the start point, for example a document, goes through the different workflow stages (places and actions) until it reaches the end point. The process is than completed.

> [Info] Data is provided from different system modules and plugins, such as *Invoicing*, *Email*, *OmniChannels*, *Tasks*, among others. The actions available to create workflows depend on the modules installed in the system.


## Places

![Place](/Assets/Screenshots/ActindoWorkFlow/Workflows/Place.png "[Place]")

A place is a step in the workflow and is represented by circle, usually with inward and outward arrows.

Places serve as link between actions, joining an output port from the previous action to the corresponding input port of the following action. Places linking mandatory input/output ports are displayed per default and cannot be deleted. Additional places can be added by clicking on the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button next to the optional input/output port. For detailed information about the types of input/output ports, see [Input and output ports](#input-and-output-port).

When clicking a place, it becomes highlighted and the corresponding element settings are displayed in the settings side bar.

![Settings side bar](/Assets/Screenshots/ActindoWorkFlow/Workflows/SettingsSideBar01.png "[Settings side bar]")

The place settings side bar is located to the right of the workspace and displays the following information:

  - *Key*  
  Element key. This information is read-only.

  - *Data container*  
  Use this field to define the data type to be used in the place.

    - ![Search](/Assets/Icons/Search.png "[Search]") (Search)  
  Enter a search text in the search bar. The data type list is filtered according to the search text entered.

    - ![Delete](/Assets/Icons/Cross02.png "[Delete]") (Delete)  
  Click this element to clear the data displayed in the search bar. A list of all available data types is displayed.

    - ![Radio button](/Assets/Icons/Radiobutton.png "[Radio button]") (Radio button)  
  Select the radio button corresponding to the appropriate option.


## Actions

![Action](/Assets/Screenshots/ActindoWorkFlow/Workflows/AddAction.png "[Action]")

Actions, also known as transitions, are the individual tasks being executed in the workflow and are represented by a rectangle.

Actions can contain any number of input and output ports, which can be mandatory or optional. For detailed information about the types of input/output ports, see [Input and output ports](#input-and-output-ports).

 When adding a new action, all compatible input and output ports are included. Mandatory input ports are already displayed and linked to a place, whereas optional ones are displayed with a ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button.

 All places linked to inputs and outputs ports must be provided with one or more pieces of data, also known as tokens, for the actions to be executed and the workflow to be completed. Otherwise, the workflow stops at the point where tokens are missing. Once an action is executed, one or more output data (tokens) are generated, which in turn become(s) input data (tokens) for the next action. For detailed information about tokens, see [Tokens](#to-be-determined).

When clicking an action, it becomes highlighted and the corresponding element settings are displayed in the settings side bar.

![Settings side bar](/Assets/Screenshots/ActindoWorkFlow/Workflows/SettingsSideBar02.png "[Settings side bar]")

The settings side bar is located to the right of the workspace and displays the following information:

  - (Action label and name)  
  The action label can be changed in the *Label* entry field. The action name provides a detailed description of the task to be performed and is read-only.

  - *Key*  
   Element key. This information is read-only.

  - *Label*  
  Action label. Click this field to edit the action label. The action label is changed both in the settings side bar and in the diagram.

  - *Queue type*  
  Click the drop-down list to select the applicable queue type. For detailed information about queue types, see [Configure the queue types](#to-be-completed).

  - *Task event*  
  Click the drop-down list to select the applicable task event.

  > [Info] This option is linked to the *Tasks* module. It is only displayed if the *Tasks* module is installed and the user has the necessary rights. The *ActindoWorkflow Process Execution Failed* task is preconfigured per default. A list of all existing task events is displayed in the *Events* menu entry of the *Tasks* module.

  - *Configuration*  
  Depending on the action, there might be configuration options, for instance, defining an email where a receipt or document must be sent. Editing the action configuration requires advanced programming knowledge.

  > [Info] Not all actions have configuration options. In this case, the *Configuration* field is not displayed.

  - *Static inputs*  
  The optional inputs are displayed. They can be edited by clicking the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button.

[comment]: <> (The static inputs determine the data type that can be input. They are preconfigured but can be further configured by the user. Only JSON values are accepted.)


## Input and output ports

![Input and output ports](/Assets/Screenshots/ActindoWorkFlow/Workflows/InputOutputPorts.png "[Input and output ports]")

Every action can contain any number of input and output ports. They can be defined with a descriptive name, such as reporter, title or event, or be simply marked as *in* (input) and *out* (output) followed by a consecutive number.

[comment]: <> (The plan is to provide all input and output ports with a name)

Input ports are positioned to the left of the action and output ports are positioned to the right of the action. Both are represented by a square.

Both input and output ports can be of two types:

- **Mandatory**  
  Mandatory ports must be linked to a place, which in turn must be linked to an action. Otherwise, the workflow stops and shows an error. Places linked to a mandatory port cannot be deleted or removed. When adding a new action, mandatory input/output places are already displayed.

- **Optional**  
 Optional ports are displayed with a ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button next to each of them. By clicking the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button a new action can be added. For detailed information about adding new actions, see [Link](#to-be-completed).


## Tokens

![Tokens](/Assets/Screenshots/ActindoWorkFlow/Workflows/Tokens.png "[Tokens]")

[comment]: <> (Token belongs in Processes)

A token is a piece of data needed to complete an action, for example a document.

The *Processes* menu entry displays a read-only view of any process taking place in real time and a list of all actions being executed in the selected process. For detailed information about tracking a workflow process, see [Link](#to-be-completed).

A process is started with one token at the start point, which will be processed in each action executed and, if necessary, turned into several tokens. It is therefore possible that a place contains several tokens, for example, several delivery notes issued for different parts of a same order. Each token will then be processed separately, that means, that the subsequent actions will be executed once for each token available.

The workflow process view displays the actions in different colours depending on their current status:

  - Green: done
  - Blue: active
  - White: waiting
  - Red: error

[comment]: <> (Colour coding changing here too?)

Next to the status of each action, a number is displayed. This number refers to the number of tokens processed in this action.  

If a token is missing at some point, for example, if a document has not been received, the action cannot be executed and the process stops at the point where data are missing. In this case, a black square is displayed on the place specifying the number of tokens waiting to be processed.

The tokens can also be displayed in a column view in the *Tokens* tab and filtered according to their status:  

  - Done (green)
  - Being processed (blue)
  - Ready (grey)
  - Error (red)

[comment]: <> (Colour coding changing here too?)


For detailed information, see [Link](#to-be-determined).


## Start and end point

![Start and end point](/Assets/Screenshots/ActindoWorkFlow/Workflows/Workflow.png "[Start and end point]")


A workflow must have a start and an end point. A piece of data, or token, initiates the workflow at the start point and goes through all stages (places and actions) until it reaches the end point. The end point is the final result of all actions executed in the workflow. A new (sub)process can be linked subsequently to the end point. for detailed information, see [Link].


### Start point

The start point is the initial stage of the workflow. It is represented by a circle with an outward arrow pointing towards an input port of the first action. Similarly to a place, when clicking it, the start point becomes highlighted and the corresponding element settings are displayed in the settings side bar.

![Start point](/Assets/Screenshots/ActindoWorkFlow/Workflows/StartPoint.png "[Start point]")

The settings side bar is located to the right of the workspace and displays the following information:

  - *Key*  
  Element key. This information is read-only.

  - *Data container*  
  Use this field to define the data type contained to be used in the place.

    - ![Search](/Assets/Icons/Search.png "[Search]") (Search)  
  Enter a search text in the search bar. The data type list is filtered according to the search text entered.

    - ![Delete](/Assets/Icons/Cross02.png "[Delete]") (Delete)  
  Click this element to clear the data displayed in the search bar. A list of all available data types is displayed.

    - ![Radio button](/Assets/Icons/Radiobutton.png "[Radio button]") (Radio button)  
  Select the radio button corresponding to the appropriate option.


### End point

The end point is the final stage of the workflow. It is represented by a circle with a inward arrow coming from one or more actions being executed in the last stage(s) of the workflow. Similarly to a place, when clicking it, the start point becomes highlighted and the corresponding element settings are displayed in the settings side bar.

![End point](/Assets/Screenshots/ActindoWorkFlow/Workflows/EndPoint.png "[End point]")

The settings side bar is located to the right of the workspace and displays the following information:

  - *Key*  
  Element key. This information is read-only.

  - *Data container*  
  Use this field to define the data type contained to be used in the place.

    - ![Search](/Assets/Icons/Search.png "[Search]") (Search)  
  Enter a search text in the search bar. The data type list is filtered according to the search text entered.

    - ![Delete](/Assets/Icons/Cross02.png "[Delete]") (Delete)  
  Click this element to clear the data displayed in the search bar. A list of all available data types is displayed.

    - ![Radio button](/Assets/Icons/Radiobutton.png "[Radio button]") (Radio button)  
  Select the radio button corresponding to the appropriate option.
