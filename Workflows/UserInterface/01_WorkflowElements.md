[!!Workflows](Workflows)

# Workflow elements

*Workflows > Menu entry Workflows > Tab OVERVIEW > Select workflow > Select workflow version*

![Workflow](/Assets/Screenshots/Workflows/Workflows/Workflow.png "[Workflow]")

A workflow is represented with a number of fixed elements, each of them having specific characteristics. These elements are used to design the workflow, which
can be edited as necessary according to customer needs. For detailed information, see [Manage workflows](#01_ManageWorkflows.md).

A workflow runs from left to right, from a start point to an end point, which can be in turn linked to another workflow. The data input in the start point, for example a document, goes through the different workflow stages (places and actions) until it reaches the end point. The process is than completed.

> [Info] Data is provided from different system modules and plug-ins, such as Invoicing, Email, OmniChannels, Tasks, etc. The actions available to create workflows depend on the modules installed in the system.


## Places

[comment]: <> (Add screenshot section)

A place, also known as node, is a step in the workflow and is represented with the ![Place](/Assets/Icons/Place.png "[Place]") (Place) icon. When clicking it, it becomes highlighted and turns light green. The place data are displayed in the settings side bar.

[comment]: <> (Data type / Daten-Container in settings side bar?)

Places are the link between actions, joining an output port from the previous action to the corresponding input port of the following action. Places linking mandatory input/output ports are displayed per default and cannot be deleted. Additional places can be added by clicking on the ![Plus](/Assets/Icons/PLus01.png "[Plus]") (Plus) icon next to the optional input/output port. For detailed information about the types of input/output ports, see [Input and output ports](#input-and-output-port).


![Settings side bar](/Assets/Screenshots/Workflows/Workflows/SettingsSideBar01.png "[Settings side bar]")

The settings side bar is located to the right of the settings side bar and displays the following information:

  - *Key*  
  Element key. This information is read-only.

  - *Data container*  

  [comment]: <> (Where data type are specified? If data type available/contained in place, action list only displays compatible actions. When adding a new action with + sign, new compatible action is linked automatically. anyValue per default? Is it possible to enter a value or is it already defined, that is, data type?)

  - ![Search](/Assets/Icons/Search.png "[Search]") (Search)  
  Enter any value to be searched in the search bar.  

  - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross)  
  Click this icon to display all available data containers.

  - ![Radio button](/Assets/Icons/Radiobutton.png "[Radio button]") (Radio button)  
  Select the radio button corresponding to the appropriate option.

Once an action is executed, one or more outputs are generated, which in turn become(s) input for the next action. Places linked to mandatory output ports cannot be left hanging, otherwise workflow displays error and stops.


## Actions

[comment]: <> (Add screenshot section)

Actions, also known as transitions, are the individual tasks being executed in the workflow and are represented with the ![Action](/Assets/Icons/Action.png "[Action]") icon. When clicking it, it becomes highlighted and turns light green. The action data are displayed in the settings side bar.

Actions can contain any number of input and output ports, which can be mandatory or optional. For detailed information about the types of input/output ports, see [Input and output ports](#input-and-output-ports).

 When adding a new action, all compatible input and output ports are included. Mandatory input ports are already displayed and linked to the new actions, whereas optional ones are displayed with a ![Plus](/Assets/Icons/PLus01.png "[Plus]") (Plus) icon. All places linked to (mandatory) inputs and outputs ports must contain data for the actions to work and the workflow to be completed. Otherwise, the workflow stops at the point where data are missing.

[comment]: <> (Where are the data? Ports or places? If an optional port is linked but no data available, does the process stop too? I guess yes?)


![Settings side bar](/Assets/Screenshots/Workflows/Workflows/SettingsSideBar02.png "[Settings side bar]")

The settings side bar is located to the right of the workspace and displays the following information:

  - (Action name and description)  
  The action name can changed in the *Label* entry field. The action description explains the task to be performed.

  [comment]: <> (Coding under the action name supposed to be left like that? Add information for user?)  

  - *Key*  
   Element key. This information is read-only.

  - *Label*  
  Action name. This information is editable. If the label is edited, the action name is changed, both in the settings side bar and in the diagram.

  - *Queue type*  
  Click the drop-down list to select the applicable queue type. For detailed information about queue types, see [Configure the queue types](#to-be-completed).

  - *Task event*  
  Click the drop-down list to select the applicable task event.

[comment]: <> (What is a task event? What do the different options mean?)

  - *Configuration*  
  Depending on the action, there might be configuration options, for instance, defining an email where a receipt or document must be sent. This information is editable and requires programming advanced knowledge.

  > [Info] Not all actions can be configured/have a configuration option. In this case, this option is not displayed.

  - *Static inputs*  ![Plus](/Assets/Icons/PLus01.png "[Plus]")  
  The optional inputs are displayed. They can be edited by clicking the ![Plus](/Assets/Icons/PLus01.png "[Plus]") (Plus) icon.

[comment]: <> (What can you do with them?)


## Input and output ports

[comment]: <> (Add screenshot section)

Every action can contain any number of input and output ports. They can be defined with a descriptive name, such as reporter, title or event, or be simply marked as in (input) and out (output) followed by a consecutive number.

[comment]: <> (Why? Is there are reason? Can the port name be edited? Maybe in "statische Inputs"? If yes, what about outputs?)

- ![Input port](/Assets/Icons/InputPort.png "[Input port]")  
  Input ports are positioned to the left of the action and represented by a blue square icon.

- ![Output port](/Assets/Icons/OutputPort.png "[Output port]")  
  Input ports are positioned to the right of the action and represented by a blue square.

[comment]: <> (Change layout!)

Both input and output ports can be of two types:

- **Mandatory**  
  Mandatory ports must be linked to a place, which in turn must be linked to an action. Otherwise, the workflow stops and shows an error. Places linked to a mandatory port cannot be deleted or removed. When adding a new action, mandatory input/output places are already displayed and linked to the new action.

- **Optional**  
 Optional ports are displayed with a ![Plus](/Assets/Icons/PLus01.png "[Plus]") (Plus) icon next to each of them. By clicking the ![Plus](/Assets/Icons/PLus01.png "[Plus]") (Plus) icon a new action can be added. For detailed information about adding new actions, see [Link](#to-be-completed).

[comment]: <> (Unclear: difference port vs. place!)


## Tokens

[comment]: <> (Add screenshot section)

A token is any piece of data needed to complete an action, for example a document.

The *Processes* menu entry displays a read-only view of any process taking place in real time and a list of all actions being executed in the selected process. For detailed information about tracking a workflow process, see [Link](#to-be-completed).

A process is started with one token at start point, which will be processed in each action executed and, if necessary, turned into several tokens. It is therefore possible that a place contains several tokens, for instance several delivery notes issued for different parts of a same order. Each token will then be processed separately, that means, that the subsequent actions will be executed once for each token available.

The workflow process view displays the actions in different colours depending on their current status:

  - Green: done
  - Blue: active
  - White: waiting
  - Red: error

Next to the status of each action, a number is displayed. This number refers to the number of tokens processed in this action.  

If a token is missing, for example, if a document has not been issued, the action cannot be executed and the process stops at the point where data are missing. In this case, a black square is displayed on the place specifying the number of tokens missing at this point.

[comment]: <> (unsure, check!!! Number of tokens missing, available, processed?)


The tokens can also be displayed in a column view in the *Tokens* tab and filtered according to their status:  

  - Green: done
  - Blue: active
  - Red: error

  [comment]: <> (Check!)


For detailed information, see [Link](#to-be-determined). 



## Start and end point

[comment]: <> (Add screenshot section)

![Start point](/Assets/Icons/StartPoint.png "[Start point]")

![End point](/Assets/Icons/EndPoint.png "[End point]")

A workflow must have a start and an end point. A new (sub)process can be linked subsequently to the end point (Workflow editor > [ADD ACTION] > Start Subprocess).
