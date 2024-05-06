# Manage workers

The workers define how the webhooks waiting in the queue are to be executed. Since you need the workers for defining the webhooks, you must first create the workers. The workers define the retry algorithm, which specifies the number of retries as well as if the webhook messages in the queue are processed sequentially or in parallel.

**Sequential processing**   
Sequential processing of webhooks is recommended for events that are related to status changes. For example, an order status change must be sent in the correct update sequence so that the status "Completed" is not overwritten by the status "Delivered". In sequential processing, only one worker processes the webhooks.<!---Wie heißen die korrekten Status für die Order?-->

> [Info] When defining the webhooks, you can specify conditions such as special fields that are to be considered. For detailed information, see [Define webhook conditions](./02_ManageWebhooks.md#define-webhook-conditions).

**Parallel processing**   
Parallel processing of webhooks is recommended for events where there is no particular sequence to follow. For example, all post persist events are suitable for parallel processing. The advantage of parallel processing is that you can define the number of workers, so you can respond to high system loads.

## Create worker

Create a worker that you will assign to a webhook later. To know the workers you will need, you need to have an idea of the different characteristics of the workers. 
Alternatively, you can define the webhooks first and associate the workers later by editing the webhooks.<!---Geht das wirklich? Prüfen--> 

#### Prerequisites

No prerequisites to fulfill.

#### Procedure

*Webhooks > Workers*

![Workers](../../Assets/Screenshots/Webhooks/Workers/Workers.png "[Workers]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.    
    The *Create worker* view is displayed.

    ![Create worker](../../Assets/Screenshots/Webhooks/Workers/CreateWorker.png "[Create worker]")

2. If you want to activate the worker directly when saving it, click the activate checkbox. Alternatively, you can activate the worker later, see [Activate worker](#activate-worker).

3. Define whether you want this worker for sequential execution. In this case, click the *Sequential execution* checkbox.   
    The *Number of jobs* field is hidden, because in sequential execution only one worker executes the webhooks.

2. Enter a name for the worker in the *Name* field. It is recommended to describe the execution mode and the retry algorithm in the name for better identification later.

3. Define the retry algorithm comma-separated in the *Retry algorithm* field. It defines the time intervals in seconds in which the worker execution should be retried after a webhook message could not be sent successfully. You can let the field empty. In this case, the default is used: 1, 2, 3, 4 (1 => 60 sec, 2 => 120 sec, 3 => 300 sec, 4 => 600 sec) You have the following options: <!---Ergänzen-->

4. Define the number of jobs in case you have decided for parallel processing.  

5. Click the [CREATE] button.   
    The *Create worker* view is closed and the *Workers* view is displayed.

## Activate worker

Activate a worker if you want to use it for processing the queue.

#### Prerequisites

At least one worker has been created, see [Create worker](#create-worker).

#### Procedure

*Webhooks > Workers*

![Workers](../../Assets/Screenshots/Webhooks/Workers/Workers.png "[Workers]")

1. Click the checkbox at the worker(s) you want to activate.   
    The [ACTIVATE] button on the top left is highlighted.

2. Click the [ACTIVATE] button.   
    The status of the worker(s) in the *Active* column has switched to ![Active](../../Assets/Icons/Check.png "[Active]") (Active). <!---Icon-->



## Deactivate worker

Deactivate a worker if you no longer want to use it. Note that all associated webhooks will no longer be executed after deactivating a worker.

#### Prerequisites

At least one worker has been created, see [Create worker](#create-worker).

#### Procedure

*Webhooks > Workers*

![Workers](../../Assets/Screenshots/Webhooks/Workers/Workers.png "[Workers]")


1. Ensure that no unwanted webhook is associated with the worker(s) you want to deactivate. To do this, select the worker for which you want to check the webhook association.   
    The *DETAILS* tab of the webhook is displayed.

2. Click the *WEBHOOKS* tab.   
    All webhooks associated with the worker are displayed.

    ![Associated webhooks](../../Assets/Screenshots/Webhooks/Workers/WebhooksWorker.png "[Associated webhooks]")

3. Remove the webhook association. For detailed information, see [Remove associated worker](./02_ManageWebhooks.md#remove-associated-worker). Do this for all workers that are listed in the *Webhooks* tab. 

4. Click the checkbox at the worker(s) you want to deactivate. 
    The [DEACTIVATE] button on the top left is highlighted.

4. Click the [DEACTIVATE] button.   
    The status of the worker(s) in the *Active* column has switched to ![Inactive](../../Assets/Icons/Cross03.png "[Inactive]") (Inactive). <!---Icon-->   



## Disable execution of workers

Disable the workers so that no new workers are executing the queue. This might be necessary when editing the workers or webhooks.

#### Prerequisites

- You have the permission to enable/disable feature flags in the engine room.

#### Procedure

*Actindo Core1 Platform > Any workspace> Click the engine room button*

<!---Screenshot von Engine room-->

1. Enable the *Disable workers* toggle in the *Webhooks* box.<!---Namen prüfen--> For detailed information, see [Switch on&frasl;off single feature flags](Core1Platform/AdministratingCore1/06_ExpertKnowledge.md#switch-on⁄off-single-feature-flags) in the *Core1 Platform* documentation.   
    The webhook workers have been disabled. No new webhooks will be sent as long as the *Disable workers* toggle is enabled.

2. Disable the *Disable workers* toggle in the *Webhooks* box after you have finished editing the workers or webhooks.   
    The execution of the queue will be continued after one minute. 

## Shut down workers

Sometimes it may be necessary to stop the current execution of the queue for specific workers, for example, if you want to edit the worker or associated webhooks. Therefore, you have to shut down a worker to avoid that the associated webhooks are executed by this worker. Alternatively, you can shut down all workers. <!---wie starte ich einen worker wieder?-->    


### Shut down single worker

Shut down a single worker to avoid that the associated webhooks are executed by it. <!---wie starte ich einen worker wieder?-->

#### Prerequisites

- At least one worker has been created, see [Create worker](#create-worker).
- At least one worker is active.

#### Procedure

*Webhooks > Workers*

![Workers](../../Assets/Screenshots/Webhooks/Workers/Workers.png "[Workers]")

1. Click the checkbox at the active worker you want to shut down.    
    The [![Shut down](../../Assets/Icons/Cross03.png "[Shut down]")<!---Icon-->SHUT DOWN] button is enabled.

2. Click the [![Shut down](../../Assets/Icons/Cross03.png "[Shut down]")<!---Icon-->SHUT DOWN] button.   
    The worker is stopped. The associated webhooks in the queue are no longer executed.


### Shut down all workers

Shut down all workers to stop the current execution of all webhooks in the queue. <!---In welchen Situation würde ich das tun? wie starte ich einen worker wieder?-->   
To avoid, that workers are started again by an event, you must disable the workers, see [Disable workers](#disable-workers).

#### Prerequisites

At least one worker has been created, see [Create worker](#create-worker).

#### Procedure

*Webhooks > Workers*

![Workers](../../Assets/Screenshots/Webhooks/Workers/Workers.png "[Workers]")

Click the [![SHUT DOWN ALL](../../Assets/Icons/Cross03.png "[SHUT DOWN ALL]")<!---Icon-->SHUT DOWN] button to right.   
The execution of all currently running workers is stopped.


## Delete worker

Delete a worker if you no longer need it. You can only delete workers that are not associated to any webhook. 

#### Prerequisites

At least one worker has been created, see [Create worker](#create-worker).

#### Procedure

*Webhooks > Workers*

![Workers](../../Assets/Screenshots/Webhooks/Workers/Workers.png "[Workers]")

1. Ensure that no webhook is associated with the worker(s), you want to delete. To do this, select the worker for which you want to check the webhook association.   
    The *DETAILS* tab of the webhook is displayed.

3. Click the *WEBHOOKS* tab. 
    All webhooks associated with the worker are displayed.

    ![Associated webhooks](../../Assets/Screenshots/Webhooks/Workers/WebhooksWorker.png "[Associated webhooks]")

    <!--- Hallo Hendrik, hier sieht es so aus, als wenn ich hier einen Webhook löschen könnte. Aber ich will doch nur die Zuordnung löschen, oder nicht?-->

4. Remove the webhook association. For detailed information, see [Remove associated worker](./02_ManageWebhooks.md#remove-associated-worker). Do this for all workers that are listed in the *Webhooks* tab.

6. Return to the *Workers* view.

7. Select the worker(s) you want to delete.   
    The [![DELETE](../../Assets/Icons/Trash04.png "[DELETE]")<!---Icon-->DELETE] button is highlighted.

8. Click the [![DELETE](../../Assets/Icons/Trash04.png "[DELETE]")<!---Icon-->DELETE] button.   
    The worker is deleted.






