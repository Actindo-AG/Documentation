# Introduction

After a product has been created in the *PIM* module, an offer for that product can be created automatically in the *Omni-Channel* module. From the *Omni-Channel* module, the offer will then be transferred to one or multiple connected sales channels. You can automate this process by using the *Process Orchestration* module and building a workflow...


## Main entities and actions involved

### Entities

**PIM product**  
A *PIM* product is ... 

For detailed information, see [Manage a product](../PIM/Operation/01_ManageProducts.md).  

**Omni-Channel connection**  
A *Omni-Channel* connection is ... 
For detailed information, see [Manage the connections](../Channels/Integration/01_ManageConnections.md).


### Actions

Endpoints 

Core actions, see [Core actions](../ActindoWorkFlow/UserInterface/08_CoreActions.md)

---

Links to Process Orchestration

[comment]: <> (check wenn Struktur geändert!)

[Create a workflow](../ActindoWorkFlow/Operation/01_ManageWorkflows.md#create-a-workflow)  
[Define the workflow basic settings](../ActindoWorkFlow/Operation/01_ManageWorkflows.md#define-the-workflow-basic-settings)  
[Create a trigger](../ActindoWorkFlow/Operation/02_ManageTriggers.md#Create-a-trigger)  

[Add a condition](../ActindoWorkFlow/Operation/02_ManageTriggers.md#Add-a-condition) 

[Add a transition](../ActindoWorkFlow/Operation/01_ManageWorkflows.md#add-a-transition)  

[Insert a static input](../ActindoWorkFlow/Operation/06_InsertStaticInput.md)  


## Set up an offer from product workflow

To set up a workflow, you have to create a new workflow and define the basic settings first.   

#### Prerequisites

- You have created a *PIM* product, see [Create a product](../PIM/Operation/01_ManageProducts.md#create-a-product).
- You have created a connection to a sales channel, see [Create a connection](../Channels/Integration/01_ManageConnections.md#create-a-connection).

#### Procedure

*Process Orchestration > Workflows > Tab OVERVIEW*

![Workflows](../Assets/Screenshots/ActindoWorkFlow/Workflows/Workflows.png "[Workflows]")

1. See [Define workflow basic settings](../ActindoWorkFlow/Operation/01_ManageWorkflows.md#define-the-workflow-basic-settings) for a general description.

2. Create a workflow and define the following workflow basic settings:

| Setting | Value |
| ------- | ----- |
| *Select a name for your new workflow* | Create offer from complete PIM product |
| *Select a unique key for your new workflow* | create_offer_from_complete_pim_product |
| *Choose the data type of your start place* |   \_\_\_WorkflowAutogen___\Actindo\Modules\Actindo\PIM\Models\PIMProduct |
| *Choose the data type of your end place* | Arbitrary Data |

[comment]: <> (Warum nicht end place Channels.Offer?)



## Create a PIM product trigger

A trigger is the combination of a business object, such as a *PIM* product, and an event that initiates a process, that is, the execution of the workflow. You need to define a trigger for a process to start automatically every time a certain scenario takes place. Otherwise, your workflow will only be executed once.

For the offer from product workflow, two main types of triggers apply: 

1. *PIM product created*: to initiate your process every time a product is created
2. *PIM product saved*: to initiate your process every time a product is changed and saved

#### Prerequisites

You have have set up an offer from product workflow, see [Set up an offer from product workflow](#set-up-an-offer-from-product-workflow).

#### Procedure

*Process Orchestration > Workflows > Tab OVERVIEW > Select the offer from product workflow > Select a workflow version*

![Workflow editor](../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowEditor.png "[Workflow editor]")

1. See [Create a trigger](../ActindoWorkFlow/Operation/01_ManageWorkflows.md#define-the-workflow-basic-settings) for a general description.

2. Create a trigger and configure the following settings depending on the trigger you want to use:

    1. *PIM product saved* trigger

        ![PIM product saved](../Assets/Screenshots/OfferCookbook/PIMProductSavedTrigger.png "[PIM product saved]")

        | Triggers ||
        |----|----|
        |**Name** | PIM product saved |
        |**Model** | Actindo\Modules\Actindo\PIM\Models\PIMProduct |
        |**Event** | After saving | 
        |**Condition fulfillment** | If all are met |   
        |**Status** | Active |
        |**Process priority** | 10 | 
        | **Unique check** | No |

    2. *PIM product created* trigger

        ![PIM product created](../Assets/Screenshots/OfferCookbook/PIMProductCreatedTrigger.png "[PIM product saved]")

        | Triggers ||
        |----|----|
        |**Name** | PIM product created |
        |**Model** | Actindo\Modules\Actindo\PIM\Models\PIMProduct |
        |**Event** | After creating | 
        |**Condition fulfillment** | If all are met |   
        |**Status** | Active |
        |**Process priority** | 10 | 
        | **Unique check** | No |

3. If desired, you can add conditions to it to define more precisely when a process is executed, see [Add a condition](#add-a-condition).



## Add a condition

[comment]: <> (Letztes Mal hat es nicht funktioniert. Mit Stefan prüfen)

You can add conditions to your triggers to define more precisely when a process is executed.  

In the case of the offer from product workflow, for example, you can determine that a new process is started only when a *PIM* product is saved and, for example, it is put on sale. This means that a new offer will be created in *Omni-Channel* only when the product price in the *PIM* module has been changed. 

[comment]: <> (if the price has been modified, -> Ist das möglich mit _pim_price? Und was wäre Value? Oder mit Is set?)

You can add several conditions to a trigger. 

#### Prerequisites

You have created a *PIM* product trigger, see [Create a PIM product trigger](#create-a-pim-product-trigger).

#### Procedure

*Process Orchestration > Workflows > Tab OVERVIEW > Select offer from product workflow > Select a workflow version > Button Points > Menu entry Triggers*

![Workflow editor](../Assets/Screenshots/OfferCookbook/ConditionPimPriceSale.png "[Workflow editor]")

> [Info] You have to select the trigger to which you want to add a condition.

1. See [Add a condition](../ActindoWorkFlow/Operation/02_ManageTriggers.md#Add-a-condition) for a general description.

2. Add a condition and configure the following settings:

| Conditions ||
|----|----|
|**Prefix** | changeset. |
|**Property** | $entity._pim_price_sale |
|**Operator** | Is set | 
|**Value** | - |   
   
[comment]: <> (check!)



## Possible workflow variations

