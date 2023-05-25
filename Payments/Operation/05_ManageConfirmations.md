# Manage confirmations

The *Confirmation* menu entry provides you with a view on all references to refunds that has been created. Before your company sends back the money to the customer, you have to check the refunds with this menu entry. This service is supported by the most payment service providers.
> [Info] If a workflow decides that you have to sent back money to the customer, you have here the possibility to check the refunds before money is returned.   

You can use this procedure to accept a refund so that the service payment provider gets the request to send back the money to the customer. You can also reject a refund, if it is not justified, for example, because the goods have already been delivered. In case of faulty transactions you can void them to clear the database.   

In the settings might have been applied special permissions.
> [Info] You might not be able to access this menu entry, because you have no permissions to do it. Furthermore, you may have access, but you are not permitted to execute refunds above a certain amount (for example, more than 50€). 


## Check confirmation transaction  

*Payments > Confirmations > Tab LIST*  

![Confirmation transaction](../../Assets/Screenshots/Payments/Confirmations/LISTConfirmations.png "[Confirmation transaction]")

A confirmation transaction provides numerous payment-related details on a refund, which may vary depending on the payment service provider settings. To decide whether you can execute, reject or void a transaction, you can check its details.  
> [Info] You can only change the status of a confirmation transaction, but not any data.


#### Prerequisites 

- At least one connection has been created, see [Create a connection](../Integration/01_ManageConnections.md#create-a-connection).
- At least one refund has been created.
- The view displays in minimum the *Amount* and the *Status* column. If it is necessary, it also shows the *Currency* column. For more information, see [LIST &ndash; Confirmations](../UserInterface/06_ListConfirmations.md#create-view).
- You have the original reference ID for this transaction.

#### Procedure

1. If desired, click the ![Search](../../Assets/Icons/Search.png "[Search]") (Search) button to display the search bar and search for the original reference ID of the refund.
2. Check the confirmation transaction status in the *Status* column. The status displays the current stage in the confirmation process. You can use the status ID prefixed below to filter the list. The following statuses are available: 
    - **2 - Confirmation required**   
    -    
3. Click on a transaction to see the details.   
    The sub-tabs of the transaction are opened.   

    ![Confirmation attributes](../../Assets/Screenshots/Payments/Confirmations/AttributesConfirmation.png "[Confirmaton attributes]")
4. If required, check the details of the refund. For more information, see the following:
     - [LIST &ndash; Attributes](../UserInterface/06_ListConfirmations.md#confirmations-–-attributes)



## Execute confirmation transaction

After you have checked a confirmation transaction and the reclaim is justified, you can execute it. The payment service provider can than arrange the repayment of the money.  

#### Prerequisites
- At least one connection has been created, see [Create a connection](../Integration/01_ManageConnections.md#create-a-connection).
- At least one refund has been created.
- At least the *Amount* and the *Status* column is displayed in the view.
- The status of a confirmation transaction is "Confirmation required". 

#### Procedure
*Payments > Confirmations > Tab LIST*

![Execute confirmation](../../Assets/Screenshots/Payments/Confirmations/ChangeConfirmation.png "[Execute confirmaton]")

1. If desired, click the ![Search](../../Assets/Icons/Search.png "[Search]") (Search) button to display the search bar and search for the original reference ID of the refund.
2. Check the confirmation transaction you want to execute, see [Check the confirmation transaction](05_ManageConfirmations.md#check-confirmation-transaction).
2. Select the confirmation transaction you want to execute by clicking the checkbox on the left.   
    The editing toolbar is displayed.
3. Click the [Execute] button.
   The status of the authorization transaction has changed to *Executed??*. The workflow will now initiate a repayment of the money.



## Reject confirmation transaction

After you have checked a confirmation transaction and the reclaim is **not** justified, you can reject it.   

#### Prerequisites
- At least one connection has been created, see [Create a connection](../Integration/01_ManageConnections.md#create-a-connection).
- At least one refund has been created.
- At least the *Amount* and the *Status* column is displayed in the view.
- The status of a confirmation transaction is "Confirmation required". 

#### Procedure

*Payments > Confirmations > Tab LIST*

![Reject confirmation](../../Assets/Screenshots/Payments/Confirmations/ChangeConfirmation.png "[Reject confirmaton]")


1. If desired, click the ![Search](../../Assets/Icons/Search.png "[Search]") (Search) button to display the search bar and search for the original reference ID of the refund.
2. Check the confirmation transaction you want to reject, see [Check the confirmation transaction](./05_ManageConfirmations.md#check-confirmation-transaction).
2. Select the confirmation transaction you want to reject by clicking the checkbox on the left.   
    The editing toolbar is displayed.
3. Click the [Execute] button. <!---was passsiert dann-->
   The status of the confirmation transaction has changed to *Rejected??*. The workflow will now inform the payment service provider about the rejection of the refund.




## Void confirmation transaction  

You can void a refund transaction, if you want to disable the transaction for the Actindo database. 
> [Info] The payment service provider will not be informed about changing the status to "Void". It is only done to clear the database.  

#### Prerequisites
- The status of a confirmation transaction is **not** "Confirmation required". 

#### Procedure

*Payments > Confirmations > Tab LIST*

![Void confirmation](../../Assets/Screenshots/Payments/Confirmations/ChangeConfirmation.png "[Void confirmaton]")

1. Identify the communication issue that led to the error. To do this, check the confirmation transaction to be voided, see [Check the confirmation transaction](05_ManageConfirmations.md#check-confirmation-transaction).
2. Select the Confirmation transaction to be voided by clicking the checkbox on the left.   
    The editing toolbar is displayed.
3. Click the [Void] button.  
   
   The status of the confirmation transaction has changed to "Void". It is no longer valid for the Actindo database.