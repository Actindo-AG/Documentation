# Manage the business document chain

## The business document chain

The different business documents form a document chain, which can be completely customized to reflect your company's business processes. The main entity of the document chain is the head document, which, in the basic order management process, is the order confirmation. The so-called deliver head, on the other hand, creates a reservation posting in the warehouse for all line items detailed in the business document. In the basic order management process, the head document and the deliver head are the same business document, but this is not mandatory and can be configured to suit your needs.


[comment]: <> (Aus Core: ggf. anpassen! Head document vs deliver head klären)

### Standard business document chain

You can configure your business document chain freely. The configuration is currently done by our Implementation team when setting up your system.

[comment]: <> (Was tun unsere ImpSpecs? Was tun der Kunde in Process Orchestration?)

Nevertheless, the nature of each business document determines to a certain extend the logical sequence of the business document chain. 

The standard business document chain presents the following sequence:

1. Offer (German abbreviation: AN)
2. Order confirmation (German abbreviation: AB)
3. Invoice (German abbreviation: RE)
4. Delivery note (German abbreviation: LI)

Usually, the system creates an order confirmation when a new order has been placed in the sales channel and is imported the via the *Omni-Channel* module. The orders imported in *Omni-Channel* are then exported to *Order Management* module for further processing. This is the first document in the chain, the so-called *head document*. All further business documents follow the head document. 

The order confirmation creates a reservation in the *Warehousing* module.

It is also possible to start the business document chain with an offer previous to the order confirmation.

The next step is the invoice. After the order has been confirmed, an invoice is created. The invoice is sent to the customer. It creates an open item in the *Accounting* module.




| Business document      | Accounting posting | Posting type        | Warehousing posting | Posting type        |
|------------------------|--------------------|---------------------|---------------------|---------------------|
| **Offer**              | no                 |                     | no                  |                     |
| **Order confirmation** | no                 |                     | yes                 | reservation         |
| **Invoice**            | yes                | open item           | no                  |                     |
| **Cash invoice**       | yes ?              | open item ?         | yes                 | sale (immediate withdrawal)  <!-- old POS, noch relevant? --> |
| **Partial invoice**    | yes ?              | open item ?         | no                  |                     |
| **Correction invoice** | yes ?              | cancels open item   | no                  |                     |
| **Value credit**       | no                 |                     | yes                 |                     |
| **Delivery note**      | no                 |                     | yes                 | reserved for open delivery note (delivery note created) <br> sale (delivery note processed and closed) |
| **Dunning notice**     | no                 |                     | no                  |                     |
| **Purchase order**     | yes ?              | open item           | yes ?               | order               |
| **Loan voucher**       | yes                |                     | yes ?               |                     |
| **Proforma invoice**   | no                 |                     | no                  |                     |
| **Reversal document**  | yes                | cancels open item?  | no                  |                     |
| **Dropship delivery note**| yes             |  open item ?        | pseudo-posting for informative purposes | dropship  |
| **Return**             |  yes               |                     | yes / no ?          |                     |
| **Return to customer or supplier** | ?      |                     | yes                 | Back to supplier ("Send to supplier and ship to customer after stock receipt" follow-up action activated) |



Aus welche Belege welche andere Belege erstellt werden können (Rechtsklick -> Context menu)

