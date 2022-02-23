[!!Accounting](Actindo/Accounting)

# Manage the accounts

The accounts are set up during the configuration process via the accounting wizard, see [Charts of accounts](01_RunAccountingWizard.md#chart-of-accounts). However, you can create, edit or delete an account if necessary in the *Accounting* module, for example if a specific account is not yet available in the system or the settings of an existing one need to be adjusted.

> [Warning] Any modifications in the accounts have far-reaching consequences for the *Accounting* module and the system automatic bookings. It is highly recommended not to make any changes in the accounts, unless you have an in-depth knowledge of their functions. In case of doubt, contact our support team.

## Prerequisites

- The accounting is configured via the configuration wizard, see [Run the Accounting Wizard](01_RunAccountingWizard.md).
- A valid fiscal year is created, see [Manage the fiscal year](04_ManageFiscalYear.md).

## Procedure

*Accounting > Settings > Accounts*

![Accounts](/Assets/Screenshots/Accounting/Settings/Accounts/Accounts.png "[Accounts]")

> [Note] The buttons [SAVE] and [SAVE & NEW] have different functions and exclude each other. For this reason, they are not activated simultaneously.

### Create an account


[comment]: <> (Inhalt genommen aus VenduoPOS/Integration/02_ManageAccounts.md -> Ist das OK? Problem mit Copy/Paste. Überschneiden sie sich oder ist es einfach das gleiche? -> Wenn das gleiche, besser Verweis?)

[comment]: <> (Frage Screenshot Konten02: nicht alle Felder beschrieben, z.B. Gültig von - bis. Nur das "Notwendigste" beschreiben? Wie wissen wir/der Kunde, ob alle Felder notig/pflichtig sind oder nicht?)

[comment]: <> (Vorwarnen über LEEREN -falls Sie aus Versehen irgendwo clicken- SAVE/SAVE&NEW/DELETE? S. VenduoPOS/Integration/02_ManageAccounts -> Dort anders gelost: [Check the account availability](#check-the-account-availability))


1. Enter an available account number in the field *Account number*.

2. Enter an account name in the field *Account name*.
[comment]: <> (Description?)

3. Select a tax type for the account in the drop-down list *Tax type*.

4. Select the corresponding function for the account in the drop-down list *Function* .   
  For detailed information, see [User Interface Accounting](/Accounting/UserInterface/00_UserInterface.md).

5. Click the button [SAVE & NEW].   
  The new account is displayed in the account list.


### Edit an account

1. Select the corresponding number range in the drop-down list *Account class* .   
  All accounts of the selected account class are displayed in the list.

2. Select the account to be edited.

3. Edit the settings as necessary.

4. Click the button [SAVE].   
The account has been edited. The edited account is displayed in the list.

[comment]: <> (Vorwarnen??? Hier ist es zu spät!)
   > [Warning] Be aware that the existing account will be then overwritten, that means, that the existing account will be completely replaced by the edited one.


### Delete an account

1. Select the account to be deleted.

2. Click the button [DELETE].  
The selected account will be deleted.

    > [Warning] Be aware that the existing tax key will be deleted permanently.

### Next steps

- [Manage the fiscal year](04_ManageFiscalYear.md)
- [Manage the customer/supplier](05_ManageCustomerSupplier.md)
- [Manage the fixed bookings](06_ManageFixedBookings.md)
- [Manage the BWA reports](07_ManageBWAReports.md)

### See also

- [Invoicing / Turnover treshold activation](#headingID)
- [Leistungsarten / Steuersätze / Steuerklasse](#headingID)
