# Manage webhooks


## Create webhook

Create a webhook to send messages to your business partners.

*Webhooks > Webhooks*

![Webhooks](../../Assets/Screenshots/Webhooks/Webhooks/Webhooks.png "[Webhooks]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.    
    The *Create webhook* view is displayed.

    ![Create webhook](../../Assets/Screenshots/Webhooks/Webhooks/CreateWebhook.png "[Create webhook]")

2. Enter the class name to be used for the webhook in the *Fully qualified class name* field.
<!--- Wo kriege ich den her? Beschreiben, wie man da dran kommt.-->
3. Enter the URL of the message receiver in the *URL* field.

4. Click the *Event* drop-down list and click the checkbox for each event that you want to trigger the webhook. The following events are available:

    - **Post persist**   
        A new database entry has been added such as a new offer.      
    - **Post update**   
        An existing database entry has been changed, for example, the name of an offer has been changed.   
    - **Post remove**   
        An existing database entry has been deleted, for example, if an offer is no longer available.

    The selected events are added to the *Event* field.

    ![Select event](../../Assets/Screenshots/Webhooks/Webhooks/SelectEvent.png "[Select event]")

5. If applicable, click the *Worker* drop-down list and select the worker to process the webhook. You can also add this information later after you have created the worker. For detailed information, see [Create worker](./03_ManageWorkers.md#create-worker).
   
6. Click the [CREATE] button.   
    <!---Ergänzen, wenn UI da. Was passiert dann?-->


## Edit webhook

Edit the webhook to add the number of retries, the workers, or optional properties.

### Prerequisites

A webhook has been created, see [Create webhook](#create-webhook).

### Procedure

*Webhooks > Webhooks*

![Webhooks](../../Assets/Screenshots/Webhooks/Webhooks/Webhooks.png "[Webhooks]")

1. Click the webhook you want to edit.
    The *Webhook "Webhook class name"* view is displayed.

    ![Edit webhook](../../Assets/Screenshots/Webhooks/Webhooks/EditWebhook.png "[Edit webhook]")

2. 


## Define webhook conditions