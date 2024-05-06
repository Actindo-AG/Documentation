# Create an offer from a product with completeness

![Offer from product with completeness](../Assets/Screenshots/OfferCookbook/OfferFromProductCompleteness.png "[Offer from product with completeness]")

## Overview

You can create an *Omni-Channel* offer automatically when all required attributes of a *PIM* product are set (total completeness is 100%).

| **Summary** |       |
| ----------- |------ |
| **Purpose** | Create an *Omni-Channel* offer from a *PIM* product with 100% completeness |
| **Affected entities** | Modules.Actindo.PIM.Models.PIMProduct <br> Actindo.Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct |
| **Included plugins** | *Process Orchestration* <br> *PIM* <br> *Omni-Channel* |
| **Included third party software** | none | 
| **Trigger** | The process is triggered by the update of a *PIM* product. |

**Included steps**

- Check if a *PIM* product completeness is 100 %
- Creation of an *Omni-Channel* offer from a PIM product 

**Necessary actions**

| Action | Short description | API endpoint |
| ------ | ----------------- | ------------ |
| split by criterion | Input value is compared to a criterion and split based on match/no match principle | Core action |
| createFromPimProduct  | Creation of an offer from a product | /Actindo.Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct |

For a detailed description of the core actions, see [Core actions](../ActindoWorkFlow/UserInterface/08_CoreActions.md) in the *Process Orchestration* documentation.


## How to set up an offer from product with completeness workflow

To set up an offer from product workflow, see [How to set up an offer from product basic workflow](./01_Introduction.md#how-to-set-up-an-offer-from-product-basic-workflow). 

For detailed description on how to create a workflow and all elements involved, see [Create a workflow](../ActindoWorkFlow/Operation/01_ManageWorkflows.md#create-a-workflow) in the *Process Orchestration* documentation.

<details><summary>Click to see complete procedure</summary>

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


</details>


## Description of the offer from product with completeness workflow

Once you have set up a basic workflow, you can edit it to add the necessary steps. 

#### Prerequisites

You have have set up an offer from product basic workflow, see [How to set up an offer from product basic workflow](./01_Introduction.md#how-to-set-up-an-offer-from-product-basic-workflow).

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

    For detailed information on how to add a transition, see [Add a transition](../ActindoWorkFlow/Operation/01_ManageWorkflows.md#add-a-transition).

5. Select the *Split by criterion* action.  
    The selected action is displayed in the workflow editor.

6. Configure the *Split by criterion* action with the following settings:  

    | Configuration ||
    |----|----|
    | **Path** | _pim_completeness.totalCompleteness |
    | **Operator** | >= |
    | **Value** | 100 |

    It is recommended to change the name in the *Label* field to a descriptive name, for example, **Completeness 100?** in this case.

7. Connect the input port to the start place. For detailed information, see [Connect the transition](../ActindoWorkFlow/Operation/01_ManageWorkflows.md#connect-the-transition).

    After setting it up, the *Split by criterion* action has the following structure: 
    
    | Input ports     | Value | -  | Output ports | Value    |
    | --------------- | --- | ---| -------------- | ----  |
    | *in*  | PIMProduct| - | *match* | PIMProduct |
    | -     |          | - | *noMatch* | (to end place)   |
    
8. Click the [NEW ACTION] button.  
    A window with a list of actions is displayed.
    
9. Select the *Create offer* action.
    The selected action is displayed in the workflow editor.

10. Connect the first input port to the *match* output port from the *Completeness 100?* action. For detailed information, see [Connect the transition](../ActindoWorkFlow/Operation/01_ManageWorkflows.md#connect-the-transition).

11. Configure the *Create offer* action static inputs as follows:

    | Static inputs | |
    |---------------|-|
    | **connection** | { "id": 2 } (static input) |
    | **changeTracking** | - |
    | **initialStatus** | "inactive" |
    | **destinationAttributeSet** | - |
    | **unique** | "1" |

12. Click on [DEPLOY] to publish the workflow.  
    The workflow is published and will be used from now on.



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






