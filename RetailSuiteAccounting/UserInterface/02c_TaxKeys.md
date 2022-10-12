# Tax keys

*Accounting > Settings > Tab TAX KEYS*

![Tax keys](../../Assets/Screenshots/RetailSuiteAccounting/Settings/TaxKeys/CreateTaxKey.png "[Tax keys]")

The list displays all available tax keys. All fields are read-only.

- *No.*  
  Tax key number.

- *I*  
  Indication of change. An **I** is displayed if the tax key has been manually created or edited by the user.

- *From*  
  Validity start date of the tax key.

- *To*  
  Validity end date of the tax key.  

- *%*  
  Applicable tax rate.

- *+/-*  
  Gross/net indication. If the posting is a gross amount, the tax must be deducted from it, and therefore a minus sign is displayed. If the posting is a net amount, the tax must be added to it, and therefore a plus sign is displayed.

- *Factor*  
  Factor applicable to the selected tax rate.

- *VAT*  
  Account where the VAT is to be posted.

- *Input tax*  
  Account where the input tax is to be posted.

- *VAT not due*  
  Account where the VAT not due is to be posted.

- *Type*  
  Abbreviation of the tax type configured for the tax key. The following options are available:  
  - Empty     
    No tax type is configured for the tax key.
  - **I**   
    The input tax is configured for the tax key.
  - **V**   
    The VAT is configured for the tax key.
  - **IV**   
    The input tax and the VAT are configured for the tax key.


[comment]: <> (Abkürzungen im System nicht übersetzt. Auf DE lassen? Wenn ja, durchgängig, also, auch in Integration und Operation)

- *Country*  
  Two-letter country code. The alpha-2 codes according to ISO 3166-1 are used, see [List of country codes](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).

- *Description*  
  Descriptive tax key name.


The input fields below allow to create, edit or delete tax keys. For detailed information about creating, editing or deleting tax keys, see [Manage the tax keys](../Integration/02_ManageTaxKeys.md).

- *Key*  
  Enter or modify the tax key.

- *Description*  
  Enter or modify a descriptive tax key name.

- *Valid from*   
  Enter or modify the tax key validity start date.

- *to*  
  Enter or modify the tax key validity end date.

- *Tax type*  
  Click the drop-down list to select the appropriate tax type for the tax key. The tax type determines how the tax paid or collected in relation to the tax key is to be registered in the system. The following options are available:
  - **( ) Not specified**  
    No tax type is configured for the tax key.  
  - **(I) Input tax**  
    The input tax is configured for the tax key.
  - **(V) VAT**  
    The VAT is configured for the tax key.
  - **(IV) Input tax and VAT**  
    The input tax and the VAT are configured for the tax key.


- *Percent / factor*  
  Enter the applicable tax rate in the first field and the corresponding factor in the second field. Click the drop-down list between the fields to select the applicable gross or net option. The following options are available:
  - **+**   
    The posting is a gross amount.
  - **-**   
    The posting is a net amount.


- *Accounts (VAT/input tax/VAT not due)*  
  Enter the account numbers of the accounts to which the applicable tax amounts are to be posted. Enter the account number for the VAT in the first field, the account number for the input tax in the second field and the VAT not due in the third field.

- *VAT ID needed*  
  Click the drop-down list to select the appropriate option. A VAT ID is needed for all transactions that involve companies. The following options are available:
  - **Yes**   
    The transaction involves companies. The VAT ID is needed.
  - **No**   
    The transaction involves only private individuals. No VAT ID is needed.


- *Country*  
  Click the drop-down list to select the applicable EU country. All European countries are displayed in the list. If no European country is to be selected, select the **No EU tax key** option.


- [SAVE & NEW]  
  Click this button to save a new tax key. The button is locked if a tax key has been selected. For detailed information about creating a tax key, see [Create a tax key](../Integration/02_ManageTaxKeys.md#create-a-tax-key).

- [SAVE]  
  Click this button to save any changes made to the selected tax key. The button is only unlocked if a tax key has been selected. For detailed information about editing a tax key, see [Edit a tax key](../Integration/02_ManageTaxKeys.md#edit-a-tax-key).

  > [Info] Be aware that all saved changes will overwrite the existing tax key data.

- [DELETE]  
  Click this button to delete the selected tax key. The button is only unlocked if an account has been selected. For detailed information, see [Delete a tax key](../Integration/02_ManageTaxKeys.md#delete-a-tax-key).

  > [Warning] **Loss of data**   
  Deleting will permanently remove the selected data. The deletion cannot be undone and the deleted data cannot be restored.       
  Problems may occur due to unresolved dependencies.   
  Make sure you really want to delete the selected data.

- [CLEAR]  
  Click this button to clear all fields.

- [HELP]  
  This function is currently not available.

- [RESTORE]  
  Click this button to restore the tax keys to their original state.

[comment]: <> (Was macht der WIEDERHERSTELLEN/RESTORE Button? Beim Klicken, Fenster mit Warnung "Möchten Sie die Steuerschlüssel in deren Ursprungs-Zustand zurückversetzen? Alle von Ihnen gemachten Änderungen werden dadurch gelöscht." Bei OK scheint es aber nichts zu passieren... Das System leert die Eingabemaske, aber nach Speichern kann man nicht wiederherstellen.)
