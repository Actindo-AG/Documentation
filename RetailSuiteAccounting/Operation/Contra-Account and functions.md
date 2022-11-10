
# Contra-Account and special functions

It is possible to prepend keys for special functions in front of the Contra-Account while creating manual postings, split postings, etc.

These BU-keys (also called "BU-Schlüssel" in the DATEV Software), consist of 2 digits called correction key (1st digit from the left) and tax key (2nd digit from the left).

Example:
* Entering "20" in front of the contra account means: correction key "2" and tax key "0"
* Entering "22" in front of the contra account means: correction key "2" and tax key "2" 
* Entering "02" or simly "2" in front of the contra account means: correction key not set, tax key "2"

> [Info] The BU-key must be entered in front of the contra account filled to the max number of digits. 
>
> * If you have 5-digit personal accounts the correct entry of the BU "29" (meaning see below) for the account 4530 would be <b>29</b>0<b>4530</b>
> * If you have 7-digit personal accounts the correct entry of the BU "29" (meaning see below) for the account 4530 would be <b>29</b>000<b>4530</b>

> [Info] The BU-key can only be entered in the contra account. If you want to post the account in debit you need to enter the posting amount *negative* 

## Correction key

Correction keys are used to cancel postings, create postings for EU transactions or postings with individual tax keys longer than 1 digit.

## Tax key

Tax keys are used to create postings with single-digit tax keys like input VAT (Vorsteuer) 

## Meaning of the BU keys
<table>
    <tr>
        <th>Number</th>
        <th>Meaning</th>
        <th>Explanation</th>
    </tr>
    <tr>
        <td>0 / empty</td>
        <td>ohne Stornoschlüssel</td>
        <td>Dieser Stornoschlüssel wird verwendet, wenn kein Stornoschlüssel angegeben wurde. Hier ist die Bedeutung der Steuerschlüssel wie folgt:

* 0: Keine Verbuchung von Steuer
* 1: keine Bedeutung
* 2: Umsatzsteuer ermäßigter Satz (7%)
* 3: Umsatzsteuer normaler Satz (19%)
* 5: Umsatzsteuer alter Normalsatz (16%)
* 7: Abzuziehende Vorsteuer alter Normalsatz (16%)
* 8: Abzuziehende Vorsteuer ermäßigter Satz (7%)
* 9: Abzuziehende Vorsteuer normaler Satz (19%)
</td>
    </tr>
    <tr>
        <td>1</td>
        <td>EG-Buchung</td>
        <td>Der Stornoschlüssel 1 löst zusammen mit einem Steuerschlüssel eine EG-Buchung aus. Die Steuerschlüssel haben in diesem Fall folgende Bedeutung:

* 0: Im anderen EG-Land steuerpflichtige Lieferung/Leistung
* 1: Steuerfreie EG-Lieferung
* 2: Im Inland steuerpflichtige EG-Lieferungen ermäßigter Satz (7%)
* 3: Im Inland steuerpflichtige EG-Lieferungen normaler Satz (19%)
* 5: Im Inland steuerpflichtige EG-Lieferungen alter Normalsatz (16%)
* 7: Steuerpflichtige innergemeinschaftliche Erwerbe alter Normalsatz (16%)
* 8: Steuerpflichtige innergemeinschaftliche Erwerbe ermäßigter Satz (7%)
* 9: Steuerpflichtige innergemeinschaftliche Erwerbe normaler Satz (19%)
</td>
    </tr>
    <tr>
        <td>2</td>
        <td>Generalumkehr</td>
        <td>Die Stornierung einer „normalen" Buchung erfolgt durch Eintrag der Ziffer 2 im ersten Feld des Gegenkontos. Der Umsatz wird mit umgekehrtem Vorzeichen eingegeben. Die hierdurch entstehende Buchung neutralisiert die angeklickte Buchung, ohne dass diese gelöscht wird.</td>
    </tr>
    <tr>
        <td>3</td>
        <td>Generalumkehr bei aufzuteilender Vorsteuer</td>
        <td>Der Stornoschlüssel 3 dient zur Aufhebung von Buchungen, die mit dem Stornoschlüssel 9 eingegeben wurden.</td>
    </tr>
    <tr>
        <td>4</td>
        <td>Aufhebung der Automatik</td>
        <td>Durch die Eingabe des Stornoschlüssels 4 wird die automatische „Heraus-Rechnung" von Vorsteuer oder Umsatzsteuer gesperrt. Auch Sammelkonten können durch die Eingabe des Steuerschlüssels 4 bebucht werden.</td>
    </tr>
    <tr>
        <td>5</td>
        <td>Individueller Steuerschlüssel</td>
        <td>Der Stornoschlüssel 5 bereitet die Eingabe mehrstelliger Steuerschlüssel vor. Hierzu öffnet sich direkt beim Verlassen des Feldes „GegKonto" ein Fenster.</td>
    </tr>
    <tr>
        <td>6</td>
        <td>Generalumkehr bei Schlüssel 1 - EG-Buchung</td>
        <td>Der Stornoschlüssel 6 dient zur Aufhebung von Buchungen, die mit dem Stornoschlüssel 1 eingegeben wurden. Hier muss natürlich der Ursprüngliche Steuerschlüssel mit angegeben werden.</td>
    </tr>
    <tr>
        <td>7</td>
        <td>Generalumkehr bei Schlüssel 5 -  Individuellem Steuerschlüssel</td>
        <td></td>
    </tr>
    <tr>
        <td>8</td>
        <td>Generalumkehr bei Schlüssel 4 - Aufhebung der Buchungsautomatik</td>
        <td>Der Stornoschlüssel 8 dient zur Aufhebung von Buchungen, die mit dem Stornoschlüssel 4 eingegeben wurden.</td>
    </tr>
    <tr>
        <td>9</td>
        <td>Aufzuteilende Vorsteuer</td>
        <td>Der Stornoschlüssel 9 löst zusammen mit den Steuerschlüsseln 6 - 9 eine Verbuchung der Vorsteuer auf die Konten für aufzuteilende Vorsteuer aus (anstatt auf die Konten für abzuziehende Vorsteuer).</td>
    </tr>
</table>
