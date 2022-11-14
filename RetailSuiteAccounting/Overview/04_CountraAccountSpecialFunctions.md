[!!Create a manual posting](../Operation/04_CreateManualBooking.md)
[!!Cancel a posting](../Operation/05_CancelBooking.md)
[!!Split a posting](../Operation/09_SplitBooking.md)
[!!Manage the tax keys](../Integration/02_ManageTaxKeys.md)
[!!Manage the accounts](../Integration/03_ManageAccounts.md)


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

Correction keys are used to cancel postings, create postings for EU transactions or postings with customized tax keys longer than 1 digit.

## Tax key

Tax keys are used to create postings with single-digit tax keys like input VAT.

## Meaning of the BU keys

> [Info] The tax rates specified below are only valid in Germany.

| Number      | Meaning     | Explanation |
|-------------|-------------|-------------|
| 0 / empty | without cancellation key | This cancellation key is used when no other cancellation key has been specified. The meaning of the tax key is defined as follows: <br> <br> &bull; 0: No tax posting <br> &bull; 1: No meaning <br> &bull; 2: Reduced VAT rate (7%) <br> &bull; 3: Standard VAT rate (19%) <br> &bull; 5: Old standard VAT rate (16%) <br> &bull; 7: Old standard deductible input tax rate (16%) <br> &bull; 8: Reduced deductible input tax rate (7%) <br> &bull; 9: Standard deductible input tax rate (19%)|
| 1 | EU posting | The cancellation key 1, together with a tax key, triggers a EU posting. In this case, the tax keys have the following meaning: <br> <br> &bull; 0: Supply of goods/services taxable in another EU country <br> &bull; 1: Tax-free EU supply of goods within the EU <br> &bull; 2: Supplies of goods taxable in Germany reduced VAT rate (7%) <br> &bull; 3: Supplies of goods taxable in Germany standard VAT rate (19%) <br> &bull; 5: Supplies of goods taxable in Germany old standard VAT rate (16%) <br> &bull; 7: Intra-community taxable acquisitions of goods old standard VAT rate (16%) <br> &bull; 8: Intra-community taxable acquisitions of goods standard VAT rate (7%) <br> &bull; 9: Intra-community taxable acquisitions of goods standard VAT rate (19%)|
| 2 | General reversal | The cancellation of a "normal" posting is performed by entering the number 2 in the first digit of the contra account. The turnover is then input with the reversed sign. The resulting posting cancels the selected posting without deleting it.|
| 3 | General reversal with input tax distribution | The cancellation key 3 is used to cancel postings that were originally entered with the cancellation key 9.|
| 4 | Cancellation of automatic function | By entering the cancellation key 4, the automatic deducting of input tax or VAT is blocked. Besides, collective accounts can also be posted to by entering the tax key 4.|
| 5 | Individual tax key | The cancellation key 5 offers the possibility to enter multi-digit tax keys. For this purpose, a window opens directly after leaving the field "Contra account". |
| 6 | General reversal with key 1 - EU-posting | The cancellation key 6 is used to cancel postings that were originally entered with the tax key 1. The original tax key must be specified in this case too.|
| 7 | General reversal with key 5 - Specific tax key |-|
| 8 | General reversal with key 4 - Cancellation of the posting automatic function | The cancellation key 8 is used to cancel postings that were originally entered with the tax key 4.|
| 9 | Input tax distribution | The tax key 9, together with the tax keys 6 to 9, triggers a posting of the input tax to the accounts for input tax distribution (instead of the accounts for input tax deduction).|
