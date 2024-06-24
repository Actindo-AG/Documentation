[!!Introduction](./01_Introduction.md)
[!!Manage a workflow](../ActindoWorkFlow/Operation/01_ManageWorkflows.md)
[!!Workflow and process elements](../ActindoWorkFlow/Overview/04_WorkflowProcessElements.md)
[!!Core actions](../ActindoWorkFlow/UserInterface/08_CoreActions.md)
[!!Manage the offers](../Channels/Operation/01_ManageOffers.md)

# Create an offer from product with completeness workflow

![Offer from product with completeness](../Assets/Screenshots/OfferCookbook/OfferFromProductCompleteness.png "[Offer from product with completeness]")


## Overview

| **Summary** |       |
| ----------- |------ |
| **Purpose** | Create an *Omni-Channel* offer from a *PIM* product with 100% completeness |
| **Affected entities** | Modules.Actindo.PIM.Models.PIMProduct <br> Actindo.Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct |
| **Included plugins** | *Process Orchestration* <br> *PIM* <br> *Omni-Channel* |
| **Included third party software** | none | 
| **Trigger** | The process is triggered when a *PIM* product is created or saved. |


**Included steps**

- Verification if a *PIM* product completeness is 100 %
- Creation of an *Omni-Channel* offer for a PIM product



## Workflow setup

- To set up an offer from product workflow, see [Set up an offer from product workflow](./01_Introduction.md#set-up-an-offer-from-product-workflow).
- To create a *PIM* product trigger, see [Create a PIM product trigger](./01_Introduction.md#create-a-pim-product-trigger).  

[comment]: <> (Alte Struktur: S. bkp files)



## Workflow description

Within a workflow, several actions are performed. In the following, all actions within the workflow are described in detail, specifying their function and functional settings.

For detailed information on how to manage a workflow, see [Manage a workflow](../ActindoWorkFlow/Operation/01_ManageWorkflows.md).

[comment]: <> (Link konkreter: create or edit?)

### Split by criterion

![Completeness 100](../Assets/Screenshots/OfferCookbook/SplitByCriterionCompleteness100.png "[Completeness 100]")

The *Split by criterion* action is used to compare the input value with a defined criterion and output it via a different branch depending on whether the input value matches or not. For detailed information, see [Split by criterion](../ActindoWorkFlow/UserInterface/08_CoreActions.md#split-by-criterion). 

In this use case, this action is used to check whether the total completeness value of the *PIM* product coming from the start place via the *in* port is greater than or equal to 100. 

The *PIM* product in the start place is input via the *in* port. If the *PIM* product total completeness input is greater than or equal to 100, the *PIM* product is output via the *match* port. Otherwise, the *PIM* product is output via the *noMatch* port, in this case, to the end place. This second branch results in no offer being created.

To do so, you must configure the *Split by criterion* action as follows:

#### Settings

| Field | Value | Comments | 
|---------|-------|----------|
| *Description* | Split by criterion | Core action <br> For detailed information, see [Core actions](../ActindoWorkFlow/UserInterface/08_CoreActions.md). |
| *Key* | splitByCriterion-0 | The key must be unique within a workflow. |
| *Label* | Completeness 100 | It is recommended to enter a short descriptive name in the *Label* field. |
| *Queue type* | Default | For detailed information on all action settings, see [Transitions](../ActindoWorkFlow/Overview/04_WorkflowProcessElements.md#transitions). |
| *Priority* | 0 | |
| *Max tries* | 1 | |
| *Long description* | - | |

**Configuration**

 Field | Value | Comments | 
|---------|-------|----------|
| *Path* | _pim_completeness.totalCompleteness |
| *Operator* | >= |
| *Value* | 100 |


Once configured, the *Completeness 100* action presents the following structure:

| Input ports     | Value | -  | Output ports | Value    |
| --------------- | --- | ---| -------------- | ----  |
| *in*  | PIM product (from start place) | - | *match* | PIM product |
| -     |          | - | *noMatch* | (to end place)   |



### Create offer from PIM product

![Create offer](../Assets/Screenshots/OfferCookbook/CreateOfferStaticInputs.png "[Create offer]")

The *Create offer from PIM product* action creates an offer in the *Omni-Channel* module from a *PIM* product.  

In this use case, you need to create an offer for the *PIM* product with 100 % completeness output via the *match* port of the previous action.  

In this use case, the *PIM* product input from the *Completeness 100* action via the *match* port is used, together with the connection ID, to create an offer for one of the sales channel configured in the *Omni-Channel* module. 

To do so, you must configure the *Create offer from PIM product* action as follows:

**Settings**

| Field | Value      | Comments |
|---------|------------|----------|
| *Description* | .createFromPimProduct <br> Create offer for pim product (/Actindo.Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct) | This field contains the API endpoint that is addressed in this action. |
| *Key* | Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct-0 | The key must be unique within a workflow. |
| *Label* | Create offer | It is recommended to enter a short descriptive name in the *Label* field. |
| *Queue type* | Default | For detailed information on all action settings, see [Transitions](../ActindoWorkFlow/Overview/04_WorkflowProcessElements.md#transitions).  |
| *Priority* | 0 | |
|  *Max tries* | 1 | |
| *Long description* | - |  |

**Static inputs**

| Field | Value | Comments |
|---------------|------|----------|
| *pimProduct* | PIM product | Connected to *match* output from previous action | 
| *connection* | { "id": 2 } | You can find out the connection ID in the *ID* column of the *Connections* view under *Omni-Channel > Settings > Connections*. <br> If the *ID* column is hidden, see [Add or remove columns](../Core1Platform/UsingCore1/05_WorkWithLists.md#add-or-remove-columns) in the *Core1* documentation. |
| *changeTracking* | - |
| *initialStatus* | "inactive" | Offers can have three different initial status: **active**, **inactive**, and **offline**. <br> For detailed information, see [Create an offer from a PIM product](../Channels/Operation/01_ManageOffers.md#create-an-offer-from-a-pim-product). |
| *destinationAttributeSet* | - |
| *unique* | "1" | The static input *unique* prevents the creation of duplicate offers. This is a boolean value, where "1" equals true and no value equals false. |

> [Info] For detailed information on how to insert a static input, see [Insert a static input](../ActindoWorkFlow/Operation/to-be-completed).

[comment]: <> (Stimmt unique as boolean?)



## JSON

    {
        "key": "create_offer_from_pim_product",
        "version": 6,
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
                "description": "Completeness 100"
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
                "processPriority": 10,
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






