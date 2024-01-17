# Key features
- Integration with the *Payments* module
- The data structure of the connection provides exactly the data that *Adyen* needs to exchange data with the *Payments* module.
- The *Adyen* integration supports the following *Payments* transactions:
  - Authorizations
  - Captures
  - Refunds
  - Cancellation and chargebacks with second chargebacks
  - Payment details
 
 - *Adyen* provides a report that the *Payments* module uses to verify that all transactions have been successfully transferred (reconciliation).
<!---Simmt nicht, nicht?
- Receipt of authorizations, captures, refunds, cancellations and chargebacks via push notification from *Adyen* triggered by external sources such as a store-->
- Verification of push data through automated reports (reconciliation)
- Capture, cancelling & refund possible either directly via the *Payments* Module or automated.
- Triple check of payment data: directly at transaction request, at success or error message, and at report reconciliation
- Easy transfer to the *Accounting* module using the *Payment Processing* module
<!---Stimmt nicht, nicht?
- Improved open item matching (reconciliation) for payments originating from *Actindo* documents
- Synchronous or asynchronous processing of messages-->
