# Monitor authorizations
The payment service provider creates an authorization ticket, when a customer presses the *Pay now* button during the order process. The payment provider sends then the authorization ticket to the *ActindoCore1 Platform*. In addition, the shop system creates an ID for this transaction. Actindo links both.
You can use this procedure to display all incoming authorization tickets of a payment service provider. You can check for communication errors between Actindo and the payment service provider that has been caused in a termination of a workflow. In addition, if applicable, you can change the status of a ticket to start continuing further processing.    
For Actindo,  the authorization ticket serves as a reference to a payment made by a customer.   
 > [Info] An authorization ticket does not contain any sensible data protected by a data protection act such as GDPR. Those data remain on the payment server provider side only. In addition, an Actindo user will not be able to redirect a payment to his or her own bank account. The authorization ticket is a reference to the communication between the Actindo system and the payment service provider's system only.    

If everything works fine with the posting of the payment, you do not need to monitor the *Authorizations* menu entry.   
<!---In rare cases something went wrong if the workflow cannot post a payment correctly. This may happen, for example, if something went wrong during pressing the *Pay now* button by the customer. In this case, the service payment provider may has sent two references to a payment to the *Payments* module. Now the workflow is not able to find the correct reference and ends with an error. -->  
In case of those errors you can capture, cancel, or void an authorization ticket manually.   
> [Info] You can only change the status of an authorization ticket, but not any data.


## Check an authorization ticket
An authorization ticket provides numerous payment-related details, which may vary depending on the payment service provider settings. To decide, whether you can manually capture, cancel, or void an authorization ticket, you need to check the its details.

#### Prerequisites

- At least one connection has been created, see [Create a connection](../Integration/01_ManageConnections.md#create-a-connection).
- At least one authorization ticket has been created.

#### Procedure
[Authorization ticket](../../Assets/Screenshots/Fulfillment/DispatchNotes/DispatchNotes.png "[Authorization ticket]")

1. Check the Authorization ticket status in the *Status* column. The status displays the current stage in the payment process. The following statuses are available: 
    - **Success**   
    The authorization ticket has been successfully processed.
    - **Error**   
    k 
    - **Failure**   
    l
    - **Preparing**  
    ö 
2. Click on the authorization ticket to see the details.   
    The sub-tabs of the ticket are opened. <!---Wie wird das richtig genannt?-->  
3. Check the attributes, dependencies, and logs of the ticket. For more information, see the following:
   - [Authorizations &ndash; Attributes](../UserInterface/01_ListAuthorizations.md#authorizations-–-attributes)
   - [Authorizations &ndash; Dependencies](../UserInterface/01_ListAuthorizations.md#authorizations-–-dependencies)
   - [Authorizations &ndash; Logs](../UserInterface/01_ListAuthorizations.md#authorizations-–-logs)
4. Return to the LIST and decide how to proceed with the ticket.

## Capture an authorization ticket

After you have checked an authorization ticket that could not be processed by the workflow, you can capture the ticket manually, so that the order process can be continued.

#### Prerequisites

The status of an authorization ticket is **not** "failure" or "error". <!---Stimmt das oder gibt es noch mehr?-->

#### Procedure

1. Check the authorization ticket you want to capture, see [Check the authorization ticket](01_ManageAuthorization.md#check-an-authorization-ticket).
2. Select the authorization ticket you want to capture by clicking the checkbox on the left.   
    The editing toolbar is displayed.
3. Click the [Capture] button. <!---was passsiert dann-->
   The status of the authorization ticket changes to *Success*.
  

## Cancel an authorization ticket
After you have checked an authorization ticket that could not be processed by the workflow, you can cancel the ticket manually, so that the order is cancelled both at Actindo  and at the PSP. Actindo will then automatically inform the PSP about the cancellation. The customer will get his or her money back.

#### Prerequisites
The status of an authorization ticket is "failure" or "error".

#### Procedure
1. Identify the communication issue that led to the error. To do this, check the authorization ticket you want to cancel, see [Check the authorization ticket](01_ManageAuthorization.md#check-an-authorization-ticket).
2. Select the authorization ticket you want to cancel by clicking the checkbox on the left.   
    The editing toolbar is displayed.
3. Click the [Cancel] button.<!---was passsiert dann-->
   The status of the authorization ticket has changed to *Cancel??*.


## Void an authorization ticket

You can void an authorization ticket, if you want to disable the ticket for the Actindo database. For example, for whatever reason the same transaction has been posted twice. In this case, you can void one of these tickets and continue the order process with the other ticket.
> [Info] The payment service provider will not be informed about changing the status to "void". It is only done to clear the database.


#### Prerequisites

The status of an authorization ticket is "failure" or "error".

#### Procedure

1. Identify the communication issue that led to the error. To do this, check the authorization ticket you want to void, see [Check the authorization ticket](01_ManageAuthorizations.md#check-an-authorization-ticket).
2. Select the authorization ticket to be voided by clicking the checkbox on the left.   
    The editing toolbar is displayed.
3. Click the [Void] button.  <!---was passsiert dann-->   
   The status of the authorization ticket has changed to "Void". It is not longer valid for the Actindo database.