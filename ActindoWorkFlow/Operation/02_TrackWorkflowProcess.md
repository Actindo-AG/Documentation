[!!Workflows](ActindoWorkFlow)

# Track the workflow process

A process is an instance of a workflow. When a transaction is performed, a piece of data is generated, for example an invoice, which in turn initiates a workflow process. Therefore, for every single transaction performed, an individual instance of the corresponding workflow, that is, a process, is initiated.

A process has a start and an end point, as well as different stages (places and actions) which the initial data goes through in order to be processed. For a detailed description of the workflow elements, see [Workflow elements](/ActindoWorkFlow/UserInterface/01_WorkflowElements.md).

The workflow process can be tracked to check the status of a whole process or of individual actions, as well as the status and the content of a token.


## Check the process status

The process status can be checked to see how far a process has progressed, detect potential problems, and solve any problems that may occur as a result of a misconfiguration or any other external issues, so that the process can continue running.

The *OVERVIEW* tab in the *Processes* menu entry displays a list of all processes that are currently being executed or have been executed in the system. Per default, all existing processes are displayed but can also be filtered according to different criteria.


### Prerequisites

- A workflow is created, see [Create a workflow](01_ManageWorkflows.md#create-a-workflow).
- A workflow process has been initiated.

### Procedure

*Workflows > Processes > Tab OVERVIEW*

![Processes](/Assets/Screenshots/ActindoWorkFlow/Workflows/Processes.png "[Processes]")

1. Click the *Status* drop-down list and select the **All** option.  
All processes, regardless of their status, are displayed.

2. Click the *Workflow* drop-down list and select the approriate workflow.  
All processes of the selected workflow are displayed.

3. Check the status of the appropriate workflow process in the *Status* column of the processes list.

> [Info] If desired, you can click the process to display the *Process ID* view with a diagram of the process including detailed information about the individual process actions and tokens.    
For detailed information about individual process actions, see [Check the process action status](#check-the-process-action-status) .   
For detailed information about tokens, see [Check the token status and content](#check-the-token-status-and-content).

### Next steps

- [Check the process action status](#check-the-process-action-status)
- [Check the token status and content](#check-the-token-status-and-content)

### See also

- [Troubleshooting](#to-be-determined)



## Check the process action status

The process action status can be checked to prove which actions have already been executed, if problems have occurred and at what place.

The *Process ID* view displays a diagram of the selected process including all places and actions. If the process is currently active, the process execution can be observed in real time.

Further details about the process actions included in the diagram as well as about the logs and tokens are displayed in separate tabs in the bottom part of the *Process ID* view.

### Prerequisites

- A workflow is created, see [Create a workflow](01_ManageWorkflows.md#create-a-workflow).
- A workflow process has been initiated.

### Procedure

*Workflows > Processes > Tab OVERVIEW > Select process*

![Process actions](/Assets/Screenshots/ActindoWorkFlow/Workflows/ProcessActions.png "[Process actions]")

1. Click the *Actions* tab in the bottom part of the *Process ID* view.   
  The *Actions* tab is displayed.

  > [Info] By default, the *Actions* tab is preselected.

  [comment]: <> (By default? Actions Reiter scheint standardmäßig ausgewählt zu sein, wenn man einen Prozess aus der Liste anklickt. Das heißt, erster Schritt etwas überflüssig)

2. Click the *Status* drop-down list and select the **All** option.    
  All actions, regardless of their status, are displayed.

  > [Info] By default, the *Actions* tab lists all actions contained in the selected process.

[comment]: <> (OLI: wenn eine Action/Token in einem Prozess ausgewählt werden, wird es als Filtereinstellung übernommen. Diese Filtereinstellung bleibt erhalten, auch man zu einem anderen Prozess wechlselt, daher sieht man nicht alle Actions, auch wenn auf "All" klickt. Bug oder erwartetes Verhalten?)

3. Check the actions displayed in the diagram.  
The workflow process diagram displays the actions in different colours depending on their current status:

  - Active (blue)
  - Done (green)
  - Waiting (white)
  - Error (red)
  - Dead (black)

 [comment]: <> (Andere möglichen Status? Vgl. mit Status in Actions Reiter: Active, Done, Error, Error; automatic retry, Suspended, Process aborted. Farben stimmen oder ändern sich noch?)

 [comment]: <> (Oli: Statuses Error; automatic retry, Suspended and Process aborted. Wo stellt man "automatic retry" ein?)

4. Click the action to be checked in the diagram.  
The selected action is displayed in the *Actions* tab.

5. Check the action status in the *Status* column and any further relevant information about the action displayed in the following columns:

  - *Tries*: The number of times an action has been tried.
  - *Maximal retries after error*: The number of times an action must be retried after error.
  - *Queue type*: The *Default* queue type is normally selected. For detailed information about configuring queue types, see [Configure the queue types](#to-be-competed).

    > [Info] A different queue type can be selected by editing an action, see [Edit an action](01_ManageWorkflows.md#edit-an-action).

  - *Defer until*: The next point in time when the action is being tried.

[comment]: <> (Oli: Is it possible to configure it somehow, i.e. Tries, Maximal retries after error and Defer until?)

6. If an error is displayed, a troubleshooting procedure can be performed. For detailed information, see [Troubleshooting](ActindoWorkFlow/Troubleshooting/00_Troubleshooting.md).

  > [Info] The *Token* tab displays detailed information about the tokens being processed in the actions. For detailed information about tokens, see [Check the token status and content](#check-the-token-status-and-content).

7. Check the *Logs* tab for further details on the error displayed.

  > [Info] A list of all actions, regardless of the process they are part of, can be displayed in the *Process Actions* tab. They can be filtered according to their status and modified simultaneously, if necessary. By clicking a specific action in the process actions list, the corresponding process will be displayed.

[comment]: <> (Oli: Logs tab auch nur in Troubleshooting oder in separatem Kapitel? Process actions wird zu einem ein Tab unter Processes, richtig?)

### Next steps

- [Check the token status and content](#check-the-token-status-and-content)

### See also

- [Troubleshooting](#to-be-determined)



## Check the token status and content

The token status and content can be checked to see how data progress within a process and, if necessary, detect and solve any data type related issues.   

The *Tokens* tab displays the tokens being processed. A token is a piece of data needed to complete an action, for example a document. When a transaction is performed, a token is generated, for instance an invoice, which in turn initiates the workflow process.

A process is started with one token at the start point, which will be input in an action to be executed. In turn, an action can output several tokens, which will become inputs for subsequent actions. It is therefore possible that a place contains several tokens, for example, several delivery notes issued for different parts of a same order. Each token will then be processed separately, that means, that the subsequent actions will be executed once for each token available.

### Prerequisites

- A workflow is created, see [Create a workflow](01_ManageWorkflows.md#create-a-workflow).
- A workflow process has been initiated, see [Link](#to-be-determined).

### Procedure

*Workflows > Processes > Tab OVERVIEW > Select process*

![Workflow](/Assets/Screenshots/ActindoWorkFlow/Workflows/Tokens.png "[Workflow]")

1. Click the *Tokens* tab.  
If the *Hide processed* toggle is active, only the tokens currently waiting to be further processed are displayed.

2. Deselect the *Hide processed* toggle, if active.  
 All tokens, including the ones that have already been processed, are displayed.

3. Check the places displayed in the diagram.  
The places are green if a token has been input (token status is processed or being processed). If no token has been input yet, the places are white.

 > [Info] A place can contain a black square displaying a number. This number specifies the number of tokens waiting to be processed at that place. Besides, a number is also displayed next to the status of each action. This number refers to the number of tokens processed in this action, and it depends on the action status and the number of tokens received. For further information, see [Workflow elements](ActindoWorkFlow/UserInterface/01_WorkflowElements.md#tokens).

4. Select a place in the diagram.  
Depending on its status and the toggle settings, the token input in the selected place is displayed in the *Tokens* tab.

5. Check the token status in the *Status* column.  
The following statuses are available:

  - Processed (green)
  - Being processed (blue)
  - Ready (grey)
  - Error (red)


  [comment]: <> (Oli: Andere Status? Status korrekt? Farben bei Dead, Suspended, Aborted? Vgl. Status/Farben Places/Actions/Tokens -> ähnlich aber leicht unterschiedlich. Ist es möglich zu vereinheitlichen?)

  Check any relevant information about the token displayed in the following columns:  

  - *Place*: The place where the token has been input.
  - *Data*: The type of data contained in the token.
  - *Next possible action(s)*: The next compatible action(s) where the token can be input.

[comment]: <> (OLI: Next possible action/s? Data - Token, sind die beiden Synonyme, wie kann man beide im Bezug zueinander besser beschreiben?)

6. Click on an action in the diagram to display further information in the *Actions* tab. For detailed information about checking action status, see [Check the process action status](#check-the-process-action-status).

7. Check the *Logs* tab for further details on any process action.

[comment]: <> (OLI: Logs vielleicht auch nur in Troubleshooting oder in separatem Kapitel? Beziehen sich Logs auf Tokens auch oder nur auf Actions/Transitions?)


### Next steps

- [To be completed](#to-be-completed)

### See also

- [Troubleshooting](#to-be-determined)
