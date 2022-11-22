[!!Create a manual posting](../Operation/04_CreateManualBooking.md)
[!!Cancel a posting](../Operation/05_CancelBooking.md)
[!!Split a posting](../Operation/09_SplitBooking.md)
[!!Manage the tax keys](../Integration/02_ManageTaxKeys.md)
[!!Manage the accounts](../Integration/03_ManageAccounts.md)


# Contra account and special functions

It is possible to prepend keys for special functions in front of the contra account while carrying out certain operations, such as create manual postings or split postings.

These BU keys (also called "BU-Schlüssel" or "Buchungsschlüssel", German for posting key, in the DATEV software) consist of 2 digits: the correction key (first digit from the left) and the tax key (second digit from the left).

Correction keys are used to cancel postings, create postings for EU transactions or postings with customized tax keys longer than 1 digit.   
Tax keys are used to create postings with single-digit tax keys, like input VAT.

For example:
  - Entering **20** in front of the contra account means: correction key **2** and tax key **0**
  - Entering **22** in front of the contra account means: correction key **2** and tax key **2**
  - Entering **02**, or simply **2** in front of the contra account means: correction key not set, tax key **2**

The BU key must be entered in front of the contra account, which must be filled to the maximal number of digits defined in the account settings. For example:

- If you have 5-digit personal accounts, the correct entry of the BU key "29" for the account 4530 would be **29**0**4530**.
- If you have 7-digit personal accounts, the correct entry of the BU key "29" for the account 4530 would be **29**000**4530**.

The BU key can only be entered in the contra account. If you want to post the account in debit, you need to enter a negative posting amount. For detailed information about the meaning of the BU keys, see [Meaning of the BU keys](#meaning-of-the-bu-keys).


## Meaning of the BU keys

The tax rates specified below are the ones applicable in Germany.

| Number      | Meaning     | Explanation |
|-------------|-------------|-------------|
| 0 / empty | Without cancellation key | This cancellation key is used when no cancellation key has been specified. The meaning of the tax key is as follows: <br> &bull; 0: No tax posting <br> &bull; 1: No meaning <br> &bull; 2: Reduced VAT rate (7%) <br> &bull; 3: Standard VAT rate (19%) <br> &bull; 5: Old standard VAT rate (16%) <br> &bull; 7: Old standard deductible input tax rate (16%) <br> &bull; 8: Reduced deductible input tax rate (7%) <br> &bull; 9: Standard deductible input tax rate (19%)|
| 1 | EU posting | The cancellation key **1** triggers, together with a tax key, an EU posting. In this case, the tax keys have the following meaning: <br> &bull; 0: Supply of goods/services taxable in another EU country <br> &bull; 1: Tax-free supply of goods within the EU <br> &bull; 2: Reduced VAT rate for domestic taxable supplies of goods within the EU (7%) <br> &bull; 3: Standard VAT rate for domestic taxable supplies of goods within the EU (19%) <br> &bull; 5: Old standard VAT rate for domestic taxable supplies of goods within the EU (16%) <br> &bull; 7: Old standard VAT rate for intra-community taxable acquisitions of goods (16%) <br> &bull; 8: Reduced VAT rate for intra-community taxable acquisitions of goods (7%) <br> &bull; 9: Standard VAT rate for intra-community taxable acquisitions of goods (19%)|
| 2 | General reversal | The cancellation of a posting is performed by entering the number **2** in the first digit of the contra account. The turnover is then entered with the reversed sign. The resulting posting cancels the selected posting without deleting it.|
| 3 | General reversal with distributable input tax | The cancellation key **3** is used to cancel postings that have been entered with the cancellation key **9**.|
| 4 | Cancellation of automatic function | By entering the cancellation key **4**, the automatic deduction of input tax or VAT is blocked. Besides, collective accounts can also be posted to by entering the tax key **4**.|
| 5 | Individual tax key | The cancellation key **5** allows to enter multi-digit tax keys. For this purpose, a window is displayed when leaving the *Contra account* field. |
| 6 | General reversal with key **1** - EU-posting | The cancellation key **6** is used to cancel postings that have been entered with the cancellation key **1**. In this case, the original tax key must be specified as well.|
| 7 | General reversal with key **5** - Individual tax key | The cancellation key **7** is used to cancel postings that have been entered with the cancellation key **5**.|
| 8 | General reversal with key **4** - Cancellation of the posting automatic function | The cancellation key **8** is used to cancel postings that have been entered with the cancellation key **4**.|
| 9 | Distributable input tax | The cancellation key 9 triggers, together with the tax keys 6 to 9, a posting of the input tax to the accounts for distributable input tax (instead of to the accounts for deductible input tax).|

[comment]: <> (Termfrage: Individual key oder customized/personalized key? Fehlende Info in Zeile 7 aus alter Doku genommen: https://www.actindo.com/de/doku/app-hilfe/handbuch/retailsuiteaccounting/latest/Grundlagen/Grundlagen.html Kurz getestet, scheint bei mir nicht zu funktionieren)
