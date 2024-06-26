[!!Manage a product](../PIM/Operation/01_ManageProducts.md)
[!!Manage the connections](../Channels/Integration/01_ManageConnections.md)
[!!Manage a workflow](../ActindoWorkFlow/Operation/01_ManageWorkflows.md)
[!!Manage the triggers](../ActindoWorkFlow/Operation/02_ManageTriggers.md)

# Introduction

The *Actindo Core1 Platform* can create an offer automatically in the *Omni-Channel* module for every product managed in the *PIM* module. From *Omni-Channel*, the offer is then transferred to one or multiple connected sales channels. You can automate this process by creating a workflow in the *Process Orchestration* module.

This *Omni-Channel offer cookbook* documentation intends to provide you with detailed instructions to configure your own workflows. It contains the following information:

- An overview of the main components you need to create an offer from product workflow
- A detailed description of the procedures involved
- A few workflow examples, from the most basic to most complex use cases
- JSON templates for every workflow example provided

In this chapter, the basic setup procedures for an offer from product workflow are described: 

- [Set up an offer from product workflow](#set-up-an-offer-from-product-workflow)
- [Create a PIM product trigger](#create-a-pim-product-trigger)
- [Add a condition to a PIM product trigger](#add-a-condition-to-a-pim-product-trigger)


## Set up an offer from product workflow

To set up a workflow, you have to create a new workflow and define the basic settings first.   

#### Prerequisites

- You have created a *PIM* product, see [Create a product](../PIM/Operation/01_ManageProducts.md#create-a-product).
- You have created a connection to a sales channel, see [Create a connection](../Channels/Integration/01_ManageConnections.md#create-a-connection).

#### Procedure

*Process Orchestration > Workflows > Tab OVERVIEW*

![Workflows](../Assets/Screenshots/ActindoWorkFlow/Workflows/Workflows.png "[Workflows]")

1. See [Define workflow basic settings](../ActindoWorkFlow/Operation/01_ManageWorkflows.md#define-the-workflow-basic-settings) in the *Process Orchestration* documentation for a general description.

2. Create a workflow and define the following workflow basic settings:

| Field | Value |
| ------- | ----- |
| *Select a name for your new workflow* | Create offer from complete PIM product |
| *Select a unique key for your new workflow* | create_offer_from_complete_pim_product |
| *Choose the data type of your start place* |   \_\_\_WorkflowAutogen___\Actindo\Modules\Actindo\PIM\Models\PIMProduct |
| *Choose the data type of your end place* | Arbitrary Data |



## Create a PIM product trigger

A trigger is the combination of a business object, such as a *PIM* product, and an event that initiates a process, that is, the execution of the workflow. You need to define a trigger for a process to start automatically every time a certain scenario takes place. Otherwise, your workflow will only be executed once.

For the offer from product workflow, two types of triggers apply: 

1. *PIM product created*: to initiate your process every time a product is created
2. *PIM product saved*: to initiate your process every time a product is changed and saved

You can add several triggers to a workflow. Bear in mind that the triggers work as a priority list, that is, a list of items arranged in descending order based on their priority. Therefore, the correct order of the triggers is crucial, as the system goes through the triggers in the order they are listed, starting from the top, and stops checking them as soon as a matching trigger is found. That means that the triggers must be organized from specific to general to cover all possible relevant cases.
 
#### Prerequisites

You have set up an offer from product workflow, see [Set up an offer from product workflow](#set-up-an-offer-from-product-workflow).

#### Procedure

*Process Orchestration > Workflows > Tab OVERVIEW > Select offer from product workflow > Select workflow version*

![Workflow editor](../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowEditor.png "[Workflow editor]")

1. See [Create a trigger](../ActindoWorkFlow/Operation/02_ManageTriggers.md#create-a-trigger) in the *Process Orchestration* documentation for a general description.

2. Create a trigger and configure the following settings depending on the trigger you want to use:

    1. *PIM product saved* trigger

        ![PIM product saved](../Assets/Screenshots/OfferCookbook/PIMProductSavedTrigger.png "[PIM product saved]")

        **Triggers**

        | Field | Value | Comments | 
        |---------|-------|----------| 
        |*Name* | PIM product saved |  |
        |*Model* | Actindo\Modules\Actindo\PIM\Models\PIMProduct | Path to data model, for example Actindo.Modules.PIM.Models.PIMProduct. For a list of data models, go to *Dev Tool > API > Data models*. |
        |*Event* | After saving | The workflow is triggered every time a product is saved in *PIM*. |
        |*Condition fulfillment* | If all are met |    |
        |*Status* | Active |  |
        |*Process priority* | 10 | |
        | *Unique check* | No |  |

    2. *PIM product created* trigger

        ![PIM product created](../Assets/Screenshots/OfferCookbook/PIMProductCreatedTrigger.png "[PIM product saved]")
        
        **Triggers**

        | Field | Value | Comments | 
        |---------|-------|----------|
        |*Name* | PIM product created |  |
        |*Model* | Actindo\Modules\Actindo\PIM\Models\PIMProduct | Path to data model, for example Actindo.Modules.PIM.Models.PIMProduct. For a list of data models, go to *Dev Tool > API > Data models*. |
        |*Event* | After creating | The workflow is triggered every time a product is created in *PIM*. |
        |*Condition fulfillment* | If all are met |  |
        |*Status* | Active |  |
        |*Process priority* | 10 |  |
        |*Unique check* | No | |

[comment]: <> (add in comments column: Model: path to data model, process priority + unique check refer to whole process -> or better add it to triggers in Process Orchestration doc)

3. If desired, you can add conditions to a trigger to define more precisely when a process is executed, see [Add a condition to a PIM product trigger](#add-a-condition-to-a-pim-product-trigger).

[comment]: <> (Unique check bezieht sich hier auf Prozess, also Prozess wird nur einmal für ein bestimmtes Produkt durchgeführt, wenn Setting auf Ja gesetzt, egal was man ändert und wie viel man was ändert.)

## Add a condition to a PIM product trigger

You can add conditions to a trigger to define more precisely when a process is executed.  

In the case of the offer from product workflow, for example, you can determine that a new process is started only when a *PIM* product is saved (trigger) and it is put on sale (condition). This means that a new offer will be created in *Omni-Channel* only when the *PIM* product is marked as a sale item (the *Sale item* toggle in the *Product data* is enabled) and saved. 

You can add several conditions to a trigger. Depending of the trigger *Condition fulfillment* setting, only one (**if any is met**) or all (**if all are met**) conditions will apply. 

#### Prerequisites

You have created a *PIM* product trigger, see [Create a PIM product trigger](#create-a-pim-product-trigger).

#### Procedure

*Process Orchestration > Workflows > Tab OVERVIEW > Select offer from product workflow > Select workflow version > Button Points > Menu entry Triggers*

![Condition product on sale](../Assets/Screenshots/OfferCookbook/ConditionChangeSetPimIsSale.png "[Condition product on sale]")

1. See [Add a condition](../ActindoWorkFlow/Operation/02_ManageTriggers.md#add-a-condition) in the *Process Orchestration* documentation for a general description.

2. Select the trigger to which you want to add a condition.

3. Add a condition and configure the following settings:

**Conditions** 

| Field | Value | Comments | 
|---------|-------|----------|
|*Prefix* | changeset. |  |
|*Property* | _pim_is_sale |  |
|*Operator* | Is set  | When selecting **Is set**, the toggle is automatically enabled.  |
|*Value* | - |   |





