# Manage webhooks


## Create webhook

Create a webhook to send messages to your business partners.


#### Prerequisites

No prerequisites to fulfill.

#### Procedure

*Webhooks > Webhooks*

![Webhooks](../../Assets/Screenshots/Webhooks/Webhooks/Webhooks.png "[Webhooks]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.    
    The *Create webhook* view is displayed.

    ![Create webhook](../../Assets/Screenshots/Webhooks/Webhooks/CreateWebhook.png "[Create webhook]")

2. Enter the class name to be used for the webhook in the *Fully qualified class name* field. To get the names, see the data models under *Dev Tools > API > Tab DATA MODELS* for reference. Use the data model that contain the entities you want to send with a webhook. Copy the desired data model names and replace the dots with slashes. See the following examples:
    - Actindo\Modules\Actindo\Channels\Models\Offer 
    - Actindo\Modules\Actindo\Channels\Models\Order
    - Actindo\Modules\Actindo\Channels\Models\Shipment

3. Enter the URL of the message receiver in the *URL* field.

4. Click the *Event* drop-down list and click the checkbox for each event that you want to trigger the webhook. The following events are available:

    - **Post persist**   
        A new database entry has been added such as a new offer.      
    - **Post update**   
        An existing database entry has been changed, for example, the name of an offer has been changed.   
    - **Post remove**   
        An existing database entry has been deleted, for example, an offer is no longer available.

    The selected events are added to the *Event* field.

    ![Select event](../../Assets/Screenshots/Webhooks/Webhooks/SelectEvent.png "[Select event]")

5. If applicable, click the *Worker* drop-down list and select the worker to process the webhook. You can also add this information later after you have created the worker. For detailed information, see [Create worker](./03_ManageWorkers.md#create-worker).
   
6. Click the [CREATE] button.   
    <!---Ergänzen, wenn UI da. Was passiert dann?-->

7. Continue with [Edit webhook](#edit-webhook) to specify optional properties and conditions.


## Edit webhook

Edit the webhook to add the number of retries, the workers, or optional properties.

### Prerequisites

At least one webhook has been created, see [Create webhook](#create-webhook).

### Procedure

*Webhooks > Webhooks*

![Webhooks](../../Assets/Screenshots/Webhooks/Webhooks/Webhooks.png "[Webhooks]")

1. Click the webhook you want to edit.
    The *Webhook "Webhook class name"* view is displayed.

    ![Edit webhook](../../Assets/Screenshots/Webhooks/Webhooks/EditWebhook.png "[Edit webhook]")

2. If desired, edit the events. Proceed as follows: 
    - To remove an event from the *Event* field, click the ![Remove](../../Assets/Icons/Cross03.png "[Remove]")<!---Icon--> button at the event name.
    - To add an event, click the *Event* drop-down list and select the event you want to add.

3. If desired, enter the number of retries in the *Workers* field. This number should fit to the *Retry algorithm* specified in the worker definition.

4. If desired, select another worker in the *Worker* drop-down list.

5. If desired, define optional properties in the *Optional properties* section. By doing this, you can narrow the entity for which the webhook is used. You can enter all DataHub entities as well as any database field. The following prerequisites must be fulfilled:   
    - The property must be part of the model you have entered in the *Fully qualified class name* field.    
    - The data must be passed as array.  
    
    See the following examples:   
    - lineItems._channels_order_shipment_line_item_quantity   
    - lineItems._lineitem_idInShop   
    - _order_idInShop   
    - connection   

6. If desired, define conditions to be used to trigger the creation of a webhook message, see [Define webhook conditions](#define-webhook-conditions).



## Define webhook conditions

Define the conditions that must be met to trigger the creation of a webhook message.

#### Prerequisites

At least one webhook has been created, see [Create webhook](#create-webhook).

#### Procedure

*Webhooks > Webhooks > Select a webhook*

![Edit webhook](../../Assets/Screenshots/Webhooks/Webhooks/EditWebhook.png "[Edit webhook]")

1. Click the [![Add condition](../../Assets/Icons/Plus04.png "[Add condition]") ADD CONDITION] in the top right corner of the *Conditions* section.    
    A new condition input line is displayed.

    ![Condition input line](../../Assets/Screenshots/Webhooks/Webhooks/WebhookCondition.png "[Condition input line]")

2. Enter the property on the basis of which you want to trigger the sending of the webhook message. The property must be part of the model you have entered in the *Fully qualified class name* field. Note that DataHub entities need a leading underscore. See the following examples: 
    - _channels_order_deliver_status.oldValue (DataHub)
    - importStatus.newValue.scalar (Channels)<!---ich finde es nicht in den Models?-->
    - connection.id (Channels)
    - _channels_order_deliver_status (DataHub)

3. Select the operator in the *Operator* drop-down list. The operator defines the relation that must exist between the property and the value for a condition to be fulfilled. The following operators are available:
    - **Not equal**
    - **Equal**

4. Define the value in the *Value* field. This describes a value that the property can have. For example, it can be the connection ID or the order delivery status.

5. If you want that the condition applies in the change set, click the checkbox in the *Apply on change set* column.<!---Was bedeutet das?-->

5. If desired, add further conditions by clicking the [![Add condition](../../Assets/Icons/Plus04.png "[Add condition]") ADD CONDITION] button.

6. Specify whether all conditions must be met to trigger the sending of the webhook message. If all must be met, click the [All conditions required] checkbox in the top right corner of the *Conditions* section. If you do not click the checkbox, at least one of the conditions must be met.

7. If desired, delete a condition line by clicking on the ![Delete](../../Assets/Icons/Trash08.png "[Delete]")(Delete) button at the right end of the line.

8. Click the [SAVE CHANGES] button in the top right corner.



## Remove associated worker

Remove an associated worker from a webhook, for example, if you want to delete a worker.

##### Prerequisites

- At least one webhook has been created, see [Create webhook](#create-webhook).
- At least one worker has been created, see [Create worker](./01_ManageWorkers.md#create-worker)

#### Procedure

*Webhooks > Webhooks > Select a webhook*

![Edit webhook](../../Assets/Screenshots/Webhooks/Webhooks/EditWebhook.png "[Edit webhook]")

1. Select another worker in the *Worker* drop-down list.

2. Click the [SAVE CHANGES] button in the top right corner.   
    The webhook association at the worker is no longer displayed.
    
    ![Associated webhooks](../../Assets/Screenshots/Webhooks/Workers/WebhooksWorker.png "[Associated webhooks]")