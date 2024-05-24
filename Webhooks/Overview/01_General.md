# General

Webhooks are an easy way to send data to recipients. With Actindo's *Webhooks* module, you cannot only define explicitly the data to be transferred, but also the events that trigger the sending of webhooks messages, as well as the way in which the data is to be sent.


Webhooks für singuläre Entitäten fokussiert, zum Beispiel, wenn es zu Entitäten änderungen gibt

Mit geringem Aufwand mit Partnern zusammenarbeiten -> Empfänger der messages können damit machen, was sie möchten
Verbindung benötigt keine Actindo-seitige Konfiguration -> so dass Aufwand für die Erstellung von kunden-spezifischen APIs entfällt

Actindo ist nicht merh der Einzige der eine Implementierung machen kann

Die kunden müssen sich keine Exporte mehr bauen, um Daten aus dem System herauszuholen und können selber entscheiden, was sie mit den Daten machen wollen Kunden können eigentständig andere Third party einbinden.

Warum nicht über API?
weniger Aufwand, keine Authentifizierung, nicht jedes mal einen Request machen, um Daten abzuholen: Webhooks schicken die message, sobald sich etwas geändert hat und muss nicht auf Request warten

Aktuell dafür genutzt - direkter Draht zum Shopsystem -> orderstatusänderungen, bestandsänderungen

Wofür es sich eignet, muss man genau überlegen, wo die Vorteile der Webhooks greifen -> zum Beispiel für reports würde es sich eher anbieten, über den DataHub exporter zu gehen. Webhooks liefern immer nur eine singuläre Änderung, nicht für große Datenmengen gedacht

GANZ WICHTIGER PUNKT Da man über DataHub gehen kann und Attributssets anpassen kann, kann man schnell Attribute hinzufügen, die man noch haben möchte und ist dadurch gegen ein API viel flexibler


Events that are not triggered by a request from your side, for example when a shopper initiated a chargeback, or when a new report becomes available (Adyen).

Receive important updates related to your account (Adyen).



## Benefits

- Specify what and how to transfer data for each recipient
- Optional authentication
- Webhooks for sequential or parallel processing


## Further information
Refer to our [Actindo Core1 Platform](../../Core1Platform/BasicPhilosophy/01_General.md) documentation for information on general features and functions, standard buttons, UI elements, and how to use the Actindo documentation.