[[!!User Interface Supplier receipts](../UserInterface/01_Book.md#Supplier receipts)
[!!Post a supplier receipt](../Operation/10_ManageReceipts.md#post-a-supplier-receipt)]

# Check the supplier receipt settings

You can retry one or several faulty process actions after you have fixed the cause of the error to continue the affected process(es).

#### Error Description

A process action fails and the process action status *Error* is displayed.

Follow the instructions below to restart the process action after you have fixed the cause of the error.

#### Prerequisites

The cause of the faulty process action is fixed.

#### Procedure

*Accounting > Settings > Tab OVERVIEW*

![Faulty process](../../Assets/Screenshots/ActindoWorkFlow/Processes/FaultyProcess.png "[Faulty process]")

1. Click the process with the **Error** status in the *Status* column.   
  The *Process ID* view of the selected process is displayed.

  ![Faulty process ID](../../Assets/Screenshots/ActindoWorkFlow/Processes/FaultyProcessID.png "[Faulty process ID]")

2. Click the faulty process action in the process diagram.   
  The selected action is displayed in the *Actions* tab in the bottom part of the *Process ID* view.

  > [Info] If required, you can switch to the *Logs* tab and click the log with the **Error** type in the column *Type* to display the *Log ID* view with the complete log message to the error.

3. Select the checkbox of the faulty action.   
  The editing toolbar is displayed.

  ![Error action selected](../../Assets/Screenshots/ActindoWorkFlow/Processes/ErrorActionSelected.png "[Error action selected]")

4. Click the ![Retry](../../Assets/Icons/Retry01.png "[Retry]") (Retry) button in the editing toolbar.     
The process action is restarted. The status of the restarted process action changes to **In Progress**. The *Status change successful* pop-up window indicating the number of restarted process actions is displayed.

  ![Status change successful](../../Assets/Screenshots/ActindoWorkFlow/Processes/StatusChangeSuccessful.png "[Status change successful]")
