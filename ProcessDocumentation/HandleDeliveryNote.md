# Handle delivery note

![Handle delivery note](../Assets/Screenshots/ProcessDocumentation/HandleDeliveryNotes.png "[Handle delivery note]")

**Short description**

The *Handle delivery note* workflow is used to process the delivery of the order handled in the [*Import order and create delivery note*](./ImportOrderCreateDeliveryNote.md) workflow. 

**Summary**

|    |    |  
|----|----|
|**Purpose** | Ship the order to the customer. |
|**Affected entities** | Actindo.Modules.Actindo.Channels.Models.Order <br> Actindo.Extensions.Actindo.UCSProductSync.Models.RetailSuiteOrder <br> Actindo.Modules.RetailSuite.RetailSuiteFaktBase.Models.BusinessDocument <br> Actindo.Modules.Actindo.Fulfillment.Models.DispatchNote <br> Actindo.Modules.Actindo.Channels.Models.Shipment (indirectly)|
|**Included plugins** | Workflows <br> Omni-Channel <br> PIM <br> Order Management <br> Warehouse <br> Accounting <br> Taxes <br> Fulfillment <br> DataHub | 
|**Included thrid party software** | (optional) |   
|**Trigger** |  The process is triggered by the subordinate [*Import order and create delivery note*](./ImportOrderCreateDeliveryNote.md) process. | 
|**Alternative workflows** |   |
|    |     |


**Included steps**

- Synchronization of the shipments in the *Omni-Channel* module
- Delivery creation in the *Omni-Channel* module and upload to the channel (marketplace or webshop) 
- Invoice creation from the delivery note
- Invoice export to an external system, for example an accounting system (optional)
- Dispatch note creation in the *Fulfillment* module
- Dispatch note transfer to an external logistics provider
- Differentiation between multiple LSPs (optional)
- Shipment status update in the channel after report by the LSP
- Synchronitation of the dispatch note



## How to set up a delivery note workflow

After a delivery note has been created for an order, the further delivery process can be handled in Actindo until its final delivery to the customer. 
You can automate this process by using the *Workflows* module and building a workflow that is handling all processes after the import up to the delivery. As each workflow can be customized, it is possible to include or exclude different processes depending on the customers needs.
In the following, it is described how to build a workflow template that is covering the processes below:
- Delivery transfer to the logistics service provider (LSP)
- Dispatch note creation
- Dispatch handling by the LSP and delivery to the customer
- Order status update
- Invoice creation
- Invoice transfer to an external system

#### Prerequisites

- The *Accounting* module is configured.
- The *Taxes* module is configured.
- The products are created in the *PIM* module. 
- A connection to the channel (marketplace or webshop) is configured in the *Omni-Channel* module and the offers to the products are created.
- A connection to the logistics service provider (LSP) is configured in the *Fulfillment* module.


#### Procedure

*Workflows > Workflows > Tab OVERVIEW*

![Workflows](../Assets/Screenshots/ActindoWorkFlow/Workflows/Workflows.png "[Workflows]")

1. Click the ![Add](../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The *New workflow* window is displayed.

  ![New workflow](../Assets/Screenshots/ActindoWorkFlow/Workflows/NewWorkflow.png "[New workflow]")

2. Enter **Handle Delivery Notes** in the *Select a name for your new workflow* field.

3. Enter **delivery_notes** in the *Select a unique key for your new workflow* field. The key is required for API access and must be unique within the workflow version.

4. Select the **___WorkflowAutogen___\Actindo\Modules\RetailSuite\RetailSuiteFaktBase\Models\BusinessDocument** option as start place type in the *Choose the data type of your start place* field.

  > [Info] Enter a keyword in the field, for example **business**, to limit the data types displayed in the list. The list of data types is filtered for your keyword as you type.

5. Select the **___WorkflowAutogen___\Actindo\Modules\RetailSuite\RetailSuiteFaktBase\Models\BusinessDocument** option as end place type in the *Choose the data type of your end place* field.

  > [Info] Enter a keyword in the field, for example **business**, to limit the data types displayed in the list. The list of data types is filtered for your keyword as you type.

6. Click the [CREATE] button in the bottom right corner.   
  The new workflow has been created. The *New workflow* window is closed. The workflow editor with the defined start and end places is displayed.  

  ![Workflow editor new](../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowEditorNew.png "[Workflow editor new]")

7. In a new window, open the JSON library for workflows and copy the JSON code for the *Handle Delivery Notes* workflow to your clipboard, see [JSON Handle Delivery Note](./HandleDeliveryNote.json).

8. In the workflow editor, click the ![Points](../Assets/Icons/Points02.png "[Points]") (Points) button in the upper left corner next to the workflow name.   
  The workflow context menu is displayed.

  ![Context menu](../Assets/Screenshots/ActindoWorkFlow/Workflows/ContextMenu.png "[Context menu]")

9. Click the *Import JSON ..* menu entry in the context menu.   
  The *Import JSON* window with the JSON code for the current workflow is displayed.

  ![Import JSON](../Assets/Screenshots/ActindoWorkFlow/Workflows/ImportJSON.png "[Import JSON]")

10. Select the complete JSON code in the window, replace it by the JSON code in your clipboard and click the [IMPORT JSON] button in the bottom right corner.
  The *Import JSON* window is closed. The copied workflow is displayed in the workflow editor.

  ![Workflow editor copied](../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowEditorCopied.png "[Workflow editor copied]")

  > [Info] You can edit the workflow as desired before deploying it.

11. Click the ![Points](../Assets/Icons/Points02.png "[Points]") (Points) button in the upper left corner next to the workflow name.   
  The workflow context menu is displayed.

  ![Context menu](../Assets/Screenshots/ActindoWorkFlow/Workflows/ContextMenu.png "[Context menu]")

12. Click the *Deploy* menu entry in the context menu.   
  The copied workflow has been deployed and published.

  > [Info] For detailed information about the single actions, see [Link zu action description](to_be_completed).



## Description of the *Handle delivery note* process

Within a workflow, several actions are performed. If a certain number of actions are executed in a specific order with a common objective that can only be achieved by executing all of these actions, we speak of a so-called *snippet*. 
In the following, all snippets and single actions within the process are described in detail, specifying their function and functional settings.


### Sync shipments

![Sync shipments](../Assets/Screenshots/ProcessDocumentation/SyncShipments01.png "[Sync shipments]")

The *Sync shipments* action is used to create the *shipment* entity in the *Omni-Channel* module and set its status to **open**. Depending on the driver of the connection, the channel is updated asynchronously.

#### Settings

The *Description* field contains the API endpoint that is addressed in this action. The *Key*, *Label*, *Queue type* and *Max tries* field have no functional meaning for the action.  

- *Description*   
  .syncShipments | syncShipments (/Actindo.Extensions.Actindo.UCSProductSync.OrderStatusSync.syncShipments)


### Create invoice 

![Create invoice](../Assets/Screenshots/ProcessDocumentation/CreateInvoice.png "[Create invoice]")

The *Create invoice* action is used to copy the document and create a document specified in the static inputs from the input document.
In this template case, the incoming delivery note is copied. Via the *origin* output port, the copied original document, that is the delivery note, is output. Via the *data* output port, an invoice is output. The destination type of the document which is output via the *data* output port is specified in the *Destination type* static input.

#### Settings

The *Description* field contains the API endpoint that is addressed in this action. The *Key*, *Label*, *Queue type* and *Max tries* field have no functional meaning for the action.  

- *Description*   
  .copy | Create a copy of the given business document (/Actindo.Modules.RetailSuite.RetailSuiteFaktBase.BusinessDocuments.copy)

**Static inputs**

- *Destination type*   
  "RE"

Other static inputs are not defined.


### Post invoice to accounting

![Post invoice to accounting](../Assets/Screenshots/ProcessDocumentation/PostInvoiceToAccounting.png "[Post invoice to accounting]")

The *Post invoice to accounting* action is used to post the document, dependent on the document type, in the internal accounting and/or warehousing system. In this template case, the invoice is posted in the *Accounting* module.

#### Settings

The *Description* field contains the API endpoint that is addressed in this action. The *Key*, *Label*, *Queue type* and *Max tries* field have no functional meaning for the action.  

- *Description*   
  .post | Post a business document to stock and/or accounting (/Actindo.Modules.RetailSuite.RetailSuiteFaktBase.BusinessDocuments.post)

**Static inputs**

No static inputs defined.



### Ship the order 

To ship an order, the following actions are required:
- Duplicate input action
- Execute PHP code
- Create dispatch
- Export dispatch to LSP
- Wait for dispatch note update
- Wait for parallel input
- Sync shipments


### Duplicate input action

![Duplicate input action](../Assets/Screenshots/ProcessDocumentation/DuplicateInputAction.png "[Duplicate input action]")

The *Duplicate input action* action is used to duplicate the input and output it via two different output ports. In this template case, the delivery note is duplicated and output via both ports.

#### Settings

The *Description* field contains the API endpoint that is addressed in this action. The *Key*, *Label*, *Queue type* and *Max tries* field have no functional meaning for the action.  

- *Description*   
  Multiply input action


### Build request

![Build request](../Assets/Screenshots/ProcessDocumentation/BuildRequest.png "[Build request]")

The *Build request* action is used to determine the delivery country in the invoice and, depending on whether the delivery country is Germany or a foreign country, output the invoice in a different output port. By doing so, a different logistics service provider (LSP) can be specified for domestic and foreign deliveries.

#### Settings

The *Description* field contains the API endpoint that is addressed in this action. The *Key*, *Label*, *Queue type* and *Max tries* field have no functional meaning for the action.  

- *Description*   
  Execute PHP Code

**Configuration**

- *PHP code*   
  ```php
  <?php
  $connectionId = $in0->getForceLagerGroupId() == 50 ? 1 : 11;
  $ret = new \___WorkflowAutogen___\RequestHydration\Modules\Actindo\Fulfillment\Models\DispatchNoteContainerCreate(['businessDocument' => ['id' => $in0->getId()],'connection' => ['id' => $connectionId]]);
  return $connectionId==1 ?  [$ret] : [null, $ret];
  ?>
  ```

**Static inputs**

No static inputs defined.


### Create dispatch

![Create dispatch](../Assets/Screenshots/ProcessDocumentation/CreateDispatch.png "[Create dispatch]")

The *Create dispatch* action is used to create and persist a dispatch note in the *Fulfillment* module from the delivery note. The data are mapped via ETL.

#### Settings

The *Description* field contains the API endpoint that is addressed in this action. The *Key*, *Label*, *Queue type* and *Max tries* field have no functional meaning for the action.  

- *Description*   
  .create | Creates and persists a new dispatch note from an existing business document. (/Actindo.Modules.Actindo.Fulfillment.DispatchNotes.create)

**Static inputs**

No static inputs defined.


### Export dispatch to LSP

![Export dispatch to LSP](../Assets/Screenshots/ProcessDocumentation/ExportDispatchToLSP.png "[Export dispatch to LSP]")

The *Export dispatch to LSP* action is used to export the dispatch note through its configured driver in the *Fulfillment* module to the logistics service provider (LSP).

#### Settings

The *Description* field contains the API endpoint that is addressed in this action. The *Key*, *Label*, *Queue type* and *Max tries* field have no functional meaning for the action.  

- *Description*   
  .export | Exports the dispatch note through its configured fulfillment driver (/Actindo.Modules.Actindo.Fulfillment.DispatchNotes.export)


### Wait for dispatch note update

![Wait for dispatch note update](../Assets/Screenshots/ProcessDocumentation/WaitForDispatchNoteUpdate.png "[Wait for dispatch note update]")

The *Wait for dispatch note update* action is used to wait for the feedback from the logistics service provider (LSP) that the order has been shipped. The status is retrieved in a predefined time interval. 

#### Settings

The *Description* field contains the API endpoint that is addressed in this action. The *Key*, *Label*, *Queue type* and *Max tries* field have no functional meaning for the action.  

- *Description*   
  Wait for dispatch note update


### Wait for parallel input

![Wait for parallel input](../Assets/Screenshots/ProcessDocumentation/WaitForParallelInput.png "[Wait for parallel input]")

The *Wait for parallel input* action is used to wait for two inputs to be received by the action before executing the action. In this template case, the action awaits the delivery note and the dispatch note and outputs the delivery note.

#### Settings

The *Description* field contains the API endpoint that is addressed in this action. The *Key*, *Label*, *Queue type* and *Max tries* field have no functional meaning for the action.  

- *Description*   
  Wait for parallel input


### Sync shipments

![Sync shipments](../Assets/Screenshots/ProcessDocumentation/SyncShipments02.png "[Sync shipments]")

The *Sync shipments* action is used to change the *shipment* entity status to **closed**. Depending on the driver of the connection, the channel is updated asynchronously.

#### Settings

The *Description* field contains the API endpoint that is addressed in this action. The *Key*, *Label*, *Queue type* and *Max tries* field have no functional meaning for the action.  

- *Description*   
  .syncShipments | syncShipments (/Actindo.Extensions.Actindo.UCSProductSync.OrderStatusSync.syncShipments)


