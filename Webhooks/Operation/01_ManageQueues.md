[!User Interface Queue](../UserInterface/03_Queue.md)

# Manage queues

In the queue, you can retry failed webhooks, reset the execution of webhooks, and delete no longer needed or finally failed webhooks.

[comment]: <> (failed webhook oder failed webhook message?)

The webhooks can have different statuses that define the actions that you can perform on these webhooks.
 - *Ready to be sent*:     
    Webhook messages that wait to be executed/sent by the worker. Note that not all webhook messages in the queue with this status will be sent by the worker. Before sending, the worker identifies those webhook messages that meet the conditions defined. Messages that do not meet the conditions, are automatically removed from the queue. In addition, all webhooks that are waiting to be retried are in this list.
 - *Pre remove*   
    Internal status that is used to temporarily store data that is to be removed.
 - *Success*   
    Webhook messages that have been sent successfully.
 - *Failed*    
    Webhooks messages that have finally failed at the last retry.

> [Info] The *Queues* view contains all queue entries ever created for the webhooks. Only queue entries with status *Success* are automatically deleted after ten days.


## Retry queue entry

Retry sending the webhook.

#### Prerequisites

At least one queue entry is available with status *Failed*.

#### Procedure

*Webhooks > Queue*

![Queue](../../Assets/Screenshots/Webhooks/Queue/Queue.png "[Queue]")

1. Select the desired queue entries with status *Failed*.   
   The [![Retry](../../Assets/Icons/Replay.png "[Retry]") RETRY] button is enabled/highlighted.

2. Click the [![Retry](../../Assets/Icons/Replay.png "[Retry]") RETRY] button.   
    The workers are started to retry sending the webhooks. If the retry is successful, the related queue entries change their status to *Success*. If the retry fails again, the related queue entries remain in the status *Failed*.   

3. Analyze the log for the entries remained in the status *Failed*. For detailed information, see <!---To be enhanced, when log is available-->

4. If you can resolve the issue causing the error, retry the queue entries again. 

5. If you cannot resolve the issue causing the error, you will need to manually transfer the message. The *Queue entry* view displays the details of what should have been sent by the webhook. For detailed information, see [Details of queue entry](../UserInterface/03_Queue.md#details-of-queue-entry).



## Reset queue entry

Reset the number of retries to start again following the retry algorithm. You can only retry queue entries that have a number in the *Tries* column that is not 0.

#### Prerequisites

At least one queue entry is available with status *Failed*.

#### Procedure

*Webhooks > Queue*

![Queue](../../Assets/Screenshots/Webhooks/Queue/Queue.png "[Queue]")

1. Click the checkbox of the queue entry you want to reset.   
   The [![Reset](../../Assets/Icons/Reset.png "[Reset]") RESET] button is enabled/highlighted.

[comment]: <> (Check Verhalten im neuen UI wenn verfügbar)

2. Click the [![Reset](../../Assets/Icons/Reset.png "[Reset]") RESET] button.   
    The workers are started again to follow the retry algorithm defined in the worker. 



## Delete queue entry

Delete a queue entry that has finally failed and for which you have manually sent the message. This is recommended so that you can keep track of the entries you still need to analyze. 

#### Prerequisites

At least one queue entry is available with status *Failed*.

#### Procedure

*Webhooks > Queue*

![Queue](../../Assets/Screenshots/Webhooks/Queue/Queue.png "[Queue]")

1. Click the checkbox of the queue entry you want to delete.   
   The [![Delete](../../Assets/Icons/Trash10.png "[Delete]") DELETE] button is enabled/highlighted.

2. Click the [![Delete](../../Assets/Icons/Trash10.png "[Delete]") DELETE] button.   
    The queue entry is deleted.