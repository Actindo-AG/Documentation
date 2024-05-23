# Key features

- Execution workers    
    Each webhook is given how it should be processed. It is a combination of itself with an execution worker, which defines how the webhooks are to be sent. The webhook defines the recipient and the data that should trigger the events, the execution worker identifies the affected webhooks in the queue. 

- Retries   
    If the recipient is currently down or other situations prevent a webhook from being successfully sent: It will be retried as many times you have specified in the execution workers until the recipient confirms receiving the message.

- DataHub properties  
    If you have customer-specific DataHub entities that should trigger an event, you can add them to the webhook definition.

- Conditions    
    You can strictly narrow the circumstances under which a webhook is to be sent, for example, if a stock level has changed.

- Authentification
    You can optionally use an authentication, whereby you can choose between xxxx or a secret key (standard hash algorithm **sha265**).    



    Zurzeit optimal für Channels properties
Direktzugriffe auf die Datenbank bekommen die Webhooks nichts mit, die Ereignisse gehen auf den Doctrine layer

Es wird solange versucht bis empfänger zurückgibt dass er nachricht empfangen
Hinterlegen eines retry algorithm

Im Unterschied zum API wollen wir wissen, was mit den Daten passiert, bei WEbhook ist egal





## Constraints

- Data that can be sent via the *Webhook* module, must follow the Actindo data models and is restricted to them. 
- Since the events are processed in the doctrine layer, a layer between the code and the databases, direct database accesses cannot be processed.

