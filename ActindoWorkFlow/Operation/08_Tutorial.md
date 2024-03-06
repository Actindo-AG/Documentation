# Workflow tutorial

The following tutorial shows by using a simple example how to create a workflow.

## Use case

An order is imported from a sales channel via a driver into the *Omni-Channel* module. There an Omni-Channel order is created. The workflow is used to create a business document of type order confirmation (AB). This is then exported into the *Order Management* module for further processing. 

## Create a workflow

1. Before you can start with creating a workflow, you need to think about the data container that is to be input/output. To do this, check the data modules that are available for your desired business transaction.  
    In our example, the creation of an Omni-Channel order is the trigger that initiates the workflow execution and a business document of type AB (order confirmation) is to be output.

2. Select *DevTools > API > Tab DATA MODEL* to search for data models that meet the requirements for the input / output. In our example, the following represent these requirements:
    - Input: Actindo.Modules.Actindo.Channels.Models.Order
    - Output: Actindo.Modules.RetailSuite.RetailSuiteFaktBase.Models.BusinessDocument

3. Select *Process Orchestration > Workflows*.
    The OVERVIEW tab is displayed.
        ![Workflows](../../Assets/Screenshots/ActindoWorkFlow/Workflows/Workflows.png "[Workflows]")

4. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    The *New workflow* window is displayed.

    ![New workflow](../../Assets/Screenshots/ActindoWorkFlow/Workflows/NewWorkflow.png "[New workflow]")

5. Enter a name and a unique key for the workflow.

6. Search for **Models\Order** in the *Choose the data type of your start place* field and select the **___WorkflowAutogen___\Actindo\Modules\Actindo\Channels\Models\Order** entry. As you see, the dots from the data model are changed to backslashes in the workflow configuration.


7. Enter **Actindo.Modules.RetailSuite.RetailSuiteFaktBase.Models.BusinessDocument** in the *Choose the data type of your end place* field.





## Edit a trigger

Think about the circumstances under which the workflow is to be started. Per default the workflow is started for each workflow that has the **Actindo.Modules.Actindo.Channels.Models.Order** as start place.
The triggers allow you to define specific conditions, under which a workflow is initiated.


## Add a transition

