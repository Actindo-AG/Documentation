# Postings input line

*Accounting > Post*

![Post](../../Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/Bookings.png "[Post]")

In all tabs of the *Post* menu entry, an identical footer with the input line is displayed. The contained elements and the corresponding functions are described below.

- *Seq. no.*  
  Leave the field empty. The posting numbers must be sequential and are added by the system automatically. Any number entered is overwritten by the system.

- *Currency code*  
  Click the drop-down menu to select the appropriate currency. All available currencies are displayed in the list. By default, the base currency is preselected.  

  > [Info] It is possible to set up accounts and post transactions in different currencies, but the *Accounting* module can only work with the base currency configured in the system. For detailed information about managing and posting exchange rate fluctuations, see [Post exchange rate fluctuations](../Operation/12_BookExchangeRateFluctuations.md).

- *Exchange rate*  
  Current exchange rate of the selected currency in the *Currency code* field. This field is automatically updated when changing the currency. It is recommended not to edit the field manually.

  > [Info] The system retrieves once a day the current foreign currency exchange rates as published by the ECB and applies them automatically, therefore always working with the most up-to-date information.

- *Turnover*  
  Enter the turnover value. Turnover values can be positive (incomes) or negative (expenses). This field is mandatory.

- *Contra account*  
  Enter the appropriate contra account. This field is mandatory.

  > [Info] After you have entered at least two numbers in the field, a list is displayed below the field with all accounts matching the entry. You can select the corresponding account in the list.

- *Receipt1*  
  Enter an appropriate reference value, such as the invoice number.

  > [Info] Even though it is not mandatory, it is highly recommended to fill in the *Receipt 1* field, as the system identifies and groups together any subsequent postings taking this field as reference, for example for an invoice settlement or a credit note in case of refund.

- *Receipt2*  
  Enter any other appropriate reference value, such as order number.

- *Date*  
  Enter the posting date. The valid date format is DDMMYY.

- *Account*   
  Enter the appropriate account number, for example a personal account number, that is, customer or supplier number. A valid range for personal account numbers (10000-69999 for customers and 70000-99999 for suppliers) is predefined in the system.

- *COST1*  
  Enter the applicable cost center number.  This field is only applicable if at least one cost center has been set up. For detailed information, see [COST ACCOUNTING](./02e_CostAccounting.md).

- *COST2*  
  Enter the applicable cost object number. This field is only applicable if at least one cost object has been set up. For detailed information, see [COST ACCOUNTING](./02e_CostAccounting.md).

- *Posting text*  
  Enter any appropriate posting text. The text is limited to 30 characters.


The following fields on the upper right part of the input line display the totals of the postings in the selected tab.

- *Amount*  
  Total amount of all postings in the list. This field is read-only.

  - *Amount 1*  
    Click this button to manually set an amount 1. The *Set amount 1* window is displayed, see [Set amount 1](#set-amount-1).

  - *Amount 2*  
    Click this button to manually set an amount 2. The *Set amount 2* window is displayed, see [Set amount 2](#set-amount-2).

[comment]: <> (Terminologie: lieber Sum oder Total? amount beinhaltet nicht, dass hier eine Summe, also der Gesamtbetrag aus meherer Beträgen aufgeführt wird...)


The following fields below the input line are filled in automatically when creating a manual posting or selecting a posting in the list. All fields are read-only.

- *Contra account*  
  Contra account name of the selected posting.

- *Balance*  
  Contra account balance. **H** stands for credit. **S** stands for debit.

- *Account*  
  Account name of the selected posting.

- *Balance*  
  Account balance. **H** stands for credit. **S** stands for debit.


The buttons in the footer allow to manage the postings manually.

- [POST]    
  Click this button to post the transaction entered in the input line.
  For detailed information, see [Create a manual posting](../Operation/04_CreateManualBooking.md).

- [CANCEL]  
  Click this button to cancel the selected posting. If no posting has been selected, an error notice is displayed above the input line.    
  For detailed information, see [Cancel a posting](../Operation/05_CancelBooking.md).

- [DELETE]    
  Click this button to delete the selected posting. This button is only unlocked if a posting has been selected.    
  For detailed information, see [Delete a single posting](../Operation/06_DeleteBookings.md#delete-a-single-posting).

- [CLEAR]    
  Click this button to clear all input line fields.

- [SPLIT]    
  Click this button to split the selected posting. The *Split posting* window is displayed, see [Split posting](#split-posting). If no posting has been selected, an error message is displayed.    
  For detailed information, see [Split a posting](../Operation/09_SplitBooking.md).

- [ASSIGN RECEIPT]  
  Click this button to assign a receipt to the selected posting or to unassign a receipt from the selected posting. If no document is assigned to the selected posting, the *Attach document* window is displayed, see [Attach a document](#attach-document). If a document is already assigned to the selected posting, the *Attached document* window is displayed, see [Attached document](#attached-document).   
  For detailed information, see [Retrieve a receipt](../Operation/10_ManageReceipts.md#retrieve-a-receipt).

[comment]: <> (Wann wird der button angezeigt? Bei mir wird er nicht angezeigt - und im Screeshot auch nicht. Muss ein bestimmtes Plugin installiert sein?)


## Set amount 1

*Accounting > Post > Button Amount 1*

![Post](../../Assets/Screenshots/RetailSuiteAccounting/Book/SetAmount1.png "[Post]")

- *Amount 1*  
  Enter an amount.

- [CANCEL]  
  Click this button to cancel the process. Any changes are rejected. The *Set amount 1* window is closed.

- [OK]  
  Click this button to set the entered amount. A confirmation window is displayed. Click the [OK] button to close the *Set amount 1* window.



## Set amount 2

*Accounting > Post > Button Amount 2*

![Post](../../Assets/Screenshots/RetailSuiteAccounting/Book/SetAmount2.png "[Post]")

- *Amount 2*  
  Enter an amount.

- [CANCEL]  
  Click this button to cancel the process. Any changes are rejected. The *Set amount 2* window is closed.

- [OK]  
  Click this button to set the entered amount. A confirmation window is displayed. Click the [OK] button to close the *Set amount 2* window.



## Split posting

*Accounting > Post > Select posting > Button SPLIT*

![Split posting window](../../Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/SplitBooking01.png "[Split posting window]")

**Postings list**

The list displays the selected posting and all partial postings. All fields are read-only.

- *Seq. no.*  
  Sequential number of the posting.

- *PP*  
  Month number of the posting period. 00 is displayed.

[comment]: <> (Bug? Should the actual posting period -month/journal- be shown here?)

- *Jnl*  
  Journal number of the posting period. 00 is displayed.

[comment]: <> (Bug? Should the actual posting period -month/journal- be shown here?)

- *Turnover*  
  Turnover value.

- *Contra account*  
  Contra account number. No information is displayed. The corresponding contra accounts are assigned to each split posting.

- *Receipt1*  
  Receipt 1 value, usually the invoice number.

- *Receipt2*  
  Receipt 2 value, which can be any other reference number, such as the order number.

- *Date*  
  Posting date. The valid date format is *DDMMYY*.

- *Account*  
  Account number, usually a personal account number, that is, a customer or supplier account number.

- *Cost1*  
  Number of the selected cost center. This field is only applicable if at least one cost center has been created.    
  For detailed information, see [COST ACCOUNTING](./02e_CostAccounting.md)

- *Cost2*  
  Number of the selected cost object. This field is only applicable if at least one cost object has been created.    
  For detailed information, see [COST ACCOUNTING](./02e_CostAccounting.md).

- *Text*  
  Posting text.


- *REST*  
  Outstanding invoice amount to be split. As soon as the remaining amount equals 0, the [SAVE] button is unlocked.  

- *Amount*  
  This field displays the total invoice amount.


**Input line**

The input line allows to split the posting.

- *Seq. no.*  
  Leave the field empty. The posting numbers must be sequential and are added by the system automatically. Any number entered is overwritten by the system.

- *Turnover*  
  Enter the turnover value for the partial posting. This field is mandatory.

- *Contra account*  
  Enter the appropriate contra account for the partial posting. This field is mandatory.

- *Receipt1*  
  Enter an appropriate reference value, such as the invoice number, for the partial posting.

- *Receipt2*  
  Enter any other appropriate reference value, such as order number, for the partial posting.

- *Date*  
  Posting date. The posting date of the partial posting must equal the posting date of the main posting. Any modification on the date is overwritten by the system.

- *Account*  
  Account number. The account number of the partial posting must equal the account number of the main posting. Any modification on the account number is overwritten by the system.

- *Cost1*  
  Enter the applicable cost center number. This field is only applicable if at least one cost center has been created.   
  For detailed information, see [COST ACCOUNTING](./02e_CostAccounting.md).

- *Cost2*  
  Enter the applicable cost object number. This field is only applicable if at least one cost object has been created.   
  For detailed information, see [COST ACCOUNTING](./02e_CostAccounting.md).

- *Text*  
  Enter any appropriate posting text. The text is limited to 30 characters.

- Currency code  
  Click the drop-down list to select the appropriate currency. All available currencies are displayed in the list. By default, the base currency is preselected.

- *Exchange rate*  
  Current exchange rate of the currency selected in the currency code drop-down list. This field is automatically updated when changing the currency. It is recommended not to edit this field manually.


- [POST]  
  Click this button to post a partial posting. The partial posting is displayed in the list.  

- [DELETE]  
  Click this button to delete the selected partial posting. The selected partial posting is removed from the list. Only partial postings can be deleted. This button is only unlocked if a posting has been selected.

- [CLEAR]  
  Click this button to clear all input line fields.

- [SAVE]  
  Click this button to save the partial postings and record them in the selected posting period. This button is only unlocked if the outstanding amount in the *REST* field equals **0**.

- [CANCEL]  
  Click this button to cancel the split process. All changes are rejected.

[comment]: <> (Check terminology -> hier ist überall von partial posting die Rede, im Operation part steht aber überall split posting -> einheitlich!)



## Attached document

*Accounting > Post > Select posting > Button ASSIGN RECEIPT*

[comment]: <> (Wann wird der button angezeigt? Bei mir wird er nicht angezeigt - und im Screeshot auch nicht. Muss ein bestimmtes Plugin installiert sein?)

For a detailed description of the contained elements and the corresponding functions, see [Attached document](./01_Header.md#attached-document).



## Attach document

*Accounting > Post > Select posting > Button ASSIGN RECEIPT*

[comment]: <> (Wann wird der button angezeigt? Bei mir wird er nicht angezeigt - und im Screeshot auch nicht. Muss ein bestimmtes Plugin installiert sein?)

![Attach document](../../Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/AttachDocument01.png "[Attach document]")

**Directory tree**

All folders and sub-folders set up in the *Documents* module are displayed in this side bar. Depending on the settings, the folders and sub-folders displayed may vary. By default, the following folder and sub-folders are available:

- *New documents*  
  This folder contains all new uploaded documents.


- *Registered documents*  
  This folder contains all registered documents. As soon as a new document is linked to a posting, it is moved automatically into the *Registered documents* folder and then placed in the appropriate sub-folder according to the following structure:
  - **10000-69999**   
    Personal account numbers in case of a debtors'/customers' document
  - **70000-79999**   
    Personal account numbers in case of a creditors'/suppliers' document


- *Printed documents*  
  This folder contains all printed documents.

- *New supplier receipts*  
  This folder contains all uploaded supplier receipts.

  [comment]: <> (Wann wird der ordner angezeigt? Bei mir wird er nicht angezeigt. Muss ein bestimmtes Plugin installiert sein?)


- ![Collapse](../../Assets/Icons/Up.png "[Collapse]") (Collapse)   
  Click this button to collapse the side bar.

- ![Expand](../../Assets/Icons/Expand.png "[Expand]") (Expand)  
  Click this button to expand the side bar.


- [START PAGE]  
  Click this button to go back to the top level directory on the start page of the *Attach document* window.

- [REFRESH]  
  Click this button to upload the list of documents.

- [PARENT DIRECTORY]  
  Click this button to go from the current folder to its parent directory.  

- [NEW DIRECTORY]  
  Click this button to create a new folder in the current directory.

- [UPLOAD]  
  Click this button to upload a new document. The *Upload file to* window is displayed, see [Upload file](#upload-file).

- [DELETE]  
  Click this button to delete the selected document or folder. When you delete a folder, all sub-folders and documents within this folder are also deleted.


**Documents**

The list displays all documents and folders in the selected directory. All fields are read-only.

- [x]  
  Select the checkbox to select the corresponding document or folder. If you click the checkbox in the header, all documents and folders in the list are selected.


- *Name*  
  Name of the folder or file. Double-click a folder to access it. By default, the following folders are predefined:
  - **.**   
    The next higher folder level is displayed.
  - **..**   
    The top level folder is displayed.
  - **New documents**  
    All new uploaded documents are contained in this folder.
  - **Registered documents**  
    All documents that have been registered in the system are contained in this folder.
  - **Printed documents**  
    All documents that have been printed are contained in this folder.
  - **New supplier receipts**  
    All supplier receipts that have been uploaded are contained in this folder.


  > [Info] Further folders can be created in the *Documents* module.

- *Size*  
  Size of the file. The size is only displayed for files.

- *Type*  
  Type of item. Currently, only the **Folder** type is displayed.

- *Changed*  
  Date and time of the last modification. This information is only displayed for files.

- *Owner*  
  Username of the owner.

- [ATTACH DOCUMENT]  
  Click this button to assign the selected document to the posting. The *Attach document* window is closed.

- [CLOSE]  
  Click this button to close the *Attach document* window.

[comment]: <> (Felder z.T. übernommen aus 03a_Import Select file)


### Upload file

*Accounting > Post > Select posting > Button ASSIGN RECEIPT > Button UPLOAD*

[comment]: <> (Wann wird der button angezeigt? Bei mir wird er nicht angezeigt - und im Screeshot auch nicht. Muss ein bestimmtes Plugin installiert sein?)

![Attach document window](../../Assets/Screenshots/RetailSuiteAccounting/Book/Bookings/UploadFileTo.png "[Attach document window]")

The list displays all uploaded documents. All fields are read-only.

- *Status*  
  Document status of the uploaded file.

[comment]: <> (Are there any statuses? Never displayed any status)

- *Document*  
  File path of the uploaded document.

- *Remark*  
  Remarks related to the uploaded document.

[comment]: <> (Possible that the column values of remarks and status are accidentally reversed? Possible remarks: Uploading..., OK., File x already exists!, Upload cancelled by user.)


- [ADD]  
  Click this button to add a file to be uploaded.

- [REMOVE]  
  Click this button to remove a selected file from the upload list. This button is only unlocked if a file is selected.

- [RESET]  
  Click this button to reset the upload list. This button is only unlocked if at least one file is uploaded.

- [UPLOAD]  
  This button is always locked. The upload starts automatically after adding a file. During the upload, the button is hidden and the [CANCEL] button is displayed instead.

[comment]: <> (Button ist überflüssig, da der Upload automatisch startet.-> entfernen? Oder gibt es eine Einstellung, dass der Upload nicht automatisch startet?)

- [CLOSE]  
  Click this button to close the *Upload file* window.
