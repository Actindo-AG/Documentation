[!!Workflows](Workflows)

# Track the workflow process

A process is an instance of a workflow. When a transaction is performed, a piece of data is generated, for example an invoice, which in turn initiates a workflow process.

Similarly to a workflow, a process has a start and an end point, as well as different stages (places and actions) which the initial data goes through in order to be processed.

The workflow process can produce an error due to misconfiguration or other external issues, and therefore can be tracked for errors to be solved.

[comment]: <> (Nicht nur!)  


[comment]: <> (introductory text about the function and use, explain briefly what processes and actions are used for and when to check them)


## Check the process status

The *Processes* menu entry displays a read-only view of any process taking place in real time and a list of all actions being executed in the selected process. For detailed information about tracking a workflow process, see [Link](#to-be-completed).

A process is started with one token at the start point, which will be processed in each action executed and, if necessary, turned into several tokens. It is therefore possible that a place contains several tokens, for example, several delivery notes issued for different parts of a same order. Each token will then be processed separately, that means, that the subsequent actions will be executed once for each token available.

The workflow process view displays the actions in different colours depending on their current status:

  - Green: done
  - Blue: active
  - White: waiting
  - Red: error

### Prerequisites

- A workflow is created, see [Create a workflow](01_ManageWorkflows.md#create-a-workflow).
- A workflow process has been initiated, see [Link](#to-be-determined).

### Procedure

*Workflows > Menu entry Processes > Tab OVERVIEW*

![Workflow](/Assets/Screenshots/Workflows/Workflows/Processes.png "[Workflow]")


### Next steps

- [Check the process action status](#check-the-process-action-status)
- [Check the token status and content](#check-the-token-status-and-content)


### See also

- [Troubleshooting](#to-be-determined)


## Check the process action status

*Workflows > Menu entry Processes > Tab OVERVIEW > Select process > Tab Actions*

![Workflow](/Assets/Screenshots/Workflows/Workflows/ProcessActions.png "[Workflow]")

### Prerequisites

- A workflow is created, see [Create a workflow](01_ManageWorkflows.md#create-a-workflow).
- A workflow process has been initiated, see [Link](#to-be-determined).

### Procedure



### Next steps

- [Check the token status and content](#check-the-token-status-and-content)

### See also



## Check the token status and content

*Workflows > Menu entry Processes > Tab OVERVIEW > Select process > Tab Tokens*

![Workflow](/Assets/Screenshots/Workflows/Workflows/Tokens.png "[Workflow]")

### Prerequisites

- A workflow is created, see [Create a workflow](01_ManageWorkflows.md#create-a-workflow).
- A workflow process has been initiated, see [Link](#to-be-determined).

### Procedure






### Next steps

- [To be completed](#to-be-completed)


### See also
