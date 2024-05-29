# Key features

- Combination with execution workers    
    Each Actindo webhook is given how it should be processed. It is a combination of itself with an execution worker, which defines how the webhooks are to be sent. The webhook defines the recipient and the data that should trigger the events, the execution worker identifies the affected webhooks in the queue. 

- Definition of retries   
    If the recipient is currently down or other situations prevent a webhook from being successfully sent: It will be retried as many times you have specified in the execution workers until the recipient confirms receiving the message.

- Conditions    
    You can strictly narrow the circumstances under which a webhook message is to be sent, for example, a stock level change should trigger the sending of a message. There is no need to request to receive messages, the message will be sent immediately, as soon as the described change has been made to an entity.  

- Using of DataHub properties  
    Because you can go through the DataHub and customize attribute sets, you can quickly add attributes that you want to have in addition to the others, which is much more flexible than an API that is restricted to a specific module entity. If you have customer-specific DataHub entities that should trigger an event, you can add them to the webhook definition.

- Authentication   
    You can optionally use an authentication, whereby you can choose between xxxx or a secret key (standard hash algorithm **sha265**).    

<!---Webhooks für singuläre Entitäten fokussiert, zum Beispiel, wenn es zu Entitäten änderungen gibt


Die kunden müssen sich keine Exporte mehr bauen, um Daten aus dem System herauszuholen und können selber entscheiden, was sie mit den Daten machen wollen Kunden können eigentständig andere Third party einbinden.

Warum nicht über API?
weniger Aufwand, keine Authentifizierung, nicht jedes mal einen Request machen, um Daten abzuholen: Webhooks schicken die message, sobald sich etwas geändert hat und muss nicht auf Request warten

Aktuell dafür genutzt - direkter Draht zum Shopsystem -> orderstatusänderungen, bestandsänderungen

Wofür es sich eignet, muss man genau überlegen, wo die Vorteile der Webhooks greifen -> zum Beispiel für reports würde es sich eher anbieten, über den DataHub exporter zu gehen. Webhooks liefern immer nur eine singuläre Änderung, nicht für große Datenmengen gedacht

GANZ WICHTIGER PUNKT Da man über DataHub gehen kann und Attributssets anpassen kann, kann man schnell Attribute hinzufügen, die man noch haben möchte und ist dadurch gegen ein API viel flexibler


    Zurzeit optimal für Channels properties
Direktzugriffe auf die Datenbank bekommen die Webhooks nichts mit, die Ereignisse gehen auf den Doctrine layer

Es wird solange versucht bis empfänger zurückgibt dass er nachricht empfangen
Hinterlegen eines retry algorithm

Im Unterschied zum API wollen wir wissen, was mit den Daten passiert, bei WEbhook ist egal-->


## Constraints

- Data that can be sent via the *Webhook* module must follow the Actindo data models and is restricted to them. 
- Since the events are processed in the doctrine layer, a layer between the code and the databases, direct database accesses cannot be processed.
- Webhooks are not suitable for large data volumes such as order statistics, but very flexible for sending messages containing single changes.

