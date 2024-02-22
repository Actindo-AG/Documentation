# Compare the workflow versions

The comparison function of the workflow enables to compare two versions of a workflow. You can use it to compare a workflow to any other version of it available on the current instance. Because you can edit the JSON code directly in the compare view, you can compare a workflow to a version available on another instance, too. You can use this function for displaying change logs as well as to be able to do software-audits.

## Compare the workflow version with another version

Compare a workflow with any other version available on the current instance.

#### Prerequisites

- At least two versions of a workflow has been created, see [Create a workflow](#create-a-workflow).
- You have the required rights to edit a workflow.
- You have opened the workflow editor in each desired instance.

#### Procedure

*Process Orchestration > Workflows > Tab OVERVIEW*

![Workflows](../../Assets/Screenshots/ActindoWorkFlow/Workflows/Workflows.png "[Workflows]")

1. Select the workflow for which you want to do a comparison.   
    The *Process orchestration versions* view is displayed.
    
    ![Workflow versions](../../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowVersions.png "[Workflow versions]")

2. Click the checkbox at the desired version you want to compare.   
    The editing toolbar is displayed.
    

3. Click the [COMPARE] button.  
    The *Workflow "workflow name"* pop-up window is displayed. On the left side, in most cases, the JSON code of the oldest version is displayed. 

    ![Workflow](../../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowComparison.png "[Workflow]")
    
    > [Info] Alternatively, you can open the comparison as follows:  
        - In the workflow editor, click the ![Points](../../Assets/Icons/Points02.png "[Points]") (Points) button in the upper left corner next to the workflow name.  
        - -Select the *Show changes* menu entry.

4. Compare the versions.   
    Inserts are displayed in green, deletions are displayed in red.
    
5. If desired, use one of the following assistant functions:   

   - Version   
        Click the version drop-down list on top of a column and select the desired version number.

    - Swap versions   
        Click the ![Swap](../../Assets/Icons/Swap.png "[Swap]") [SWAP VERSIONS] button to swap the versions displayed. Note that on the left side always the deletions are displayed, on the right side the inserts.
       
    - Format code  
        Click the ![Format code](../../Assets/Icons/Swap.png "[Format code]") [FORMAT CODE] button to smooth the comparison. The function compares the lines of code and puts them in the same order, so that order differences are no longer highlighted.

    - All properties   
       Click the ![All properties](../../Assets/Icons/Toggle.png "[All properties]") (All properties) toggle to compare all changes. This includes properties which have no functional impact such as the version number or the positioning of the nodes.

        ![All properties](../../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowComparisonAllProperties.png "[All properties]")



## Compare the workflow versions from different instances 

Compare a workflow with any other version available on another instance.

#### Prerequisites

- At least one workflow has been created in each required instance, see [Create a workflow](#create-a-workflow).
- You have the required rights to edit a workflow.
- A workflow has been selected, see [Select a workflow](#create-a-workflow).

#### Procedure

*Process Orchestration > Workflows > Tab OVERVIEW > Select workflow > Select version > Select points > Select Show changes in both systems*

![Workflow](../../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowComparison.png "[Workflow]")

1. Copy the JSON code from the workflow version you want to use as source for the comparison.

2. Delete the code in the desired target version.   
    The columns contains no longer any code.
    ![Workflow](../../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowComparisonAnotherInstance.png "[Workflow]")

3. Paste the source JSON code to the target version.   
    The comparison is displayed again.
    
    ![Workflow](../../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowComparison.png "[Workflow]")
    
4. Compare the versions. If desired, copy missing code from the source to the target version or delete unnecessary code in the target.


