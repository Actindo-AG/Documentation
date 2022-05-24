[!!Workflows](ActindoWorkFlow)

# Retry a single process action

## Error Description

A process actions fails and the process action status *Error* is displayed.

Follow the instructions below to restart the process action after you have fixed the cause of the error.


## Prerequisites

The cause of the faulty process action is fixed.

## Procedure

*Workflows > Processes > Tab OVERVIEW*

![Faulty process](/Assets/Screenshots/ActindoWorkFlow/Processes/FaultyProcess.png "[Faulty process]")

1. Click the process with the **Error** status in the *Status* column.   
  The *Process ID* view of the selected process is displayed.

  ![Faulty process ID](/Assets/Screenshots/ActindoWorkFlow/Processes/FaultyProcessID.png "[Faulty process ID]")

2. Click the faulty process action in the process graph.   
  The selected action is displayed in the *Actions* tab in the bottom part of the *Process ID* view.

  > [Info] Switch to the *Logs* tab and click the log with the **Error** type in the column *Type* to display the *Log ID* view with the complete log message to the error.

3. Select the checkbox of the faulty action.   
  The editing toolbar is displayed.

  ![Error action selected](/Assets/Screenshots/ActindoWorkFlow/Processes/ErrorActionSelected.png "[Error action selected]")

4. Click the ![Retry](/Assets/Icons/Retry01.png "[Retry]") (Retry) button in the editing toolbar.     
The process action is restarted. The status of the restarted process action changes to **In Progress**. The *Status change successful* pop-up window indicating the number of restarted process actions is displayed.

  ![Status change successful](/Assets/Screenshots/ActindoWorkFlow/Processes/StatusChangeSuccessful.png "[Status change successful]")

## See also

- [User Interface Workflows](/ActindoWorkFlow/UserInterface/00_UserInterface.md)
- [Retry multiple process actions](#retry-multiple-proces-actions)
- [Track a workflow process](/ActindoWorkFlow/Operation/02_TrackWorkflowProcess)
- [Workflow elements](/ActindoWorkFlow/UserInterface/01_WorkflowElements.md)



# Retry multiple process actions

## Error Description

Multiple process actions fail and the process action status *Error* is displayed for these actions.

Follow the instructions below to restart the process actions after you have fixed the cause of the error(s).


## Prerequisites

The cause of the faulty process actions is fixed.

## Procedure

*Workflows > Process Actions > Tab OVERVIEW*

![Process actions](/Assets/Screenshots/ActindoWorkFlow/ProcessActions/ProcessActions.png "[Process actions]")

1. Click the *Status* drop-down list and select the **Error** option.  
All failed process actions are displayed in the list of actions.

  ![Error process actions](/Assets/Screenshots/ActindoWorkFlow/ProcessActions/ErrorProcessActions.png "[Error process actions]")

2. Select the checkboxes of all faulty actions you want to retry. If you want to retry all faulty actions in the list, you can also select the checkbox in the header.   
  The editing toolbar is displayed.

  ![Error actions selected](/Assets/Screenshots/ActindoWorkFlow/ProcessActions/ErrorActionsSelected.png "[Error actions selected]")

4. Click the ![Retry](/Assets/Icons/Retry01.png "[Retry]") (Retry) button in the editing toolbar.     
All selected process actions are restarted. The status of the restarted process actions changes to **In Progress**. The actions are removed from the *Error* status list. The *Status change successful* pop-up window indicating the number of restarted process actions is displayed.

  ![Status change successful](/Assets/Screenshots/ActindoWorkFlow/Processes/StatusChangeSuccessful.png "[Status change successful]")

## See also

- [User Interface Workflows](/ActindoWorkFlow/UserInterface/00_UserInterface.md)
- [Retry a single process action](#retry-a-single-proces-action)
- [Track a workflow process](/ActindoWorkFlow/Operation/02_TrackWorkflowProcess)
- [Workflow elements](/ActindoWorkFlow/UserInterface/01_WorkflowElements.md)


## Was this chapter helpful?

If you need further assistance, please contact the Customer Support.
