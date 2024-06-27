# Queue

*Webhooks > Queue*

![Queue](../../Assets/Screenshots/Webhooks/Queue/Queue.png "[Queue]")

The list shows all webhooks in the queue that are waiting to be executed/sent, as well as all those that have been sent successfully and those that have failed. Depending on the settings, the displayed columns may vary. All fields are read-only.

The following functions are available in the row above the list header:

- ![Select](../../Assets/Icons/Checkbox03.png "[Select]")   
   Select the checkbox to the left of a list entry. This allows you to select one or more entries for an action, which you can then perform by clicking a button in the upper left corner above the list header.
    If you click the checkbox in the list header, all entries in the list are selected. 

- [![Retry](../../Assets/Icons/Replay.png "[Retry]") RETRY]      
    Click this button to retry sending the webhook. 

- [![Reset](../../Assets/Icons/ResetTV.png "[Reset]") RESET]   
    Click this button to reset the amount of tries, so that the system again tries to send the webhooks, depending on the *Retry algorithm* defined in the worker. The button is disabled, if the number of tries is equal to zero.

- [![Delete](../../Assets/Icons/Trash10.png "[Delete]") DELETE]    
    Click this button to delete a queue entry. <!---You can delete several webhooks at once?-->

The following fields are available in the list:
- *ID*   
    ID of the queue entry.

- *Webhook*   
    Class name of the webhook.

- *Execution worker*   
    Name of the worker that is configured to execute the webhook.

- *Entry status*   
    Status of the queue entry. The following statuses are available:

    - **Ready to be sent**:     
        Webhook messages that wait to be executed/sent by the worker. Note, that not all webhook messages in the queue with this status will be sent by the worker. Before sending, the worker identifies those webhook messages that meet the conditions defined. Messages that do not meet the conditions, are automatically removed from the queue. In addition, all webhooks that are waiting to be retried are in this list.
    - **Pre remove**   
        Internal status that is used to temporarily store data that is to be removed.
    - **Sucess**   
        Webhook messages that have been sent successfully.
    - **Failed**    
        Webhooks messages that have been finally failed at the last retry.

- *Event*   
    Event that has triggered the webhook.

- *Tries*   
    Number of tries already made.
    


## Details of queue entry 

*Webhooks > Queue > Select queue*

![Queue entry](../../Assets/Screenshots/Webhooks/Queue/QueueDetails.png "[Queue entry]")

The view shows the details of a selected queue entry.

The following queue-related functions are available in the list header:

- *Queue entry ID*  
    ID of the queue entry.

- Status icon    
    Status of the selected queue entry.

- [![Retry](../../Assets/Icons/Replay.png "[Retry]") RETRY]   
    Click this button to retry sending the webhook. 

- [![Reset](../../Assets/Icons/ResetTV.png "[Reset]") RESET]    
    Click this button to reset the amount of tries, so that the system again tries to send the webhook, depending on the *Retry algorithm* defined in the worker. The button is disabled, if the number of tries in the *Tries* field is equal to zero.

- [![Delete](../../Assets/Icons/Trash10.png "[Delete]") DELETE]    
    Click this button to delete the queue entry. 

The following fields and functions are available on the left part of this view:

- *Webhook*   
    Class name of the webhook.

- *Execution worker*   
    Name of the worker that is desired to execute the webhook or has executed it.

- *Event*   
    Event that has triggered the webhook.

- *Tries*   
    Number of tries already made.

- *Execute time*   
    <!---Date and time of the first webhook execution by a worker??.-->
- *Execute after*   
    <!---??? Date and time of the next try to execute the webhook-->
- *Submitted at*   
    <!---Date and time of the change that has triggered the execution of the webhook.-->

- *Submitted by*   
    <!--Name and username of the person who has done the changes that triggered the creation of the webhook.-->

The following fields and functions are available on the right side in this view:

- *Change set*   
    Native webhook message that is to be sent/has been sent. Use the scroll bar on the right to see the whole message.

- *Prepared change set*   
    More readable version of the change set created by the system during first execution. This prepared change set replaces database IDs with keys to make an entry easier to understand. Use the scroll bar on the right to see the whole message.

- *Entity*   
    Detail information in JSON code about the worker which has sent the message.



