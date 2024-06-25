# Update a deployed version
<!---NEU Neues Kapitel-->
The *Update deployed version* function makes it easier for you to design and test your workflow. Updating a deployed version does not create a new version, but overwrites the current version. This means that changes to the workflow are not recorded. This function is useful, for example, if one of the included transitions fails due to a faulty configuration, and you do not want to set up the entire workflow again.   

It is strongly recommended that you do not use this function in a production system.

#### Prerequisites

- You are in the testing stage. 
- At least one workflow has been created, see [Create a workflow](./01_ManageWorkflows.md#create-a-workflow).
- You have the required rights to edit a workflow.
- A workflow version has been selected, see [Select a workflow version](./01_ManageWorkflows.md#select-a-workflow-version).
- In the current version, you have not added any additional transitions, nor you have made any other changes to the structure.

#### Procedure

*Process Orchestration > Workflows > Tab OVERVIEW > Select workflow > Select version*

![Workflow editor](../../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowEditor.png "[Workflow editor]")

1. Make minor changes to the workflow, for example, change the configuration or the attributes of a transition. Changes on the following settings are allowed:
    - Name
    - Long description
    - Moving nodes to a different position
    - Transition setting changes:
        - Queue type
        - Priority
        - Max tries <!--- hier kriege ich eine Fehlermeldung: Bug ticket https://internal-jira.actindo.com/browse/BUG-525 -->
        - Label
        - Long description
        - Task event
        - Configuration

2. If desired, check your changes by selecting the **Show changes** option. For detailed information, see [Compare the workflow versions](03_CompareWorkflows.md).


3. Click the ![Points](../../Assets/Icons/Points02.png "[Points]") (Points) button in the upper left corner next to the workflow name.   
    The workflow context menu is displayed.

4. Select **Update deployed version**.   
    The current deployed version is overwritten. No new version is created.  
    If you have changed something that is not allowed, the following error message is displayed. 

    ![Update not allowed](../../Assets/Screenshots/ActindoWorkFlow/Workflows/UpdateNotAllowed.png "[Update not allowed]")

    In case an error message is displayed, proceed as follows:
    1. Click the [OK] button to close the error message.
    2. Undo the last change by clicking the ![Undo](../../Assets/Icons/Undo02.png "[Undo]") (Undo) button or deploy the workflow as usual by creating a new version, see [Deploy a workflow version](01_ManageWorkflows.md#deploy-a-workflow-version).



    



