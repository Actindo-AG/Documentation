[!!Workflows](ActindoWorkFlow)

# Track the workflow process

A process is an instance of a workflow. When a transaction is performed, a piece of data is generated, for example an invoice, which in turn initiates a workflow process. Therefore, for every single transaction performed, an individual instance of the corresponding workflow, that is, a process, is initiated.

A process has a start and an end point, as well as different stages (places and actions) which the initial data goes through in order to be processed. For a detailed description of the workflow elements, see [Workflow elements](/ActindoWorkFlow/UserInterface/01_WorkflowElements.md).

The workflow process can be tracked to check the status of a whole process or of individual actions, as well as the status and content of a token.


## Check the process status

The process status can be checked to see how far a process has progressed, detect potential problems, and solve any problems that may occur as a result of a misconfiguration or any other external issues, so that the process can continue running.

The *OVERVIEW* tab in the *Processes* menu entry displays a list of all processes that are currently being executed or have been executed in the system. Per default, all existing processes are displayed but can also be filtered according to different criteria.


### Prerequisites

- A workflow is created, see [Create a workflow](01_ManageWorkflows.md#create-a-workflow).
- A workflow process has been initiated, see [Link](#to-be-determined).

### Procedure

*Workflows > Processes > Tab OVERVIEW*

![Processes](/Assets/Screenshots/ActindoWorkFlow/Workflows/Processes.png "[Processes]")


1. Click *Status* drop-down list and select **All** to display all processes.  
All processes, regardless of their status, are displayed.

2. Click the *Workflow* drop-down list and select the specific workflow type to be displayed.  
All processes of the selected workflow type are displayed.

3. Check the list displayed for process to be checked.  
The current process status can be checked in the *Status* column.

  > [Info] Processes can also be filtered with the filter options. Click the ![Filter](/Assets/Icons/Filter.png "[Filter]") (Filter) button to display the filter options. For detailed information, see [Link](#to-be-completed).

4. Click a process in the list to select it and display individual process actions and tokens.  
A read-only diagram of the process including all individual places and actions is displayed. For detailed information about individual process actions, see [Check the process action status](#check-the-process-action-status). For detailed information about tokens, see [Check the token status and content](#check-the-token-status-and-content).


### Next steps

- [Check the process action status](#check-the-process-action-status)
- [Check the token status and content](#check-the-token-status-and-content)

### See also

- [Troubleshooting](#to-be-determined)


## Check the process action status

The process status can be checked to see which actions have already executed and where problems may occur.

After selecting a process, the *OVERVIEW* tab displays a read-only diagram of the selected process including all places and actions. If the process is currently active, the process execution can be observed in real time.

The workflow process diagram displays the actions in different colours depending on their current status:

  - Done (green)
  - Active (blue)
  - Waiting (white)
  - Error (red)
  - Dead (black)

  [comment]: <> (Check possible statuses and colours?)

Per default, the *Actions* tab listing all existing actions in the selected process is displayed. The actions are displayed in column view providing further details apart from the status.

### Prerequisites

- A workflow is created, see [Create a workflow](01_ManageWorkflows.md#create-a-workflow).
- A workflow process has been initiated, see [Link](#to-be-determined).

### Procedure

*Workflows > Processes > Tab OVERVIEW > Select process*

[comment]: <> (Specify Tab Actions?)

![Process actions](/Assets/Screenshots/ActindoWorkFlow/Workflows/ProcessActions.png "[Process actions]")

[comments]: <> (Check one action or several actions at a time? See Troubleshooting)

1. tab actions wählen

2. filter nach status auf all (ich will erstmal alle actions anzeigen)

3. actions in diagramm anschauen (status farben erklären)

4. action in diagramm auswählen (je nach status wird action in tab angezeigt)

5. status und weitere infos zu action in tab actions anschauen (spalten erklären: status, tries, max tries, queue type, defer until)

6. hinweis auf troubleshooting bei error, verweis auf tokens

7. ggf. logs einschließen -> mit oli klären (vielleicht auch nur in troubleshooting oder in separatem kapitel)

-> beschreiben, wie man alternativ die actions im menüpunkt Process actions anzeigen kann (und von dort aus zu den prozessen gelangt)


1. Click the action in the process diagram to be checked.  
The selected action is displayed in the *Actions* tab.

2. Alternatively, click *Status* drop-down list to filter the processes according to their status.   
All existing actions with the selected status are displayed.

  The following statuses are displayed:

  - **All**  
  All existing actions are displayed. This option is displayed per default.

  - **Active**  
  The actions that are currently running are displayed.

  - **Done**  
  The actions that are finished are displayed.

  - **Error**  
  The actions that have produced an error are displayed.

  - **Error; automatic retry**  
  The actions that have produced an error but are set up for automatic retry are displayed. For detailed information about action settings, see [Link](#to-be-completed).

  - **Suspended**

  - **Process aborted**

  > [Info] Actions can also be filtered with the filter options. Click the ![Filter](/Assets/Icons/Filter.png "[Filter]") (Filter) button to display the filter options.

[comment]: <> (Oli: Statuses Error; automatic retry, Suspended and Process aborted. Wo stellt man "automatic retry" ein?)

3. Check the current action status in the *Status* column.  

  > [Info] Further information about the selected action(s) can be found in the *Logs* tab.

4. Check the number of times an action has been tried in the *Tries* column.

5. Check the number of times an action must be retried after error in the *Maximal retries after error* column.

[comment]: <> (Useful for user to mention those options? Is it possible to configure it somehow?)

6. Check the queue type in the *Queue type* column.  
The *Default* queue type is normally selected. For detailed information about configuring queue types, see [Configure the queue types](#to-be-competed).

  > [Info] A different queue type can be selected by editing an action, see [Edit an action](01_ManageWorkflows.md#edit-an-action).

7. Check the next point in time when the action is being tried in the *Defer until* column.

[comment]: <> (Useful for user to mention it? Is it possible to configure it somehow?)


---
[comment]: <> (Further info probably only for Troubleshooting)


- If an error is displayed, take the necessary action to solve the problem before retrying the action.

  > [Info] Further information about the error displayed can be found in the *Logs* tab.

- Click the checkbox to select the action to be checked.    
The (editing) toolbar is displayed.

  > [Info] If several action have been filtered according to status, it is also possible to select them all simultaneously. Click the checkbox in the column header to select all actions filtered. For detailed information about this process, see [Retry a process action](#to-be-completed).

- Click the [RETRY] button to execute the action again.



### Next steps

- [Check the token status and content](#check-the-token-status-and-content)

### See also

- [Troubleshooting](#to-be-determined)

## Check the token status and content

The *Tokens* tab displays the tokens that are being or have been processed. A token is a piece of data needed to complete an action, for example a document. When a transaction is performed, a token is generated, for instance an invoice, which in turn initiates the workflow process.

A process is started with one token at the start point, which will be processed in each action executed and, if necessary, turned into several tokens. It is therefore possible that a place contains several tokens, for example, several delivery notes issued for different parts of a same order. Each token will then be processed separately, that means, that the subsequent actions will be executed once for each available token.

### Prerequisites

- A workflow is created, see [Create a workflow](01_ManageWorkflows.md#create-a-workflow).
- A workflow process has been initiated, see [Link](#to-be-determined).


### Procedure

*Workflows > Processes > Tab OVERVIEW > Select process > Tab Tokens*

[comment]: <> (Specify Tab Tokens or start with OVERVIEW -> clicking on place shows tokens too?)

![Workflow](/Assets/Screenshots/ActindoWorkFlow/Workflows/Tokens.png "[Workflow]")

1. Click a place in the workflow process diagram to display the available token(s).  
The available token(s) in the selected place are displayed in the *Tokens* tab.

  > [Info] If the workflow process is finished, all available tokens are placed in the end point.

2.  Check the status of the selected token(s) in the *Status* column.  
  The following statuses are available:

  - Processed (green)
  - Being processed (blue)
  - Ready (grey)
  - Error (red)


3. Click the *Hide processed* ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") (Toggle) button to hide the processed tokens.    
All unprocessed tokens are displayed.  

> [Info] Tokens can also be filtered with the filter options. Click the ![Filter](/Assets/Icons/Filter.png "[Filter]") (Filter) button to display the filter options. For detailed information, see [Link](#to-be-completed).

4. Check the place where the token(s) are located in the *Place* column.  

5. Check what type of data is the selected token in the *Data* column.


### Next steps

- [To be completed](#to-be-completed)

### See also

- [Troubleshooting](#to-be-determined)
