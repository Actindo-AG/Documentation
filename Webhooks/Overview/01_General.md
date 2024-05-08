# General

daten an einen Endpunkt beim Kunden schicken, was der Kunde damit macht, ist uns egal

Die Daten, die über WEbhook modul geschickt werden können, folgen den Actindo Datenmodelle

In den Webhooks selbst ist schon der empfänger des Webhhooks vermerkt

Es wird solange versucht bis empfänger zurückgibt dass er nachricht empfangen
Hinterlegen eines retry algorithm

Im Unterschied zum API wollen wir wissen, was mit den Daten passiert, bei WEbhook ist egal

optional eine Authentifizierung
wenn man nicht möchte, kann man auch NOAuth als typ Auswählen
Wenn Empfänger keine Autorisierung bauen möchte, geht es auch mit Secret key (standard hash algorithmus sha256)

man kann conditions angeben, so dass eng eingegrenzt werden kann, unter welchen Umständen webhook gesendet werden soll,z.B. nur wenn sich ein Lagerbestand geändert hat.

DataHub properties werden standardmäßig nicht mitgeliefert, ich kann aaberin optional properties angeben, so dass diese Daten mitgeliefert werden.

Jedem Webhook wird mitgegeben, wie es verarbeitet werden solle (worker wird zugeordnet)

Events that are not triggered by a request from your side, for example when a shopper initiated a chargeback, or when a new report becomes available (Adyen).

Receive important updates related to your account (Adyen).

Bis 25:00

## Benefits


## Further information
Refer to our [Actindo Core1 Platform](../../Core1Platform/BasicPhilosophy/01_General.md) documentation for information on general features and functions, standard buttons, UI elements, and how to use the Actindo documentation.