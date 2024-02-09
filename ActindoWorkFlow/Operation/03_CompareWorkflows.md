# Compare the workflow versions

The comparison function of the workflow enables to compare two versions of a workflow. You can use it to compare a workflow to any other version available on the current instance. It is possible to edit the JSON code directly in the compare view, so that you can also compare to a workflow with a version available on another instance.

## Compare the workflow version with other version

Compare a workflow with any other version available on the current instance.

#### Prerequisites

- At least one workflow has been created, see [Create a workflow](#create-a-workflow).
- You have the required rights to edit a workflow.
- A workflow has been selected, see [Select a workflow](#create-a-workflow).

#### Procedure

*Workflows > Workflows > Tab OVERVIEW*

![Workflows](../../Assets/Screenshots/ActindoWorkFlow/Workflows/Workflows.png "[Workflows]")

1. Select the workflow for which you want to do a comparison.   
    The *Workflow versions* view is displayed

2. Click the checkbox at the desired version you want to compare.
    The editing toolbar is displayed.

3. Click the [COMPARE] button.  
    The *Workflow "workflow name"* pop-up window is displayed. On the left side, the JSON code of the selected version is displayed. On the right side, the latest version of the workflow is displayed.    
    If you have previously selected the latest version, the previous version is displayed.

    ![Workflow](../../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowComparison.png "[Workflow]")

    > [Info] If you are currently working in the workflow editor, and want to display changes from the previous version, you can also display this view as follows:  
        - Click the ![Points](../../Assets/Icons/Points02.png "[Points]") (Points) button in the upper left corner next to the workflow name.  
        - Click the *Show changes* menu entry.

4. Compare the versions.   
    Inserts are displayed in green, deletions are displayed in red.
    
5. You have the following options that support you:   

   - Select version   
        Click the version drop-down list on top of each column and select the desired version number.

    - Swap versions   
        Click the ![Swap](../../Assets/Icons/Swap.png "[Swap]") [SWAP VERSIONS] button to swap the versions displayed. Note that on the left side always the deletions are displayed, on the right side the inserts.
       
    - Smoothen comparison   
        Click the ![Code](../../Assets/Icons/Swap.png "[Code]") [FORMAT CODE] button to increase the comparability of the coding lines. The function compares the coding lines and puts them in the same order, so that these differences are no longer visible.

    - Display all changes   
       Click the ![All properties](../../Assets/Icons/Toggle.png "[All properties]") (All properties) toggle to compare all properties. This also includes properties such as the version number, which is logically different.




## Compare the workflow versions from different instances 

#### Prerequisites

- At least one workflow has been created, see [Create a workflow](#create-a-workflow).
- You have the required rights to edit a workflow.
- A workflow has been selected, see [Select a workflow](#create-a-workflow).

#### Procedure

