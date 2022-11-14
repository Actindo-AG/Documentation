[!!Create a manual posting](../Operation/04_CreateManualBooking.md)
[!!Cancel a posting](../Operation/05_CancelBooking.md)
[!!Split a posting](../Operation/09_SplitBooking.md)
[!!Review an account](../Operation/02_ReviewAccount.md)

# Contra account and special functions

It is possible to prepend keys for special functions in front of the contra account while carrying out certain operations, such as create manual postings or split postings.

These BU-keys (also called "BU-Schlüssel" or "Buchungsschlüssel", German for posting key, in the DATEV software) consist of 2 digits: the correction key (first digit from the left) and the tax key (second digit from the left).

A few examples of BU-keys:
  - Entering **20** in front of the contra account means: correction key **2** and tax key **0**
  - Entering **22** in front of the contra account means: correction key **2** and tax key **2**
  - Entering **02**, or simply **2** in front of the contra account means: correction key not set, tax key **2**

> [Info] The BU-key must be entered in front of the contra account filled to the maximal number of digits according to the account settings.
>
> - If you have 5-digit personal accounts, the correct entry of the BU "29" for the account 4530 would be **29**0**4530**.
> - If you have 7-digit personal accounts, the correct entry of the BU "29" for the account 4530 would be **29**000**4530**.
>
> For detailed information about the BU-keys meaning, see [Meaning of the BU keys](#meaning-of-the-bu-keys). The BU-key can only be entered in the contra account. If you want to post the account in debit, you need to enter a negative posting amount.

[comment]: <> (Als normaler Text, nicht Info? Als Info von Patrick hinzugefügt)

## Correction key

Correction keys are used to cancel postings, create postings for EU transactions or postings with individual tax keys longer than 1 digit.

## Tax key

Tax keys are used to create postings with single-digit tax keys like input VAT.

## Meaning of the BU keys

> [Info] The tax rates specified below are only valid in Germany.

| Number      | Meaning     | Explanation |
|-------------|-------------|-------------|
| 0 / empty | without cancellation key | This cancellation key is used when no other cancellation key has been specified. The meaning of the tax key is defined as follows: <br> <br> &bull; 0: No tax posting <br> &bull; 1: No meaning <br> &bull; 2: Reduced VAT rate (7%) <br> &bull; 3: Standard VAT rate (19%) <br> &bull; 5: Old standard VAT rate (16%) <br> &bull; 7: Old standard deductible input tax rate (16%) <br> &bull; 8: Reduced deductible input tax rate (7%) <br> &bull; 9: Standard deductible input tax rate (19%)|
| 1 |EU posting| The cancellation key 1, together with a tax key, triggers a EU posting. In this case, the tax keys have the following meaning: <br> <br> &bull; 0: Supply of goods/services taxable in another EU country <br> &bull; 1: Tax-free intra-EU supply of goods <br> &bull; 2: Im Inland steuerpflichtige EG-Lieferungen ermäßigter Satz (7%) <br> &bull; 3: Im Inland steuerpflichtige EG-Lieferungen normaler Satz (19%) <br> &bull; 5: Im Inland steuerpflichtige EG-Lieferungen alter Normalsatz (16%) <br> &bull; 7: Steuerpflichtige innergemeinschaftliche Erwerbe alter Normalsatz (16%) <br> &bull; 8: Steuerpflichtige innergemeinschaftliche Erwerbe ermäßigter Satz (7%) <br> &bull; 9: Steuerpflichtige innergemeinschaftliche Erwerbe normaler Satz (19%)|
|2|Generalumkehr|Die Stornierung einer „normalen" Buchung erfolgt durch Eintrag der Ziffer 2 im ersten Feld des Gegenkontos. Der Umsatz wird mit umgekehrtem Vorzeichen eingegeben. Die hierdurch entstehende Buchung neutralisiert die angeklickte Buchung, ohne dass diese gelöscht wird.|
|3|Generalumkehr bei aufzuteilender Vorsteuer|Der Stornoschlüssel 3 dient zur Aufhebung von Buchungen, die mit dem Stornoschlüssel 9 eingegeben wurden.|
|4|Aufhebung der Automatik|Durch die Eingabe des Stornoschlüssels 4 wird die automatische „Heraus-Rechnung" von Vorsteuer oder Umsatzsteuer gesperrt. Auch Sammelkonten können durch die Eingabe des Steuerschlüssels 4 bebucht werden.|
|5|Individueller Steuerschlüssel|Der Stornoschlüssel 5 bereitet die Eingabe mehrstelliger Steuerschlüssel vor. Hierzu öffnet sich direkt beim Verlassen des Feldes „GegKonto" ein Fenster.|
|6|Generalumkehr bei Schlüssel 1 - EG-Buchung|Der Stornoschlüssel 6 dient zur Aufhebung von Buchungen, die mit dem Stornoschlüssel 1 eingegeben wurden. Hier muss natürlich der Ursprüngliche Steuerschlüssel mit angegeben werden.|
|7|Generalumkehr bei Schlüssel 5 - Individuellem Steuerschlüssel|-|
|8|Generalumkehr bei Schlüssel 4 - Aufhebung der Buchungsautomatik|Der Stornoschlüssel 8 dient zur Aufhebung von Buchungen, die mit dem Stornoschlüssel 4 eingegeben wurden.|
|9|Aufzuteilende Vorsteuer|Der Stornoschlüssel 9 löst zusammen mit den Steuerschlüsseln 6 - 9 eine Verbuchung der Vorsteuer auf die Konten für aufzuteilende Vorsteuer aus (anstatt auf die Konten für abzuziehende Vorsteuer).|
