# Insert static input

Some transitions are based on an API. With the static input function, you can use an input port to pass customer-specific API data to the workflow endpoint.     
For example, you want to send offer data to a specific sales channel. Since it is not possible to add a sales channel to a start point and to pass it through the entire workflow, you can add this information to a transition which then routes the sales channel information to the workflow endpoint.
All input ports that are not yet connected to a place are displayed in this section. Enter the appropriate value in the text field below the input name. The value entered must be a valid JSON value. 
 
> [Info] Not all input ports can be configured as static inputs. At least one input port must be linked to a place.  

The following procedure shows an example of how to edit the static inputs by adding a sales channel information which requires complex JSON code. 

#### Prerequisites

The transition you want to add has additional input ports. 

#### Procedure

*Workflows > Workflows > Tab OVERVIEW > Select workflow > Select version*

![Workflow editor](../../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowEditor.png "[Workflow editor]")

1. Add the desired transition. For detailed information, see [Add a transition](./01_ManageWorkflows.md#add-a-transition).   
    The transition is added. It has several input ports which are listed in the *Static inputs* section of the transition settings sidebar. 

    ![Input ports](../../Assets/Screenshots/ActindoWorkFlow/Workflows/TransitionInputPorts.png)

2. Check the API used in the API documentation. To do this, select *Dev Tools > API > Select tab API* and select the API.    
    The API documentation is displayed. On the left side, the API list is displayed. The middle column contains the input parameters. The left side shows the JSON code of the API parameters. 
      
    ![PI documentation](../../Assets/Screenshots/ActindoWorkFlow/Workflows/WorkflowAPIDocumentation.png "[API documentation]")

    
3. Check the input parameters of the API.    
    All required input parameters are indicated. You must fill the required parameters to ensure a smooth data transfer. 

   ![API input parameters](../../Assets/Screenshots/ActindoWorkFlow/Workflows/TransitionStaticInputParameters.png "[API input parameters]")
   
4. Expand all input parameters which have a complex structure. To do this, click the ![Collapsed](../../Assets/Icons/Close.png "[Collapsed]") (Collapsed) button at the input parameter value.   
    The ![Collapsed](../../Assets/Icons/Close.png "[Collapsed]") (Collapsed) button has changed to an ![Expanded](../../Assets/Icons/Down.png "[Expanded]") (Expanded) button.

     ![Expanded input parameter](../../Assets/Screenshots/ActindoWorkFlow/Workflows/TransitionStaticInputComplex.png "[Expanded input parameter]").

5. In the right column, copy the entire JSON code of the desired complex input parameter you want to use, including the curly brackets.

    ![Copy input in curly brackets](../../Assets/Screenshots/ActindoWorkFlow/Workflows/TransitionStaticInputCopy.png "[Copy input in curly brackets]").

6. Change back to your workflow configuration. In the *Static inputs* section of the transition's settings side bar, click the ![Plus](../../Assets/Icons/Plus04.png "[Plus]") (Plus) button at the desired input parameter.    
    The ![Delete](../../Assets/Icons/Trash07.png "[Delete]") (Delete) button is displayed at the input parameter. 

    ![Add JSON code](../../Assets/Screenshots/ActindoWorkFlow/Workflows/TransitionStaticInputAdd.png "[Add JSON code]").
    
7. Enter the copied JSON code. By doing it, delete the quotes. Enter the required value.  
    The complex code has been added to the input parameter. A small arrow without a place is displayed in front of the input port with a static input value. 

    ![Insert JSON code](../../Assets/Screenshots/ActindoWorkFlow/Workflows/TransitionStaticInputInsert.png "[Insert JSON code]")

    > [Info] If you add a simple string, do not delete the quotes. Instead, use the following syntax, for example: **"U_ACTIO"**.

8. If desired, click the ![Delete](../../Assets/Icons/Trash07.png "[Delete]") (Delete) button to delete the JSON code. 