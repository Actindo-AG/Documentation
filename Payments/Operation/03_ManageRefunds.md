[!!LIST (Refunds)](../UserInterface/03a_ListRefunds.md)

# Monitor refunds

A refund is a request for a repayment of a capture. It is initiated by the receiver of a payment, for example, when a customer has returned the product. Each refund is to be confirmed with the *Confirmation* menu entry later.

> [Info] You cannot follow up a case with the ID of an authorization or a payments and captures transaction. However, the most payment service providers support an original reference ID that you can use to search for a specific case in the whole payment process.

You can use this procedure to display all incoming references to a refund from a payment service provider. You can check for communication and other errors between Actindo and the payment service provider resulted in a workflow being stopped, for example. In addition, if applicable, you can manually change the status of a transaction to **Void** to clear the database. Note that you can only change the status of a refund transaction, but not any data.
   
If everything works fine with the posting of a refund, you do not need to monitor the *Refunds* menu entry. You can follow up the successfully processed refunds with the *Confirmation* menu entry. 



## Check refund transaction

A refund transaction provides numerous payment-related details, which may vary depending on the payment service provider settings. To decide whether you can manually void a refund transaction, you need to check its details, so that the issue can be solved.   
In case of errors or failures, there may be a general issue that is caused by the payment service provider, by the shop, or by Actindo. In this case, contact the according business partner, so that the issue can be solved.  


#### Prerequisites

- At least one connection has been created, see [Create PSP connection](../Integration/01_ManageConnection.md#create-psp-connection).
- At least one refund has been created.

> [Info] It is recommended to add the following columns to your view to get the required information and to better filter and sort the entries: *Status ID* and *Status information* (if applicable).


#### Procedure   

*Payments > Refunds > Tab LIST* 

![Refund transactions](../../Assets/Screenshots/Payments/Refunds/LISTRefunds.png "[Refund transactions]")

1. Check the refund transaction status in the *Status* column. The status displays the current stage in the payment process. You can use the status ID prefixed below to filter the list. The following statuses are available:   
    - **1 - Preparing**  
        The transaction has been created, but is not yet transferred.
    - **2 - Unconfirmed**   
        A refund is reserved but not yet released by an Actindo user. This status is relevant for some functions only, for example, the cancellations and chargebacks.
    - **3 - Success**  
        Actindo as well as the payment service provider has processed the transaction successfully. 
        You can now follow up this case under the menu entry *Confirmations*. <!---Stefan ist das richtig?--> 
    - **4 - Failure**   
        The payment service provider has received the request, but rejected it. If available for the connection, the status information field provides further information.
    - **5 - Error**   
        Errors have been occurred during transfer.
    - **6 - Void**   
        The transaction has been voided, see [Void refund transaction](#void-refund-transaction)
    
2. Click a transaction to see the details.   
    The *"Refund ID"* view is displayed. The *Attributes* tab is preselected by default.    

    ![Attributes](../../Assets/Screenshots/Payments/Refunds/AttributesRefund.png "[Attributes]")

3. Check the list of attributes, for example, whether the required fields are filled. For detailed information on fields, see [Refund &ndash; Attributes](../UserInterface/03a_ListRefunds.md#refund-–-attributes).

4. Click the *Logs* tab.   
    The *Logs* tab is displayed and shows the messages that have been created for this issue. 

    ![Logs](../../Assets/Screenshots/Payments/Refunds/AttributesRefund.png "[Logs]")

5. Check the logs, for example, if there is a general communication issue.
    For detailed information on fields and functions, see [LIST (Logging)](../UserInterface/07a_ListLogging.md).

     
6. Return to the list of refunds and decide how to proceed with the transaction.



## Void refund transaction

You can void a refund transaction, if you want to invalidate the transaction for the Actindo database. 

> [Info] The payment service provider will not be informed about changing the status to **Void**. It is only done to clear the database from faulty entries.

#### Prerequisites

The status of a refund transaction is **Failure** or **Error**. 

#### Procedure

*Payments > Refunds > Tab LIST*

![Refund transactions](../../Assets/Screenshots/Payments/Refunds/LISTRefunds.png "[Refund transactions]")

 1. Identify the issue that led to the error/failure. To do this, check the refund transaction you want to void, see [Check refund transaction](#check-refund-transaction).

2. Select the refund transaction to be voided by clicking the checkbox on the left.   
    The editing toolbar is displayed.

3. Click the [VOID] button.   
    A confirmation message is displayed. The status of the refund transaction has changed to **Void**. The transaction is no longer valid for the Actindo database.