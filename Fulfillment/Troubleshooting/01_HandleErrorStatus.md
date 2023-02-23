[!!Export a dispatch note](../Operation/01_ManageDispatchNotes.md#export-a-dispatch-note) 
[!!Workflows](../../ActindoWorkFlow/Overview/01_General.md) 

# Handle an error status

The *Fulfillment* module manages the communication between the *Actindo Core1 Platform* and the fulfillment partner(s). Occasionally, a dispatch note or a shipment may display an error.

An error status may be set for many different reasons and strongly depends on the connection and the fulfiller's own internal processes. 

A dispatch note usually displays an error status when the data export from the Core1 to the partner's system has failed. A shipment, on the other hand, may display an error status when the fulfiller has reported an error, for instance because the shipment could not be arranged, but also when no feedback from fulfiller has been received. The errors are notified via the ![Notifications](../../Assets/Icons/Notifications.png) icon (Notifications) on the upper right corner as they occur.

In any case, the corresponding workflow stops at the point where the error occurs. The *Actindo Core1 Platform* logging system provides detailed information on any error, which allows to identify the cause and implement the appropriate solution.

#### Error Description

The *Status* or the *Shipment status* columns in the list of dispatch notes display an error.

Follow the instructions below to identify the cause of the error and proceed accordingly.

#### Prerequisites

No prerequisites to fulfill.

#### Procedure

*Fulfillment > Dispatch notes > Tab LIST*

![Error status](../../Assets/Screenshots/Fulfillment/DispatchNotes/DispatchNotesErrorStatus.png "[Error status]")

1. Click the dispatch note displaying an error in the *Status* or the *Shipment status* columns.  
    The *Dispatch note "Dispatch note ID"* view is displayed. 

2. Click the *Logs* sub-tab.  
    The list of intents related to the selected dispatch note are displayed.

    ![Logs](../../Assets/Screenshots/Fulfillment/DispatchNotes/DispatchNoteLogsError.png "[Logs]")

3. Click the desired intent from the list to access further information.  
    The list of messages is displayed.  

    ![Messages](../../Assets/Screenshots/Fulfillment/DispatchNotes/DispatchNoteLogsMessages.png "[Messages]")

4. If necessary, click the relevant message for further information.  
    The *Detail of log message "Log message name"* is displayed.
 
5. If no further information is detailed or the information displayed is not conclusive, click the [CLOSE] button in the upper right corner to close the current view.  
    The list of dispatch notes is displayed again. 

6. Copy the dispatch note number in the *Document number* column to your clipboard.

    > [Note] The document number equals the delivery note number in the *Order management* module.

7. Switch to the *Workflows* module and select the *Processes* menu entry.  
    The list of processes is displayed. 

    ![Processes](../../Assets/Screenshots/ActindoWorkFlow/Processes/FaultyProcess.png "[Processes]")

8. Paste the document number in the search field and press the **ENTER** key to start the search.  
    The process related to the selected dispatch note number is displayed. 

9. Click the process to display further process details.  
    The *Process ID: "Process ID", Workflow: "Workflow name"* view is displayed. 

    ![Process ID](../../Assets/Screenshots/ActindoWorkFlow/Processes/FaultyProcessID.png "[ProcessID]")
        
    > [Info] The action where the error has ocurred is displayed in red, both in the process diagram as well as in the process actions listed below.

10. Click the *Logs* tab to display all process-related logs.  
    The list of logs is displayed.

     ![Logs](../../Assets/Screenshots/ActindoWorkFlow/Processes/Logs.png"[Logs]")

    > [Info] If necessary, the logs can be filtered by log level.

11. Click the log displaying the error. 
    The *Log ID "Log ID"* view is displayed.

    ![Log ID](../../Assets/Screenshots/ActindoWorkFlow/Processes/LogID.png"[LogID]")

12. Check the log message for further information about the error. Once the error cause has been established, an appropriate solution can be implemented.  

    > [Info] Depending on the source of the error, it may be necessary to take action in one or more additional modules or even to contact externally the fulfillment partner. 

13. After the error cause has been fixed, the action may be retried, see [Retry a process action](../../ActindoWorkFlow/Troubleshooting/01_RetryProcessAction.md). 



  
#### Was this chapter helpful?

If you need further assistance, please contact the Customer Support.
