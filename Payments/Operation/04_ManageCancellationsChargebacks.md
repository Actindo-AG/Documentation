[!!LIST (Cancellations and chargebacks](../UserInterface/05a_ListCancellationsChargebacks.md)

# Monitor cancellations and chargebacks

In the context of a payment transaction a chargeback is a retroactive cancellation of a capture. It is initialized by the customer, for example, if he or she withdraws the payment. A cancellation is a revocation of the reservation of a product that has not yet been delivered. It is also initialized by the customer.    

> [Info] The most payment service providers create a new reference, when a payment has been cancelled or charged back by the customer. However, the most payment service providers support an original reference ID that you can use to search for a specific case in the whole payment process.  

You can use this procedure to display all incoming references to cancellations and chargebacks from a payment service provider. You can check for communication errors between Actindo and the payment service provider that has been caused in a termination of a workflow, for example. In addition, if applicable, you can manually change the status of a transaction to *void* to clear the database.    
   
If everything works fine with the posting of a cancellation and chargeback, you do not need to monitor the *Cancellations and chargebacks* menu entry.  


## Check cancellations and chargeback transaction

A cancellation and chargeback transaction provides numerous payment-related details, which may vary depending on the payment service provider settings. To decide whether you can manually void a cancellation and cancellation and chargeback transaction, you need to check its details.  
> [Info] You can only change the status of a chargeback transaction, but not any data.

#### Prerequisites

- At least one connection has been created, see [Create a connection](../Integration/01_ManageConnections.md#create-a-connection).
- At least one customer has created a chargeback or a cancellation.
- It is recommended that you add the *Status ID* field to your view so that you are able to sort or filter for specific statuses. 

#### Procedure

*Payments > Cancellations and chargebacks > Tab LIST *   

![Cancellations and chargebacks](../../Assets/Screenshots/Payments/CancellationsChargebacks/LISTCancellationsChargebacks.png "[Cancellation and chargeback transaction]")

1. Select the desired view.   

2. If desired, select the cancellation and chargeback type you want to check. The following types are available:   
    - **Cancel**   
      Depending on the payment service provider, an appropriately permitted person has cancelled the authorization. 
    - **Chargeback**   
      The customer has withdrawn a capture.
    - **Chargeback Reversal**   
      The customer has terminated his or her withdrawing of the authorization.
    - **Second Chargeback**   
      Again, the customer has withdrawn the authorization.

3. Check the cancellation and chargeback transaction status in the *Status* column. The status displays the current stage in the payment process. You can use the status ID prefixed below to filter the list. The following statuses are available:   
    - **1 - Preparing**  
        The transaction has been created, but is not yet transferred.
    - **2 - Unconfirmed**   
        A refund is reserved but not yet released by an Actindo user. 
    - **3 - Success**  
        Actindo has got the response from the service payment provider, that the transfer was successfully.
    - **4 - Failure**   
        The payment service provider has received the request, but it cannot process it. If available for the connection, the status information field provides further information.
    - **5 - Error**   
       Errors have been occurred during transfer.
    - **6 - Void**   
       The transaction has been voided, see [Void an authorization transaction](./01_ManageAuthorizations.md#void-an-authorization-transaction).
    
2. Click on a transaction to see the details.   
    The sub-tabs of the transaction are opened.   

    *Payments > Cancellations and chargebacks> Tab LIST > Select a cancellation and chargeback transaction*  

    ![Cancellations and chargebacks attributes and logs](../../Assets/Screenshots/Payments/CancellationsChargebacks/CheckCancellationsChargebacks.png "[Cancellations and chargebacks attributes and logs]")

3. Check the attributes and logs of the transaction. For detailed information, see the following:
     - [LIST &ndash; Attributes](../UserInterface/05_ListCancellationsChargebacks.md#cancellations-and-chargebacks-–-attributes)
     - [LIST &ndash; Logs](../UserInterface/04_ListRefunds.md#refunds-–-logs)
4. Return to the LIST and decide how to proceed with the transaction.


## Void cancellation and chargeback transaction

You can void a cancellation and chargeback transaction, if you want to disable the transaction for the Actindo database. 
> [Info] The payment service provider will not be informed about changing the status to "void". It is only done to clear the database.

#### Prerequisites

The status of a cancellation and chargeback transaction is **not** success. In case of success, the cancellation and chargeback has already been further processed and is available under the *Confirmations* menu entry. <!---Stefan, ist das richtig oder ist es unter Refund? --> 

#### Procedure

*Payments > Cancellations and chargebacks > LIST*   

![LIST (Cancellations and chargebacks](../../Assets/Screenshots/Payments/CancellationsChargebacks/VoidCancellationsChargebacks.png "[LIST (Cancellations and chargebacks]")

 1. Identify the communication issue that led to the error. To do this, check the cancellation and chargeback transaction to be voided, see [Check cancellation and chargeback transaction](#check-cancellations-and-chargeback-transaction).
2. Select the cancellation and chargeback transaction to be voided by clicking the checkbox on the left.   
    The editing toolbar is displayed.
3. Click the [Void] button.    
   A confirmation message is displayed. The status of the cancellation and chargeback transaction has changed to *Void*. It is no longer valid for the Actindo database.
