# Queue

*Webhooks > Queue*

![Workers](../../Assets/Screenshots/Webhooks/Queue/Queue.png "[workers]")

The list shows all webhooks in the queue that are waiting to be executed/sent, as well as all those that have been sent successfully and those that have failed. Depending on the settings, the displayed columns may vary. All fields are read-only.

The following functions are available for the row above the list header:

- ![Select](../../Assets/Icons/Checkbox.png "[Select]") <!--- Icon-->   
   Select the checkbox to the left of a list entry. This allows you to select one or more entries for an action, which you can then perform by clicking a button in the upper left corner above the list header.
    If you click the checkbox in the list header, all entries in the list are selected. 

- [![Retry](../../Assets/Icons/Retry01.png "[Retry]") RETRY]<!---Icon-->    
    Click this button to retry sending the webhook. 

- [![Reset](../../Assets/Icons/Reset.png "[Reset]") RESET]<!---Icon-->   
    Click this button to reset the amount of tries, so that the system again tries to send the webhooks, depending on the *Retry algorithm* defined in the worker. The button is disabled, if the number of tries is equal to zero.

- [![Delete](../../Assets/Icons/Trash01.png "[Delete]") DELETE]    
    Click this button to delete a queue entry. <!---You can delete several webhooks at once?-->

The following fields are available in the list:
- *ID*   
    ID of the queue entry.

- *Webhook*   
    Class name of the webhook.

- *Execution worker*   
    Name of the worker.

- *Entry status*   
    Status of the queue entry. The following statuses are available:

    - **0 = Ready to be sent**   
        The webhook is waiting to be sent.
    - **1 = Success**   
        The webhook was sent successfully
    - **2 = Failed**   
        The sending of the webhook failed and the amount of tries reached the maximum. This entry must be handled manually.   
    - **3 - Pre remove**   
        This entry has been created during preremove. This status will be set to *Ready to be sent* during the postRemove event.<!--????nachfragen-->

- *Event*   
    Event that has triggered the webhook.

- *Tries*   
    Number of tries the worker has needed so far to send the webhook.

