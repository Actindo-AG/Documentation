# Key features

- Combination with execution workers    
    Each Actindo webhook is given how it should be processed. It is a combination of itself with an execution worker, which defines how the webhooks are to be sent. The webhook defines the recipient and the data that should trigger the events, the execution worker identifies the affected webhooks in the queue. 

- Definition of retries   
    If the recipient is currently down or other situations prevent a webhook from being successfully sent: It will be retried as many times you have specified in the execution workers until the recipient confirms receiving the message.

- Conditions    
    You can strictly narrow the circumstances under which a webhook message is to be sent. For example, a stock level change should trigger the sending of a message.  Message will be sent immediately, as soon as the described change has been made to an entity. There is no need to send a request to receive messages.

- Using of DataHub properties  
    The webhooks are much more flexible than an API that is restricted to a specific module entity. In the *DataHub* module, you can quickly add attributes that you want to have in addition to the default attributes. If you have customer-specific DataHub entities that should trigger an event, you can add them to the webhook definition.

- Authentication   
    You can optionally use an authentication method, whereby you can choose between xxxx or a secret key (standard hash algorithm **sha265**).    



## Constraints

- Data that can be sent via the *Webhook* module must follow the Actindo data models and is restricted to them. 
- Direct database accesses cannot be processed, because the events are processed in the doctrine layer, a layer between the code and the databases.
- Webhooks are not suitable for large data volumes such as order statistics, but very flexible for sending messages containing single changes.

