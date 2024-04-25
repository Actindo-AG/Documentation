# Create offer from product for multiple connections

![Advanced offer](../Assets/Screenshots/OfferCookbook/AdvancedOffer.png "[Advanced offer]")

## Description

| **Summary** |       |
| ----------- |------ |


#### Prerequisites



#### Procedure


1. [NEW ACTION]: Split by criterion  
    - Completeness 
    - Additional feature: Price is set 

2. [NEW ACTION]: Multiply input action

3. [NEW ACTION]: Create offer  




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