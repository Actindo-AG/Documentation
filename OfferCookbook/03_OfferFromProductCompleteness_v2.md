# Create offer from product with completeness

![Offer from product with completeness](../Assets/Screenshots/OfferCookbook/OfferFromProductCompleteness.png "[Offer from product with completeness]")

## Overview

You want to create an *Omni-Channel* offer when all required attributes of a *PIM* product are set (total completeness is 100 %).

| **Summary** |       |
| ----------- |------ |
| **Purpose** | Create an *Omni-Channel* offer from a *PIM* product with 100% completeness |
| **Affected entities** | Modules.Actindo.PIM.Models.PIMProduct <br> Actindo.Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct |
| **Included plugins** | *Process Orchestration* <br> *PIM* <br> *Omni-Channel* |
| **Included third party software** | none/optional | 
| **Trigger** | The process is triggered by the creation or the update of a *PIM* product. |

**Included steps**

- Verification if a *PIM* product completeness is 100 %
- Creation of an *Omni-Channel* for a PIM product 

**Necessary actions**

| Action | Short description | API endpoint |
| ------ | ----------------- | ------------ |
| split by criterion | Input value is compared to a criterion and split based on match/no match principle | Core action |
| createFromPimProduct  | Create an offer from a product | /Actindo.Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct |

For a detailed description of the core actions, see [Core actions](../ActindoWorkFlow/UserInterface/08_CoreActions.md) in the *Process Orchestration* documentation.


## How to set up an offer from product workflow

To set up any workflow, you have to create a new workflow and define the basic settings first. For detailed information, see [Define workflow basic settings](../ActindoWorkFlow/Operation/01_ManageWorkflows.md#define-the-workflow-basic-settings). 

For detailed information on how to create a workflow, see [Create a workflow](../ActindoWorkFlow/Operation/01_ManageWorkflows.md#create-a-workflow).

[comment]: <> (gleich für alle! Unter Basic und darauf verweisen!)

#### Prerequisites

- You have created a *PIM* product, see [Create a product](../PIM/Operation/01_ManageProducts.md#create-a-product).
- You have created a connection to a sales channel, see [Create a connection](../Channels/Integration/01_ManageConnections.md#create-a-connection).

#### Procedure

*Process Orchestration > Workflows > Tab OVERVIEW*

![Workflows](../Assets/Screenshots/ActindoWorkFlow/Workflows/Workflows.png "[Workflows]")

Create a new workflow and define the following workflow basic settings: 

| Setting | Value |
| ------- | ----- |
| *Select a name for your new workflow* | Create offer from complete PIM product |
| *Select a unique key for your new workflow* | create_offer_from_complete_pim_product |
| *Choose the data type of your start place* |   \_\_\_WorkflowAutogen___\Actindo\Modules\Actindo\PIM\Models\PIMProduct |
| *Choose the data type of your end place* | Arbitrary Data |

For detailed information on how to create a workflow, see [Define the workflow basic settings](../ActindoWorkFlow/Operation/01_ManageWorkflows.md#define-the-workflow-basic-settings).

[comment]: <> (Warum nicht end place Channels.Offer?)



## Description of the offer from product with completeness workflow

Once you have set up a basic workflow, you can edit it to add the necessary steps. For detailed information on setting up the basic workflow, see [Set up the basic workflow](#set-up-the-basic-workflow).

Click on the workflow you want to edit, see [Edit a workflow](../ActindoWorkFlow/Operation/01_ManageWorkflows.md#edit-a-workflow).

### Product saved trigger

![PIM product saved trigger](../Assets/Screenshots/OfferCookbook/PIMProductSavedTrigger.png "[PIM product saved trigger]")

1. Create a *PIM Product saved* trigger to create an offer when a product is updated.  
    A new trigger input line is displayed.

    For detailed information on how to create a trigger, see [Create a trigger](../ActindoWorkFlow/Operation/03_ManageTriggers.md#create-a-trigger).

2. Configure the following settings for the *PIM Product saved* trigger:

    | Triggers ||
    |----|----|
    |**Name** | PIM product saved |
    |**Model** | Actindo\Modules\Actindo\PIM\Models\PIMProduct |
    |**Event** | After saving | 
    |**Condition fulfillment** | If all are met |   
    |**Status** | Active |
    |**Process priority** | 10 | 
    | **Unique check** | No |

### Split by criterion

![Split by criterion](../Assets/Screenshots/OfferCookbook/Completeness100Action.png "[Split by criterion]")

Select the *Split by criterion* action and configure it with the following settings:

| Configuration ||
|----|----|
| **Path** | _pim_completeness.totalCompleteness |
| **Operator** | >= |
| **Value** | 100 |

It is recommended to change the name in the *Label* field to a descriptive name, for example, **Completeness 100** in this case.

### Create offer

![Create offer](../Assets/Screenshots/OfferCookbook/CreateOfferAction.png "[Create offer]")

Select the *Create offer* action and configure it with the following settings:

| Static inputs | |
|---------------|-|
| **connection** | { "id": 2 } (static input) |
| **changeTracking** | - |
| **initialStatus** | "inactive" |
| **destinationAttributeSet** | - |
| **unique** | "1" |


## JSON

        {
            "key": "create_offer_from_pim_product",
            "version": 4,
            "name": "Create offer from PIM product",
            "published": true,
            "places": {
                "input": "Modules.Actindo.PIM.Models.PIMProduct",
                "output": "anyValue",
                "p-pimProduct-0": "ReadOnly.Modules.Actindo.PIM.Models.PIMProductContainer"
            },
            "comment": null,
            "transitions": [
                {
                    "maxTries": 1,
                    "queueType": "1",
                    "key": "t-Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct-0",
                    "action": "Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct",
                    "priority": 0,
                    "comment": null,
                    "description": "Create offer"
                },
                {
                    "maxTries": 1,
                    "queueType": "1",
                    "key": "t-splitByCriterion-0",
                    "action": "splitByCriterion",
                    "priority": 0,
                    "comment": null,
                    "config": {
                        "path": "_pim_completeness.totalCompleteness",
                        "operator": ">=",
                        "value": 100
                    },
                    "description": "Completeness 100?"
                }
            ],
            "arcs": [
                "t-Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct-0(data) -> output",
                "p-pimProduct-0 -> t-Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct-0(pimProduct)",
                "input -> t-splitByCriterion-0(in)",
                "t-splitByCriterion-0(match) -> p-pimProduct-0",
                "t-splitByCriterion-0(noMatch) -> output",
                "{\"id\":2} -> t-Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct-0(connection)",
                "\"inactive\" -> t-Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct-0(initialStatus)",
                "\"1\" -> t-Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct-0(unique)"
            ],
            "triggers": [
                {
                    "name": "PIM product saved",
                    "event": "postUpdate",
                    "active": true,
                    "unique": false,
                    "processPriority": "10",
                    "model": "Actindo\\Modules\\Actindo\\PIM\\Models\\PIMProduct",
                    "allConditionsRequired": true,
                    "conditions": []
                }
            ],
            "nodePositions": {
                "input": {
                    "x": -60,
                    "y": -80
                },
                "output": {
                    "x": 930,
                    "y": -60
                },
                "t-Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct-0": {
                    "x": 680,
                    "y": -270
                },
                "t-splitByCriterion-0": {
                    "x": 150,
                    "y": -80
                },
                "p-pimProduct-0": {
                    "x": 400,
                    "y": -150
                }
            }
        }






