# Monitor payments and captures

The most payment service providers create a new reference, when a payment has been captured. This means that the reference ID of an authorization ticket has been changed in this case and you will not be able to identify the transaction here with the authorization ticket ID.
You can use this procedure to display all incoming referencies to a payment and capture from a payment service provider.  You can check for communication errors between Actindo and the payment service provider that has been caused in a termination of a workflow, for example. In addition, if applicable, you can manually change the status of a ticket to *void* or *refund* to start continuing further processing.       
If everything works fine with the posting of a payment or capture, you do not need to monitor the *Payments and Captures* menu entry.   

## Check payment and capture ticket

A payment and capture provides numerous payment-related details, which may vary depending on the payment service provider settings. To decide, whether you can manually refund or void a payment or capture ticket, you need to check its details.
> [Info] You can only change the status of a payment and capture ticket, but not any data.

#### Prerequisites

- At least one connection has been created, see [Create a connection](../Integration/01_ManageConnections.md#create-a-connection).
- At least one payment or capture has been created.

#### Procedure
[Payment and capture](../../Assets/Screenshots/Payments/PaymentsAndCaptures/DispatchNotes.png "[Payment and capture ticket]")

1. Check the payment and capture ticket status in the *Status* column. The status displays the current stage in the payment process. The following statuses are available: 
    - **Success**   
    The payment and capture ticket has been successfully processed.
    - **Failure**   
    m
    
2. Click on a ticket to see the details.   
    The sub-tabs of the ticket are opened. <!---Wie wird das richtig genannt?-->  
3. Check the attributes, dependencies, and logs of the ticket. For more information, see the following:
     - [LIST &ndash; Attributes](../UserInterface/03_ListPaymentsAndCaptures.md#payments-and-captures-–-attributes)
     - [LIST &ndash; Dependencies](../UserInterface/03_ListPaymentsAndCaptures.md#payments-and-captures-–-dependencies)
     - [LIST &ndash; Logs](../UserInterface/03_ListPaymentsAndCaptures.md#payments-and-captures-–-logs)

## Refund a payment and capture ticket

After you have checked a payment and capture ticket that could not be processed by the workflow, you can refund the payment or capture manually, so that the order process can be cancelled.

#### Prerequisites

The status of an payment and capture ticket is **not** success. In this case, the further processing has been started. <!---ist das richtig-->

#### Procedure
1. Check the payment and capture ticket you want to refund, see [Check the payment and capture ticket](02_ManagePaymentsAndCaptures.md#check-payment-and-capture-ticket).
2. Select the payment and capture ticket you want to refund by clicking the checkbox on the left.   
    The editing toolbar is displayed.
3. Click the [Refund] button. <!---was passsiert dann-->
   The status of the payment and capture ticket has changed to *Refund*.

## Void payment and capture ticket

You can void a payment and capture ticket, if you want to disable the ticket for the Actindo database. 
> [Info] The payment service provider will not be informed about changing the status to "void". It is only done to clear the database.

#### Prerequisites

The status of a payment and capture ticket is **not** success. In this case, further processing has already been started. <!---ist das richtig-->

#### Procedure

 1. Identify the communication issue that led to the error. To do this, check the payment and capture ticket you want to void, see [Check the authorization ticket](02_ManagePaymentsAndCaptures.md#check-payment-and-capture-ticket).
2. Select the authorization ticket to be voided by clicking the checkbox on the left.   
    The editing toolbar is displayed.
3. Click the [Void] button.  <!---was passsiert dann-->   
   The status of the authorization ticket has changed to "Void". It is not longer valid for the Actindo database.