## Manage workers

The workers define the way in which the webhooks waiting in the queue are to be executed. They define the retry algorithm, which specifies both the number of retries and if the webhook messages in the queue are processed sequentially or in parallel.

**Sequential processing**   
Sequential processing of webhooks is recommended for events that are related to status changes. For example, an order status change must be sent in the correct update sequence so that the status "Completed" is not overwritten by the status "Delivered". In sequential processing, only one worker processes the webhooks.<!---Wie heißen die korrekten Status?-->

> [Info] When defining the webhooks, you can specify conditions such as special fields that are to be considered. For detailed information, see [Define webhook conditions](./02_ManageWebhooks.md#define-webhook-conditions).

**Parallel processing**   
Parallel processing of webhooks is recommended for events where there is no particular sequence to follow. For example, all post persist events are suitable for parallel processing. The advantage of parallel processing is that you can define the number of workers, so you can respond to high system loads.

## Create worker