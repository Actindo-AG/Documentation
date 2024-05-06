# Create offer from product with completeness

![Offer from product with completeness](../Assets/Screenshots/OfferCookbook/OfferFromProductCompleteness.png "[Offer from product with completeness]")

## Use case

You want to create an *Omni-Channel* offer when all required attributes of a *PIM* product are set (total completeness is 100 %).

## Overview

| **Summary** |       |
| ----------- |------ |
| **Purpose** | Create an *Omni-Channel* offer from a *PIM* product with 100% completeness |
| **Affected entities** | Modules.Actindo.PIM.Models.PIMProduct <br> Actindo.Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct |
| **Included plugins** | Workflows <br> PIM <br> Omni-Channel |
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

- You have create a *PIM* product, see [Create a product](../PIM/Operation/01_ManageProducts.md#create-a-product).
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


## Description of the offer from product with completeness workflow

Once you have set up a basic workflow, you can edit it to add the necessary steps. 

#### Prerequisites

You have have set up the basic workflow, see [Set up the basic workflow](#set-up-the-basic-workflow).

#### Procedure

1. Select the newly created workflow to edit it.  
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

[comment]: <> (Configure the workflow; trigger/s auch gleich für alle, auf Basic und darauf verweisen!)

4. Click the [NEW ACTION] button.  
    A window with a list of actions is displayed. 

    For detailed information on how to create a transition, see [Create a transition](../ActindoWorkFlow/Operation/01_ManageWorkflows.md#add-a-transition).

4. Select the *Split by criterion* action.  
    The selected action is displayed in the workflow editor.

5. Configure the *Split by criterion* action with the following settings:  

    | Configuration ||
    |----|----|
    | **Path** | _pim_completeness.totalCompleteness |
    | **Operator** | >= |
    | **Value** | 100 |

    
6. Join the input port to... and the output port ... 

    The *Split by criterion* action contains/has the following data/structure: 
    
    | Input ports     | Value | -  | Output ports | Value    |
    | --------------- | --- | ---| -------------- | ----  |
    | *in*  | PIMProduct| - | *match* | PIMProduct |
    | -     |          | - | *noMatch* | (to end place)   |
    

7. Click the [NEW ACTION] button.  
    A window with a list of actions is displayed.
    
8. Select the *Create offer* action.
    The selected action is displayed in the workflow editor.

9. Configure the *Create offer* action with the following settings:

    | Static inputs | |
    |---------------|-|
    | **connection** | { "id": 2 } (static input) |
    | **changeTracking** | - |
    | **initialStatus** | "inactive" |
    | **destinationAttributeSet** | - |
    | **unique** | "1" |

10. Join the input port to... and the output port ... 

    The *Create offer* action contains/has the following data/structure: 
    
    | Input ports     | Value | -  | Output ports | Value    |
    | --------------- | --- | ---| -------------- | ----  |
    | *in*  | PIMProduct| - | *match* | PIMProduct |
    | -     |          | - | *noMatch* | (to end place)   |

    *pimProduct* input port: pimProduct 
    Output: data (anyValue)




## Potential variations and extensions

- Use case 1: Add multiple connections, see [Create offer from product for multiple connections](./04_OfferFromProductMultiConnections.md)
- Use case 2: ...



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






