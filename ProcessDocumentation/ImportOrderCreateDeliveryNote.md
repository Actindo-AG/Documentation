# Import order and create delivery notes

![Import order and create delivery notes](../Assets/Screenshots/ProcessDocumentation/ImportChannelsOrderInOMSAndCreateDeliveryNotes.png "[Import order and create delivery notes]")

The *Import order and create delivery note* workflow is used to import orders from the *Omni-Channel* module to the *Order management* module, generate a leading document and, if required, a delivery note and trigger the further delivery process. The delivery process is handled in the subordinate [*Handle delivery note*](./HandleDeliveryNote.md) workflow. The aim of this process is to import the order to the *Order management* module. The process is triggered as soon as an order is completely imported from the channel (marketplace or webshop) to *Omni-Channel*.

In a first step, the order is imported to the *Order management* module and a leading document is created. The type of the document depends on the type which is defined by customer in the ETL mapping. Mostly, an order confirmation or a cash invoice for POS is created.
If a cash invoice has been created, no further steps are required, as no delivery is necessary. If needed, a payment sync from the *Venduo POS* module to the *Accounting* module can be performed, otherwise, the workflow ends with the cash invoice. 
If an order confirmation or any other document than a cash invoice has been created as a leading document, this document is further processed. Depending on whether a payment is required for further processing, either the receipt of payment is awaited or the document is processed regardless of payment. Anyway, a delivery note is created and the subordinate [*Handle delivery note*](./HandleDeliveryNote.md) workflow is started. The delivery note is important to handle that the order leaves the warehouse and is delivered, because the leading document only reserves the stock in the warehouse.
At the end of this process, the order has been processed and the delivery process has been triggered.


## How to set up an order import workflow

After an order has been placed in a webshop or on a marketplace and imported to the *Omni-Channel* module, this order can be further processed in Actindo. 
You can automate this process by using the *Workflows* module and building a workflow that is handling all processes after the import up to the delivery. As each workflow can be customized, it is possible to include or exclude different processes depending on the customers needs.
In the following, it is described how to build a workflow template that is covering the processes below:
- Order export from *Omni-Channel* to *Order management*
- Delivery note creation


#### Prerequisites

- The *Accounting* module is configured.
- The *Taxes* module is configured.
- The products are created in the *PIM* module. 
- A connection to the channel (marketplace or webshop) is configured in the *Omni-Channel* module and the offers to the products are created.


#### Procedure

*Workflows > Workflows > Tab OVERVIEW*

![Workflows](../Assets/Screenshots/ActindoWorkFlow/Workflows/Workflows.png "[Workflows]")

1. Click the ![Add](../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The *New workflow* window is displayed.

  ![New workflow](../Assets/Screenshots/ActindoWorkFlow/Workflows/NewWorkflow.png "[New workflow]")

2. Enter **Import channels order in OMS and create Delivery Notes** in the *Select a name for your new workflow* field.

3. Enter **create_delivery_notes** in the *Select a unique key for your new workflow* field. The key is required for API access and must be unique within the workflow version.

4. Select the **___WorkflowAutogen___\Actindo\Modules\Actindo\Channels\Models\Order** option as start place type in the *Choose the data type of your start place* field.

  > [Info] Enter a keyword in the field, for example **order**, to limit the data types displayed in the list. The list of data types is filtered for your keyword as you type.

5. Select the **___WorkflowAutogen___\Actindo\Modules\RetailSuite\RetailSuiteFaktBase\Models\BusinessDocument** option as end place type in the *Choose the data type of your end place* field.

  > [Info] Enter a keyword in the field, for example **business**, to limit the data types displayed in the list. The list of data types is filtered for your keyword as you type.

6. Click the [CREATE] button in the bottom right corner.   
  The new workflow has been created. The *New workflow* window is closed. The workflow editor with the defined start and end places is displayed.  

  ![Workflow editor new](../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowEditorNew.png "[Workflow editor new]")

7. In a new window, open the JSON library for workflows and copy the JSON code for the *Import channels order in OMS and create Delivery Notes* workflow to your clipboard, see [JSON Import channels order in OMS and create Delivery Notes](./ImportOrderCreateDeliveryNote.json).

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


## Description of the *Import order and create delivery notes* process

Within a workflow, several actions are performed. If a certain number of actions are executed in a specific order with a common objective that can only be achieved by executing all of these actions, we speak of a so-called *snippet*. 
In the following, all snippets and single actions within the process as well as their start and end place are described in detail, specifying their function and settings.


### Start place

As soon as an order is completely imported from the channel (marketplace or webshop) to *Omni-Channel*, the *Import order and create delivery note* process is triggered. The order is put in the start place.

#### Settings

- *Key*     
  Input

- *DataContainer*   
  Modules.Actindo.Channels.Models.Order


### Import an order to OMS

To import an order from the *Omni-Channel* module to the *Order management* module, the following four actions are required:
- Setup order for export
- Export base order
- Export positions
- Finish order export


### Setup order for export    

![Setup order for export](../Assets/Screenshots/ProcessDocumentation/SetupOrderExport.png "[Setup order for export]")

The *Setup order for export* action is used to prepare the order in the *Omni-Channel* module to be exported to the *Order management* module.

#### Settings

- *Description*   
  .setupOrderExport | setting up ucssync order to be exported (/Actindo.Extensions.Actindo.UCSProductSync.RetailSuiteOrderSync.setupOrderExport)

- *Key*    
  t-Extensions.Actindo.UCSProductSync.RetailSuiteOrderSync.setupOrderExport-0

- *Label*    
  setupOrderExport

- *Queue type*   
  Default

- *Max tries*
  1


### Export base order

![Export base order](../Assets/Screenshots/ProcessDocumentation/ExportBaseOrder.png "[Export base order]")

The *Setup order for export* action is used to export the document header, for example customer data to create a new customer if not yet registered, and to assign the document number to the leading document.

#### Settings

- *Description*   
  .exportBaseOrder | exportBaseOrder (/Actindo.Extensions.Actindo.UCSProductSync.RetailSuiteOrderSync.exportBaseOrder)

- *Key*    
  t-Extensions.Actindo.UCSProductSync.RetailSuiteOrderSync.exportBaseOrder-0

- *Label*    
  exportBaseOrder

- *Queue type*   
  Default

- *Max tries*
  1


### Export positions

![Export positions](../Assets/Screenshots/ProcessDocumentation/ExportPositions.png "[Export positions]")

The *Setup order for export* action is used to export the item data of the order and to determine from which warehouse the items are taken.

#### Settings

- *Description*   
  .exportPositions | exportPositions (/Actindo.Extensions.Actindo.UCSProductSync.RetailSuiteOrderSync.exportPositions)

- *Key*    
  t-Extensions.Actindo.UCSProductSync.RetailSuiteOrderSync.exportPositions-0

- *Label*    
  exportPositions

- *Queue type*   
  Default

- *Max tries*
  1


### Finish order export

![Finish order export](../Assets/Screenshots/ProcessDocumentation/FinishOrderExport.png "[Finish order export]")

The *Finish order export* action is used to finish the order export to OMS and post the leading document. Most of the time, this leading document is a cash invoice or an order confirmation, but in general, the customer can define the type of document individually in the ETL mapping.

#### Settings

- *Description*   
  .finishExport | finishExport (/Actindo.Extensions.Actindo.UCSProductSync.RetailSuiteOrderSync.finishExport)

- *Key*    
  t-Extensions.Actindo.UCSProductSync.RetailSuiteOrderSync.finishExport-0

- *Label*    
  finishOrderExport

- *Queue type*   
  Default

- *Max tries*
  1



### Finalize cash invoice or create delivery note

To finalize the document in case of a cash invoice or to create a delivery note for any other document type, the following four actions are required:
- Split AB, RB; Prepare Allow Dispatch
- Allow dispatch
- Create deliveries
- Start subprocess 


### Split AB, RB; Prepare Allow Dispatch

![Execute PHP Code](../Assets/Screenshots/ProcessDocumentation/ExecutePHPCode.png "[Execute PHP Code]")

The *Split AB, RB; Prepare Allow Dispatch* action is used to determine the type of document and, depending on the document type, output the document in a different output port. By doing so, different ways can be specified for the different document types.
The  corresponding PHP code defining which document types are being output via which output port must be entered in the *Configuration* section of the action settings. In this template case, cash invoices are output via the output port 0, all other document types via the output port 1. By this distinction, the cash invoice can be directly finalized whereas the any other document types trigger the delivery note creation and the related processing. 
Further, a request is build to set the *dispatch allowed* field to **true**. 

#### Settings

- *Description*   
  Execute PHP Code

- *Key*    
  t-executePHP-0

- *Label*    
  Split AB, RB; Prepare Allow Dispatch

- *Queue type*   
  Default

- *Max tries*
  1

 **Configuration**

- *PHP code*    
  ```php
  <?php
  $in0->setDispatchAllowed(true);
  $ret = new \___WorkflowAutogen___\RequestHydration\Modules\RetailSuite\RetailSuiteFaktBase\Models\BusinessDocumentContainerChange($in0);
  $ret->setSerializableFields(['id','dispatchAllowed']);
  return $in0->getType() != 'RB' ? [$ret] : [null, $in0];
  ?>
  ```

**Static inputs**

No static inputs defined.


### Allow dispatch

![Allow dispatch](../Assets/Screenshots/ProcessDocumentation/AllowDispatch.png "[Allow dispatch]")

The *Allow dispatch* action is used to save the changes on the document requested in the preceding *Split AB, RB; Prepare Allow Dispatch* action. The field *Dispatch allowed* in the document is changed to **true** to allow the further delivery note creation.

#### Settings

- *Description*   
  .save | Save changes on a business document (/Actindo.Modules.RetailSuite.RetailSuiteFaktBase.BusinessDocuments.save)

- *Key*    
  t-Modules.RetailSuite.RetailSuiteFaktBase.BusinessDocuments.save-0

- *Label*    
  Allow Dispatch

- *Queue type*   
  Default

- *Max tries*
  1


### Create deliveries

![Create  deliveries](../Assets/Screenshots/ProcessDocumentation/CreateDeliveries.png "[Create deliveries]")

The *Create deliveries* action is used to create the delivery note/s. For each (partial) delivery, a single delivery note is created in the *Order management* module. The delivery note is necessary to trigger that the order will leave the warehouse. 

#### Settings

- *Description*   
  .createDelivery | Create a delivery (delivery notes or dropship delivery notes) for a business document (/Actindo.Modules.RetailSuite.RetailSuiteFaktBase.BusinessDocuments.createDelivery)

- *Key*    
  t-Modules.RetailSuite.RetailSuiteFaktBase.BusinessDocuments.createDelivery-0

- *Label*    
  createDeliveries

- *Queue type*   
  Default

- *Max tries*
  1

**Static inputs**

No static inputs defined.


### Start subprocess 

![Start subprocess](../Assets/Screenshots/ProcessDocumentation/StartSubprocess.png "[Start subprocess]")

The *Start subprocess* action is used to start the process specified in the configuration as a subprocess. In this template case, the [*Handle delivery note*](./HandleDeliveryNote.md) subprocess is started to handle the further delivery processing. Define the key of the workflow you want to start as a subprocess in the configuration. For each delivery note, a single subprocess will be started. The delivery note is transferred to the start place of the subprocess.

#### Settings

- *Description*   
  Start Subprocess

- *Key*    
  t-startSubprocess-0

- *Label*    
  Start Subprocess

- *Queue type*   
  Default

- *Max tries*
  1
  
**Configuration**

- *Workflow Key*   
  delivery_notes



### End place

The process is completed as soon as one or multiple delivery notes and or the cash invoice have been created and put in the end place.

#### Settings
 
- *Key*     
  Output

- *DataContainer*   
  Modules.RetailSuite.RetailSuiteFaktBase.Models.BusinessDocument