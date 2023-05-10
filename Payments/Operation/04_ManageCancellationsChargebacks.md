# Monitor cancellations and chargebacks

The most payment service providers create a new reference, when a payment has been cancelled or charged back by the customer. This means that the reference ID of a refund ticket has been changed in this case and you will not be able to identify the transaction here with the refund ticket ID.   
You can use this procedure to display all incoming referencies to a cancellation and chargeback from a payment service provider. You can check for communication errors between Actindo and the payment service provider that has been caused in a termination of a workflow, for example. In addition, if applicable, you can manually change the status of a ticket to *void* to clear the database.    
   
If everything works fine with the posting of a cancellation and chargeback, you do not need to monitor the *Cancellations and Chargebacks* menu entry.  

## Check cancellation and chargeback ticket

A cancellation and chargeback ticket provides numerous payment-related details, which may vary depending on the payment service provider settings. To decide whether you can manually void a cancellation and chargeback ticket, you need to check its details.  
> [Info] You can only change the status of a cancellation and chargeback ticket, but not any data.

#### Prerequisites

- At least one connection has been created, see [Create a connection](../Integration/01_ManageConnections.md#create-a-connection).
- At least one chargeback or cancellation has been created.

#### Procedure
[Refunds](../../Assets/Screenshots/Payments/ManageConfirmations/DispatchNotes.png "[Refund ticket]")

1. Check the cancellation and chargeback ticket status in the *Status* column. The status displays the current stage in the payment process. The following statuses are available: 
    - **Success**   
    The payment and capture ticket has been successfully processed.
    - **Failure**   

    
2. Click on a ticket to see the details.   
    The sub-tabs of the ticket are opened. <!---Wie wird das richtig genannt?-->  
3. Check the attributes, dependencies, and logs of the ticket. For more information, see the following:
     - [LIST &ndash; Attributes](../UserInterface/05_ListCancellationsChargebacks.md#cancellations-and-chargebacks-–-attributes)
     - [LIST &ndash; Dependencies](../UserInterface/04_ListRefunds.md#refunds-–-dependencies)
     - [LIST &ndash; Logs](../UserInterface/04_ListRefunds.md#refunds-–-logs)


## Void a cancellation and chargeback ticket

You can void a cancellation and chargeback ticket, if you want to disable the ticket for the Actindo database. 
> [Info] The payment service provider will not be informed about changing the status to "void". It is only done to clear the database.

#### Prerequisites

The status of a cancellation and chargeback ticket is **not** success. In case of success, the refund has already been processed further. <!---ist das richtig-->

#### Procedure

 1. Identify the communication issue that led to the error. To do this, check the cancellation and chargeback ticket to be voided, see [Check the cancellation and chargeback ticket](04_ManageCancellationsChargebacks.md#check-cancellation-and-chargeback-ticket).
2. Select the cancellation and chargeback ticket to be voided by clicking the checkbox on the left.   
    The editing toolbar is displayed.
3. Click the [Void] button.  <!---was passsiert dann-->   
   The status of the cancellation and chargeback ticket has changed to "Void". It is not longer valid for the Actindo database.
