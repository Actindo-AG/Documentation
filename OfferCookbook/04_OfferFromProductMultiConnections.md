# Create an offer from product workflow in multiple channels

![Offer from product in multiple channels](../Assets/Screenshots/OfferCookbook/OfferFromProductMultiConnection.png "[Offer from product in multiple channels]")

## Overview

| **Summary** |       |
| ----------- |------ |
| **Purpose** | Create an *Omni-Channel* offer from a *PIM* product in multiple channels |
| **Affected entities** | Modules.Actindo.PIM.Models.PIMProduct <br> Actindo.Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct |
| **Included plugins** | *Process Orchestration* <br> *PIM* <br> *Omni-Channel* |
| **Included third party software** | none | 
| **Trigger** | The process is triggered when a *PIM* product is created or saved. |


## Prerequisites

- You have created a *PIM* product, see [Create a product](../PIM/Operation/01_ManageProducts.md#create-a-product).
- You have created a connection to a sales channel, see [Create a connection](../Channels/Integration/01_ManageConnections.md#create-a-connection).
- You have set up an offer from product workflow, see [Set up an offer from product workflow](./01_Introduction.md#set-up-an-offer-from-product-workflow).
- You have created a *PIM* product trigger, see [Create a PIM product trigger](./01_Introduction.md#create-a-pim-product-trigger). 



## Detailed description

Within a workflow, several actions are performed. In the following, all single actions within the workflow are described in detail, specifying their function and functional settings.

For detailed information on how to manage a workflow, see [Manage a workflow](../ActindoWorkFlow/Operation/01_ManageWorkflows.md).


### Split by criterion

![Completeness 100](../Assets/Screenshots/OfferCookbook/SplitByCriterionCompleteness100.png "[Completeness 100]")

The *Split by criterion* action is used to compare the input value with a defined criterion and output it via a different branch depending on whether the input value matches or not. For detailed information, see [Split by criterion](../ActindoWorkFlow/UserInterface/08_CoreActions.md#split-by-criterion). 

In this use case, you need to check whether the total completeness value of the *PIM* product coming from the start place via the *in* port is greater than or equal to 100. 

To do so, the *Split by criterion* action must be configured as follows:

**Settings**

The *Description*, *Key*, *Label*, *Queue type*, *Priority*, *Max tries* and *Long description* fields have no functional meaning for the action.

| Setting | Value | Comments | 
|---------|-------|----------|
| Description | Split by criterion | Core action |
| *Key* | splitByCriterion-0 | The key must be unique within a workflow. |
| *Label* | Completeness 100 | It is recommended to enter a short descriptive name in the *Label* field. |
| *Queue type* | Default | |
| *Priority* | 0 | |
| *Max tries* | 1 | |
| *Long description* | - | |


| Configuration ||
|----|----|
| *Path* | _pim_completeness.totalCompleteness |
| *Operator* | >= |
| *Value* | 100 |


Once configured, the *Completeness 100* action presents the following structure:

| Input ports     | Value | -  | Output ports | Value    |
| --------------- | --- | ---| -------------- | ----  |
| *in*  | PIMProduct (from start place) | - | *match* | PIMProduct |
| -     |          | - | *noMatch* | (to end place)   |

The *PIM* product in the start place is input via the *in* port. If the *PIM* product completeness input is greater than or equal to 100, the *PIM* product is output via the *match* port. Otherwise, the *PIM* product is output via the *noMatch* port, in this case, to the end place.


### Multiply input action

![Price set](../Assets/Screenshots/OfferCookbook/MultiplyInputAction.png "[Price set]")

[comment]: <> (Deprecated in Key??? Check!)

The *Multiply input action* is used to output the data coming in via one input port to two output ports. For detailed information, see [Multiply input action](../ActindoWorkFlow/UserInterface/08_CoreActions.md#multiply-input-action). 

In this use case, you use it to output the value (*PIM* product) coming via the *p* input port from the *match* output port of the previous action (*Completeness 100*) into two output ports, in order to create two different offers, one per sales channel.

To do so, the *Multiply input action* action must be configured as follows:

**Settings**

The *Description*, *Key*, *Label*, *Queue type*, *Priority*, *Max tries* and *Long description* fields have no functional meaning for the action.

| Setting | Value | Comments | 
|---------|-------|----------|
| Description | Multiply input action | Core action |
| *Key* | deprecated_duplicate_input-0 | The key must be unique within a workflow. |
| *Label* | Multiply input action | It is recommended to enter a short descriptive name in the *Label* field. |
| *Queue type* | Default | |
| *Priority* | 0 | |
| *Max tries* | 1 | |
| *Long description* | - | |

[comment]: <> (Sinnvoll hier auch umzubenennen? It is recommended to enter a short descriptive name in the *Label* field.)


Once configured, the *Multiply input action* presents the following structure:

| Input ports     | Value | -  | Output ports | Value    |
| --------------- | --- | ---| -------------- | ----  |
| *p*  | PIM product with 100 completeness | - | *p0* | PIM product (for channel A)|
| -     |          | - | *p1* | PIM product  (for channel B) |


The *p0* output port will be connected to a sales channel A, for instance, your own web shop. The *p1* output port will be connected to a sales channel B, such as a retailer platform. The workflow continues through two different branches, which can be configured differently.


### Split by criterion

![Price set](../Assets/Screenshots/OfferCookbook/SplitByCriterionPriceSet.png "[Price set]")

The *Split by criterion* action is used to compare the input value with a defined criterion and output it via a different branch depending on whether the input value matches or not. For detailed information, see [Split by criterion](../ActindoWorkFlow/UserInterface/08_CoreActions.md#split-by-criterion). 

In this use case, you want to check whether the price of the *PIM* product coming from the previous action via the *in* port is set, that is, is greater than 0, before creating an offer for the sales channel B. 

To do so, the *Split by criterion* action must be configured as follows:

**Settings**

The *Description*, *Key*, *Label*, *Queue type*, *Priority*, *Max tries* and *Long description* fields have no functional meaning for the action.

| Setting | Value | Comments | 
|---------|-------|----------|
| Description | Split by criterion | Core action |
| *Key* | splitByCriterion-1 | The key must be unique within a workflow. |
| *Label* | Price set | It is recommended to enter a short descriptive name in the *Label* field. |
| *Queue type* | Default | |
| *Priority* | 0 | |
| *Max tries* | 1 | |
| *Long description* | - | |

**Configuration**

| Setting | Value | Comments |
|---------|-------|----------|
| *Path* | _pim_price | |
| *Operator* | > | |
| *Value* | 0 | |


Once configured, the *Price set* action presents the following structure:

| Input ports     | Value | -  | Output ports | Value    |
| --------------- | --- | ---| -------------- | ----  |
| *in*  | PIM product  | - | *match* | PIM product |
| -     |          | - | *noMatch* | (to end place)   |

The *PIM* product in *p1* of the previous action is input via the *in* port. If the *PIM* price is set, that is, it is greater than 0, the *PIM* product is output via the *match* port. Otherwise, the *PIM* product is output via the *noMatch* port, in this case, to the end place.


### Create offer from PIM product

The *Create offer from PIM product* action creates an offer in the *Omni-Channel* module from a *PIM* product.  

In this use case, you want to create an offer for the *PIM* product for two different sales channels: your online shop and your retail store.


### Create shop offer

![Create offer](../Assets/Screenshots/OfferCookbook/CreateShopOffer.png "[Create offer]")

To do so, configure the *Create offer from PIM product* action as follows:

**Settings**

 The *Key*, *Label*, *Queue type*, *Priority*, *Max tries* and *Long description* fields have no functional meaning for the action.

| Setting | Value      | Comments |
|---------|------------|----------|
| Description | .createFromPimProduct <br> Create offer for pim product (/Actindo.Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct) | This field contains the API endpoint that is addressed in this action. |
| *Key* | splitByCriterion-0 | The key must be unique within a workflow. |
| *Label* | Completeness 100 | It is recommended to enter a short descriptive name in the *Label* field. |
| *Queue type* | Default | |
| *Priority* | 0 | |
|  *Max tries* | 1 | |
| *Long description* | - |  |


**Static inputs**

| Static input | Value | Comments |
|---------------|------|----------|
| *connection* | { "id": 2 } | You can find out the connection ID in the *ID* column of the *Connections* view under *Omni-Channel > Settings > Connections*. <br> If the *ID* column is hidden, see [Add or remove columns](../Core1Platform/UsingCore1/05_WorkWithLists.md#add-or-remove-columns) in the *Core1* documentation. |
| *changeTracking* | - |
| *initialStatus* | "inactive" | Offers can have three different initial status: **active**, **inactive**, and **offline**. <br> For detailed information, see [Create an offer from a PIM product](../Channels/Operation/01_ManageOffers.md#create-an-offer-from-a-pim-product). |
| *destinationAttributeSet* | - |
| *unique* | "1" | The static input *unique* prevents the creation of duplicate offers. This is a boolean value, where "1" equals true and no value equals false. This setting can be configured at this point or in the workflow trigger (*Unique check* setting). |

> [Info] For detailed information on how to insert a static input, see [Insert a static input](../ActindoWorkFlow/Operation/to-be-completed).

[comment]: <> (Stimmt unique as boolean? Stimmt Unique check info?)


### Create POS offer

To do so, configure the *Create offer from PIM product* action as follows:

**Settings**

 The *Key*, *Label*, *Queue type*, *Priority*, *Max tries* and *Long description* fields have no functional meaning for the action.

| Setting | Value      | Comments |
|---------|------------|----------|
| Description | .createFromPimProduct <br> Create offer for pim product (/Actindo.Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct) | This field contains the API endpoint that is addressed in this action. |
| *Key* | splitByCriterion-0 | The key must be unique within a workflow. |
| *Label* | Completeness 100 | It is recommended to enter a short descriptive name in the *Label* field. |
| *Queue type* | Default | |
| *Priority* | 0 | |
|  *Max tries* | 1 | |
| *Long description* | - |  |


**Static inputs**

| Static input | Value | Comments |
|---------------|------|----------|
| *connection* | { "id": 2 } | You can find out the connection ID in the *ID* column of the *Connections* view under *Omni-Channel > Settings > Connections*. <br> If the *ID* column is hidden, see [Add or remove columns](../Core1Platform/UsingCore1/05_WorkWithLists.md#add-or-remove-columns) in the *Core1* documentation. |
| *changeTracking* | - |
| *initialStatus* | "inactive" | Offers can have three different initial status: **active**, **inactive**, and **offline**. <br> For detailed information, see [Create an offer from a PIM product](../Channels/Operation/01_ManageOffers.md#create-an-offer-from-a-pim-product). |
| *destinationAttributeSet* | - |
| *unique* | "1" | The static input *unique* prevents the creation of duplicate offers. This is a boolean value, where "1" equals true and no value equals false. This setting can be configured at this point or in the workflow trigger (*Unique check* setting). |

> [Info] For detailed information on how to insert a static input, see [Insert a static input](../ActindoWorkFlow/Operation/to-be-completed).


## JSON

        {
            "key": "create_offer_from_complete_pim_product",
            "version": 20,
            "name": "Create Offer from complete PIM product",
            "published": true,
            "places": {
                "input": "Modules.Actindo.PIM.Models.PIMProduct",
                "output": "anyValue",
                "p-p-0": "anyValue",
                "p-p1-0": "anyValue",
                "p-pimProduct-1": "ReadOnly.Modules.Actindo.PIM.Models.PIMProductContainer",
                "p-p1-1": "anyValue"
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
                    "description": "Create Shop Offer"
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
                    "description": "Split by criterion"
                },
                {
                    "key": "t-Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct-1",
                    "action": "Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct",
                    "description": "create pos offer",
                    "priority": 0,
                    "maxTries": 1
                },
                {
                    "key": "t-splitByCriterion-1",
                    "action": "splitByCriterion",
                    "description": "Split by criterion",
                    "priority": 0,
                    "maxTries": 1,
                    "config": {
                        "value": 0,
                        "path": "_pim_price",
                        "operator": ">"
                    }
                },
                {
                    "key": "t-deprecated_duplicate_input-0",
                    "action": "deprecated_duplicate_input",
                    "description": "Multiply input action",
                    "priority": 0,
                    "maxTries": 1
                }
            ],
            "arcs": [
                "t-Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct-0(data) -> output",
                "input -> t-splitByCriterion-0(in)",
                "t-splitByCriterion-0(match) -> p-p-0",
                "t-splitByCriterion-0(noMatch) -> output",
                "\"1\" -> t-Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct-0(unique)",
                "{\"id\":2} -> t-Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct-0(connection)",
                "\"inactive\" -> t-Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct-0(initialStatus)",
                "p-pimProduct-1 -> t-Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct-0(pimProduct)",
                "p-p1-0 -> t-Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct-1(pimProduct)",
                "{\"id\":12} -> t-Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct-1(connection)",
                "\"active\" -> t-Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct-1(initialStatus)",
                "\"1\" -> t-Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct-1(unique)",
                "t-Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct-1(data) -> output",
                "p-p1-1 -> t-splitByCriterion-1(in)",
                "t-splitByCriterion-1(match) -> p-p1-0",
                "t-splitByCriterion-1(noMatch) -> output",
                "p-p-0 -> t-deprecated_duplicate_input-0(p)",
                "t-deprecated_duplicate_input-0(p0) -> p-pimProduct-1",
                "t-deprecated_duplicate_input-0(p1) -> p-p1-1"
            ],
            "triggers": [
                {
                    "name": "PIM Product Saved",
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
                    "x": -220,
                    "y": -70
                },
                "output": {
                    "x": 1080,
                    "y": -40
                },
                "t-Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct-0": {
                    "x": 700,
                    "y": -260
                },
                "t-splitByCriterion-0": {
                    "x": -60,
                    "y": -60
                },
                "p-p-0": {
                    "x": 50,
                    "y": -210
                },
                "p-p1-0": {
                    "x": 540,
                    "y": -210
                },
                "p-pimProduct-1": {
                    "x": 530,
                    "y": -270
                },
                "t-Extensions.Actindo.PimChannelsConnection.Offers.createFromPimProduct-1": {
                    "x": 700,
                    "y": -190
                },
                "t-splitByCriterion-1": {
                    "x": 440,
                    "y": -160
                },
                "p-p1-1": {
                    "x": 340,
                    "y": -200
                },
                "t-deprecated_duplicate_input-0": {
                    "x": 190,
                    "y": -240
                }
            }
        }