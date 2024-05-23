# Introduction

After a product has been created in the *PIM* module, an offer for that product can be created automatically in the *Omni-Channel* module. From the *Omni-Channel* module, the offer will then be transferred to one or multiple connected sales channels. You can automate this process by using the *Process Orchestration* module and building a workflow...


## "Ingredients"

Entities and actions involved


Links to Process Orchestration

[Create a workflow](../ActindoWorkFlow/Operation/01_ManageWorkflows.md#create-a-workflow)
[Define the workflow basic settings](../ActindoWorkFlow/Operation/01_ManageWorkflows.md#define-the-workflow-basic-settings)
[Add a transition](../ActindoWorkFlow/Operation/01_ManageWorkflows.md#add-a-transition)


## How to set up an offer from product basic workflow



To set up a workflow, you have to create a new workflow and define the basic settings first. For detailed information, see [Define workflow basic settings](../ActindoWorkFlow/Operation/01_ManageWorkflows.md#define-the-workflow-basic-settings). 

For detailed information on how to create a workflow, see [Create a workflow](../ActindoWorkFlow/Operation/01_ManageWorkflows.md#create-a-workflow).

#### Prerequisites

- You have created a *PIM* product, see [Create a product](../PIM/Operation/01_ManageProducts.md#create-a-product).
- You have created a connection to a sales channel, see [Create a connection](../Channels/Integration/01_ManageConnections.md#create-a-connection).

#### Procedure

*Process Orchestration > Workflows > Tab OVERVIEW*

![Workflows](../Assets/Screenshots/ActindoWorkFlow/Workflows/Workflows.png "[Workflows]")

1. Click the ![Add](../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    The *New workflow* window is displayed.

    ![New workflow](../Assets/Screenshots/ActindoWorkFlow/Workflows/NewWorkflow.png "[New workflow]")

2. Enter **Create offer from complete PIM product** in the *Select a name for your new workflow* field.

3.  Enter **create_offer_from_complete_pim_product** in the *Select a unique key for your new workflow* field. The key is required for API access and must be unique within the workflow version.

4.  Select the **___WorkflowAutogen___\Actindo\Modules\Actindo\PIM\Models\PIMProduct** option as start place type in the *Choose the data type of your start place* field.

5. Select the **Arbitrary Data** option as end place type in the *Choose the data type of your end place* field.

6. Click the [CREATE] button in the bottom right corner.   
    The new workflow has been created. The *New workflow* window is closed. The workflow editor with the defined start and end places is displayed.



## PIM product saved trigger

Was ist ein Trigger
Wann wird es verwendet
Warum product saved trigger

#### Prerequisites

You have have set up the basic workflow, see [Set up the basic workflow](#set-up-the-basic-workflow).

#### Procedure

![PIM product saved trigger](../Assets/Screenshots/OfferCookbook/PIMProductSavedTrigger.png "[PIM product saved trigger]")

1. Select the newly created workflow to edit it. For detailed information, see [Edit a workflow](../ActindoWorkFlow/Operation/01_ManageWorkflows.md#edit-a-workflow).   
    The workflow editor is displayed.

2. Create a *PIM Product saved* trigger to create an offer when a product is updated.  
    A new trigger input line is displayed.

    For detailed information on how to create a trigger, see [Create a trigger](../ActindoWorkFlow/Operation/03_ManageTriggers.md#create-a-trigger).

3. Configure the following settings for the *PIM Product saved* trigger:

    | Triggers ||
    |----|----|
    |**Name** | PIM product saved |
    |**Model** | Actindo\Modules\Actindo\PIM\Models\PIMProduct |
    |**Event** | After saving | 
    |**Condition fulfillment** | If all are met |   
    |**Status** | Active |
    |**Process priority** | 10 | 
    | **Unique check** | No |


# PIM product created trigger

Was ist ein Trigger
Wann wird es verwendet
Warum product created trigger

#### Prerequisites

You have have set up the basic workflow, see [Set up the basic workflow](#set-up-the-basic-workflow).

#### Procedure

![PIM product created trigger](../Assets/Screenshots/OfferCookbook/ "[PIM product created trigger]")

1. Select the newly created workflow to edit it. For detailed information, see [Edit a workflow](../ActindoWorkFlow/Operation/01_ManageWorkflows.md#edit-a-workflow).   
    The workflow editor is displayed.

2. Create a *PIM Product created* trigger to create an offer when a product is created.  
    A new trigger input line is displayed.

    For detailed information on how to create a trigger, see [Create a trigger](../ActindoWorkFlow/Operation/03_ManageTriggers.md#create-a-trigger).

3. Configure the following settings for the *PIM Product saved* trigger:

    | Triggers ||
    |----|----|
    |**Name** | PIM product created |
    |**Model** | Actindo\Modules\Actindo\PIM\Models\PIMProduct |
    |**Event** | After creating | 
    |**Condition fulfillment** | If all are met |   
    |**Status** | Active |
    |**Process priority** | 10 | 
    | **Unique check** | No |


## Potential workflow extensions

