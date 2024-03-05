# Compare the workflows

The comparison function of the workflow enables to compare different workflow versions. By doing this, you can compare the JSON code lines of two different workflow versions, whereby all differences between the code lines are highlighted.  
You can use this function to compare a specific workflow version both with any other version of the selected workflow available on the current instance or with any workflow version available on another instance. As you can edit the JSON code directly in the compare view, you can use this function to compare a workflow to a version available on another instance or to do insertions and deletions.   
You can use this function for displaying change logs as well as to be able to do software-audits.

## Open the comparison window

Open the comparison window to compare different workflow versions. There are two different ways to open the comparison window.

#### Prerequisites

You have the required rights to edit a workflow.

#### Procedure

*Process Orchestration > Workflows > Tab OVERVIEW*

![Workflows](../../Assets/Screenshots/ActindoWorkFlow/Workflows/Workflows.png "[Workflows]")

Select the workflow for which you want to do a comparison.   
The *Workflow versions* view is displayed.
    
![Workflow versions](../../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowVersions.png "[Workflow versions]")

**Open the comparison window via the workflow versions view**

1. Click the checkbox at the desired version you want to use for comparison.   
    The editing toolbar is displayed.
    
2. Click the [COMPARE] button.  
    The *Workflow* pop-up window is displayed. 

    ![Workflow](../../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowComparison.png "[Workflow]")  

**Open the comparison window in the workflow editor**   

1. Select the workflow version.   
    The workflow editor is displayed.

2. Click the ![Points](../../Assets/Icons/Points02.png "[Points]") (Points) button in the upper left corner next to the workflow name.  

3. Select the *Show changes* menu entry.
    The *Workflow* pop-up window is displayed. 

    ![Workflow](../../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowComparison.png "[Workflow]")
    

## Compare the workflow versions

Compare a workflow with any other version available on the current instance.

#### Prerequisites

- At least two versions of a workflow has been created, see [Create a workflow](#create-a-workflow).
- You have the required rights to edit a workflow.
- You have opened the *Workflow* pop-up window, see [Open the comparison window](#open-the-comparison-window).

#### Procedure

*Process Orchestration > Workflows > Tab OVERVIEW > Select workflow > Tick workflow version > Select COMPARE*  
*Process Orchestration > Workflows > Tab OVERVIEW > Select workflow > Select workflow version > Select points > Select Show changes*

![Workflow](../../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowComparison.png "[Workflow]")
   
1. Compare the versions.   
    The left column highlights the differences in red, the right column in green. Inserts that are not available in the other version are highlighted as a gray shaded area. The scrollbar on the right highlights all differences in red or green, so you can quickly scroll to a position with differences.
    
2. If desired, use one of the following assistant functions:   

   - Version   
        Click the version drop-down list on top of a column and select the desired version number to use another version for comparison.

    - Swap versions   
        Click the ![Swap](../../Assets/Icons/Swap.png "[Swap]") [SWAP VERSIONS] button to swap the versions displayed. 
       
    - Format code  
        Click the ![Format code](../../Assets/Icons/Swap.png "[Format code]") [FORMAT CODE] button to smooth the comparison. The function compares the lines of code and puts them in the same order, so that order differences are no longer highlighted.

    - All properties   
       Click the ![All properties](../../Assets/Icons/Toggle.png "[All properties]") (All properties) toggle to compare all changes. This includes properties which have no functional impact such as the version number or the positioning of the nodes.

        ![All properties](../../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowComparisonAllProperties.png "[All properties]")

3. Click the [X CLOSE] button to close the comparison window.



## Compare the workflow version from a different instance

Compare a workflow version with any other version available on another instance.

#### Prerequisites

- At least one workflow has been created in each required instance, see [Create a workflow](#create-a-workflow).
- You have the required rights to edit a workflow.
- You have opened the *Workflow* pop-up window, see [Open the comparison window](#open-the-comparison-window).
- You are logged in to the instance, from which you want to compare a workflow version.

#### Procedure

*Process Orchestration > Workflows > Tab OVERVIEW > Select workflow > Tick workflow version > Select COMPARE in both systems*  
*Process Orchestration > Workflows > Tab OVERVIEW > Select workflow > Select workflow version > Select points > Select Show changes in both systems*

![Workflow](../../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowComparison.png "[Workflow]")

1. Copy the JSON code from the workflow version you want to use as source for the comparison.

2. Change to the instance on which you want to perform the comparison. 

2. Delete the JSON code in the desired target version.   
    The column contains no longer any code.
    ![Workflow](../../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowComparisonAnotherInstance.png "[Workflow]")

3. Paste the copied source JSON code to the target version.   
    The comparison is displayed again.
    
    ![Workflow](../../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowComparison.png "[Workflow]")
    
4. Compare the versions. If desired, use the assistant functions, see [Compare the workflow versions](#compare-the-workflow-versions). 

5. If desired, copy missing code from the source to the target version or delete unnecessary code in the target. 

5. Click the [X CLOSE] button to close the comparison window.



## Change the workflow to be compared 

Change the workflow to be compared without leaving the comparison pop-up window.

#### Prerequisites

- You have the required rights to edit a workflow.
- You have opened the *Workflow* pop-up window, see [Open the comparison window](#open-the-comparison-window).

#### Procedure

*Process Orchestration > Workflows > Tab OVERVIEW > Select workflow > Tick workflow version > Select COMPARE*  
*Process Orchestration > Workflows > Tab OVERVIEW > Select workflow > Select workflow version > Select points > Select Show changes*

![Workflow](../../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowComparison.png "[Workflow]")

1. Click the drop-down list next to the window title.  
    A list of all workflows available in the current instance is displayed.

2. Select the appropriate workflow.  
   The current workflow code has been removed. The columns are empty.

   ![Changed Workflow](../../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowComparisonEmptyColumns.png)

3. Select the desired workflow version by clicking on the *Version* drop-down list of the left column.  
    A list of all available workflow versions available for the selected workflow is displayed.

4. Select the desired version.
   The column is filled with JSON code.

5. Repeat step 3 and 4 for the right column.

6. Compare the workflow versions. If desired, use the assistant functions, see [Compare the workflow versions](#compare-the-workflow-versions). 

7. Click the [X CLOSE] button to close the comparison window.








