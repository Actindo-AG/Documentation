[!!Manage the fixed postings](../Integration/06_ManageFixedBookings.md)

# Fixed posting

*Accounting > Settings > Tab FIXED POSTINGS*

![Fixed posting](../../Assets/Screenshots/RetailSuiteAccounting/Settings/FixedBookings/CreateFixedBookingBatch.png "[Fixed posting]")

- *Fixed posting batch*  
    Click the drop-down list to select a fixed posting batch. The selected batch is displayed in the *Fixed postings &ndash; Batch "Batch name"* window.   
    Click the **New batch** option in the drop-down list to create a new batch. The *Name* field is displayed below the drop-down list. By default, the **New batch** option is preselected.    
    For detailed information about creating a new batch, see [Create a fixed posting batch](../Integration/06_ManageFixedBookings.md#create-a-fixed-posting-batch).

- *Name*  
    Enter a batch name. This field is only displayed when the *New batch* option is selected in the *Fixed posting batch* drop-down list.

- [DELETE]  
    Click this button to delete the selected fixed posting batch.    
    For detailed information about deleting a new batch, see [Delete a fixed posting batch](../Integration/06_ManageFixedBookings.md#delete-a-fixed-posting-batch).

- [CREATE]  
    Click this button to create a fixed posting batch. The *Fixed postings &ndash; Batch "Batch name"* window is displayed, see [Fixed postings &ndash; Batch "Batch name"](#fixed-postings-–-batch).

- [EDIT]  
    Click this button to edit a fixed posting batch. The *Fixed postings &ndash; Batch "Batch name"* window is displayed, see [Fixed postings &ndash; Batch "Batch name"](#fixed-postings-–-batch).


## Fixed postings &ndash; Batch

*Accounting > Settings > Tab FIXED POSTINGS > Select batch*

![Fixed posting batch](../../Assets/Screenshots/RetailSuiteAccounting/Settings/FixedBookings/FixedBookingBatch.png "[Fixed posting batch]")

The list displays all fixed postings to the selected batch. All fields are read-only.    

- *Seq. no.*  
    Sequential number of the posting. The posting numbers are added by the system automatically.

- *PP*  
    Posting period. This value is set to **00** by default.  

    > [Info] The fixed postings can be added to a specific posting period when selecting the fiscal year, see [Select the fiscal year](../Operation/01_SelectFiscalYear.md).

- *Jnl*  
    Journal. This value is set to **00** by default.  

    > [Info] The fixed postings can be added to a specific journal when selecting the fiscal year, see [Select the fiscal year](../Operation/01_SelectFiscalYear.md).

- *Turnover*  
    Posting turnover value.  

- *Contra account*  
    Contra account number.

- *Receipt1*  
    Invoice number.

- *Receipt2*  
    Other reference number.

- *Date*  
    Posting date.

- *Account*  
    Account number.

- *Cost1*  
    Cost center number.

- *Cost2*  
    Cost object number.

- *Text*  
    Posting reference text.

- *AMOUNT*  
    Fixed posting batch total amount.

- *Amount*  
    Fixed posting batch total amount.

[comment]: <> (FH/Fachreviewer: Unterschied zwischen AMOUNT und Amount?)


The input fields allow to create, edit and delete fixed postings. Click a fixed posting in the list to display its details in the input fields and edit or delete it. Clear the input fields to add a new fixed posting.

- *Seq. no.*    
    Leave this field empty. The sequential posting number is added by the system automatically.

- *Turnover*  
    Enter the turnover value.

- *Contra account*  
    Enter the contra account number. This field is mandatory.

    > [Info] After you have entered at least two numbers in the field, a list is displayed below the field with all accounts matching the entry. You can select the corresponding account in the list.

- *Receipt1*  
    Enter an appropriate reference number, such as the invoice number.

- *Receipt2*  
    Enter any other appropriate reference number, such as order number.

- *Date*  
    Enter the date for the fixed posting. The valid date format is DDMMYY. This field is mandatory.

- *Account*  
    Enter the account number. This field is mandatory.  

    > [Info] After you have entered at least two numbers in the field, a list is displayed below the field with all accounts matching the entry. You can select the corresponding account in the list.

- *Cost1*  
    Enter a cost center number.

- *Cost2*  
    Enter a cost object number.

- *Text*  
    Enter a reference text.  


- [POST]  
    Click this button to add a new fixed posting to the batch or edit the selected fixed posting.   
    For detailed information about adding or editing a fixed posting, see [Add a fixed posting](../Integration/06_ManageFixedBookings.md#add-a-fixed-posting) and [Edit a fixed posting](../Integration/06_ManageFixedBookings.md#edit-a-fixed-posting).

    > [Info] Note that you must click the [SAVE] button to save any changes made to the fixed postings. Otherwise, all changes will be rejected.

- [DELETE]  
    Click this button to delete the selected fixed posting from the batch. For detailed information about deleting a fixed posting, see [Delete a fixed posting](../Integration/06_ManageFixedBookings.md#delete-a-fixed-posting).

- [CLEAR]  
    Click this button to clear all input fields.

- [SAVE]  
    Click this button to save any changes made.

- [CANCEL]  
    Click this button to cancel the process. A confirmation window is displayed. Click [OK] to proceed. The *Fixed postings &ndash; Batch "Batch name"* window is closed.
