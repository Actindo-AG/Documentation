# Synchronous processing

**Initial situation**    
You use the synchronous processing of messages and a faulty message from Adyen blocks its queue.

**Description**    

Like Actindo, Adyen uses a queue to send messages. If you are using synchronous message processing, it may happen that a faulty message blocks the queue.  In this case, Adyen will periodically try to process the message again. As long as this is not successful, all subsequent messages will wait, and you will not receive any payment data from Adyen.

**Solution approach**

If applicable, change from synchronous processing to asynchronous processing to prevent these situations. For detailed information, see [Define synchronous or asynchronous processing](../Integration/01_ManageAdyenSettings.md).
