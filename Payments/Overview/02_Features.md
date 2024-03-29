# Key features
Organize and monitor your incoming payments and refunds:   
- Automated import of payments and refunds
- Flexible Connection with payment service providers
- Payment processing and accounting linked
- Secure handling of sensitive data  



## Automated import  
With the *Payments* module of Actindo, pre-authorized payments are captured automatically at the moment orders are delivered. The prerequisite for this is that the process has previously been automated or orchestrated with the workflow to map your specific business cases.  For example, you can define a workflow that maps the following process: You announce a product that customers can reserve, but the payment is not captured until the shipment has been started.  
In case of returns or credit notes, refund requests are automatically sent out to the original means of payment. By using the 4-eyes principle, you can optionally double-check the refunds, for example, with specific user permissions depending on the invoice amount.  
The single steps of the payments process are usually integrated in an order workflow. The workflow controls that no products are shipped without a payment commitment from the customer.


## Connecting with payment service providers  
You can flexibly connect various payment service providers such as Adyen&trade; or Paypal&trade; to the *Actindo Core1 Platform*. Depending on the payment service provider you decide for, credit cards, bank transactions, and other standard payment methods are supported implicitly.


##  Payment processing and accounting linked   
 If you have the *Actindo Accounting* module in use, the *Actindo Payments* module connects the business accounts at your various payment service providers and the *Actindo Payments Processing* module. In being the smart connection between these two, the *Actindo Payments* module helps you to process orders faster and more efficiently.  Thanks to automated payment checks, incoming payments are registered directly, and orders could therefore be processed immediately. Refunds can be made just as quickly and automatically. By linking payment and accounting, you do not only minimize the workload for your employees, but also offer your customers a smooth and fast service.


**Payments' interaction with other modules** 

![Payments interaction with other modules](../../Assets/Screenshots/Payments/Overview/PaymentsProcessModules.png "[Payments interaction with other modules]")


##  Managing all payments centrally   
In order to be able to offer your customers the widest possible range of payment methods &ndash; from invoice to credit card to direct debit &ndash; cooperation with various providers is required and provided by Actindo. This enables the management of all payments and refunds centrally via the *Actindo Core1 Platform*.  
To ensure consistent databases and if supported by the payment service provider, the *Payments* module can reconcile every day whether all payments have been successfully transferred from the payment service provider to the *Payments* module. In addition, the *Payments* module supports both asynchronous and synchronous processing. Specifics of which methods can be used depends on the capabilities of the payment service provider.


##  Handling of sensitive data  
Although you can view and monitor all incoming payments and refunds, you do not have access to any sensitive customer data. In the *Payments* module, all incoming payments and refunds are referenced to the number of the payment service provider transactions.   
Sensible data such as the full card numbers, card verification value/code, expiration dates or other data protected are not visible in the *Payments* module.  
The sensitive data remain on the payment server provider side only. In addition, an Actindo user will not be able to redirect a payment to his or her own bank account. The *Payments* transactions are a reference to the communication between the Actindo system and the payment service provider's system only. 

