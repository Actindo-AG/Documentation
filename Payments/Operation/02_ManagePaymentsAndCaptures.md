# Monitor payments and captures

A capture is a payment made. The most payment service providers create a new reference, when a payment has been captured.
> [Info] This means that the reference ID of an authorization transaction has been changed in this case. You will not be able to identify the transaction here with the authorization transaction ID.   

You can use this procedure to display all incoming references to a capture transaction from a payment service provider. You can check for communication errors between Actindo and the payment service provider that has been caused in a termination of a workflow, for example. In addition, if applicable, you can manually change the status of a transaction to *refund* to start continuing further processing. You can set the status also to *void* to clear the database.      
If everything works fine with the posting of a capture, you do not need to monitor the *Payments and Captures* menu entry.   
> [Info] You can only change the status of a capture transaction, but not any data.


## Check capture transaction

A capture provides numerous payment-related details, which may vary depending on the payment service provider settings. To decide, whether you can manually refund or void a capture transaction, you need to check its details.

#### Prerequisites

- At least one connection has been created, see [Create a connection](../Integration/01_ManageConnections.md#create-a-connection).
- At least one capture transaction has been created.

#### Procedure
[Payment and capture](../../Assets/Screenshots/Payments/PaymentsAndCaptures/DispatchNotes.png "[Payment and capture transaction]")

1. Check the capture transaction status in the *Status* column. The status displays the current stage in the payment process. You can use the status ID prefixed below to filter the list. The following statuses are available:   
    - **1 - Preparing**  
        The transaction has been created, but is not yet transferred.
    - **2 - Unconfirmed**   
    k 
    - **3 - Success**  
        Actindo has got the response from the service payment provider, that the transfer was successfully.
    - **4 - Failure**   
        The payment service provider has received the request, but it cannot process it. If available for the connection, the status information field provides further information.
    - **5 - Error**   
       Errors have been occurred during transfer.
    - **6 - Void**   
       The transaction has been voided, see [Void a payments and capture transaction](#check-payment-and-capture-transaction).
    
2. Click on a transaction to see the details.   
    The sub-tabs of the transaction are opened. <!---Wie wird das richtig genannt?-->  
3. Check the attributes, dependencies, and logs of the transaction. For more information, see the following:
     - [LIST &ndash; Attributes](../UserInterface/03_ListPaymentsAndCaptures.md#payments-and-captures-–-attributes)
     - [LIST &ndash; Dependencies](../UserInterface/03_ListPaymentsAndCaptures.md#payments-and-captures-–-dependencies)
     - [LIST &ndash; Logs](../UserInterface/03_ListPaymentsAndCaptures.md#payments-and-captures-–-logs)

## Refund capture transaction

After you have checked a capture transaction that could not be processed by the workflow, you can refund the capture transaction manually, so that the order process can be cancelled.

#### Prerequisites

The status of a capture transaction is **not** success. In this case, the further processing has been started. <!---ist das richtig-->

#### Procedure
1. Check the capture transaction you want to refund, see [Check the capture transaction](#check-capture-transactionn).
2. Select the capture transaction you want to refund by clicking the checkbox on the left.   
    The editing toolbar is displayed.
3. Click the [Refund] button. <!---was passsiert dann-->
   A confirmation message is displayed. The status of the capture transaction has changed to *Refund*.

## Void payment and capture transaction

You can void a capture transaction, if you want to disable the transaction for the Actindo database. 
> [Info] The payment service provider will not be informed about changing the status to "void". It is only done to clear the database.

#### Prerequisites

The status of a capture transaction is **not** success. In this case, further processing has already been started. <!---ist das richtig-->

#### Procedure

 1. Identify the communication issue that led to the error. To do this, check the capture transaction you want to void, see [Check the payments and captures transaction](#check-capture-transaction).
2. Select the capture transaction to be voided by clicking the checkbox on the left.   
    The editing toolbar is displayed.
3. Click the [Void] button. 
   A confirmation message is displayed. The status of the capture transaction has changed to "Void". It is no longer valid for the Actindo database.