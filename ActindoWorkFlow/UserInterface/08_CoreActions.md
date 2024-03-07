[!!Workflow and process elements](../Overview/04_WorkflowProcessElements.md)

# Workflow core actions

![Core actions](../../Assets/Screenshots/ActindoWorkFlow/Workflows/CoreActions/CoreActions.png "[Core actions]")

To create a workflow, you must include one or several process actions.   
In the *Process Orchestration* module, a certain number of process actions is always preconfigured, the so-called *Core actions*. These core actions are used to build control flow structures in a workflow.   
Other process actions are available depending on the plugins installed in the current system.   

In the following, the core actions, their use and their settings are described in detail:

- [Change process priority](#change-process-priority)
- [Multiply input action](#multiply-input-action)
- [Execute PHP code](#execute-php-code)
- [Extract value](#extract-value)
- [Manipulate process priority](#manipulate-process-priority)
- [Manual action](#manual-action)
- [Split by criterion](#split-by-criterion)
- [Start subprocess](#start-subprocess)
- [Switch case action](#switch-case-action)
- [Update process name and search string](#update-process-name-and-search-string)
- [Wait for criterion](#wait-for-criterion)
- [Wait for parallel input](#wait-for-parallel-input)
- [Waiting action](#waiting-action)


## Change process priority

![Change process priority](../../Assets/Screenshots/ActindoWorkFlow/Workflows/CoreActions/ChangeProcessPriority.png "[Change process priority]")

The *Change process priority* core action is used to change the preconfigured priority of the process while the process is already running.
> [Info] The process priority can be defined in the workflow configuration by a trigger, see [Create a trigger](../Operation/02_ManageTriggers.md#create-a-trigger).

The data runs via the *loop_through* input port into the process action and is output via the *p* output port. However, the data is only output when data has also been incoming via the *priority* input port. The input value of the *priority* input port must be an integer. This integer will be used as the new priority.

[comment]: <> (ticket ICBPM-199 in arbeit: static inputs sollen im priority input port möglich sein, ändern sobald möglich)

### Configuration   

**Static inputs**

The *Change process priority* core action has two input ports:
- loop through: <!---TO BE ENHANCED-->
- priority: New value used for the process priority.



## Extract value

![Extract value action](../../Assets/Screenshots/ActindoWorkFlow/Workflows/CoreActions/ExtractValue.png "[Extract value action]")

The *Extract value* core action is used to extract a specific value and to use this as input for further processing. For example, you extract a specific value from a business document position such as the *pimProduct* field of the **Actindo.Modules.RetailSuite.RetailSuiteFaktBase.Models.BusinessDocumentPosition** data model, or you extract a certain position of a business document. 

You define the value to be extracted in the *Path to value* field in the configuration. 

### Configuration

*Path to value*   
Search for the parameter name of the objects's data model that is available in the input port of the transition, copy the required parameter name, and enter it in the *Path to value* field, for example **pimProduct.pim.variants**.



## Manipulate process priority

![Manipulate process priority](../../Assets/Screenshots/ActindoWorkFlow/Workflows/CoreActions/ManipulateProcessPriority.png "[Manipulate process priority]")

The *Manipulate process priority* core action is used to change the preconfigured priority of the process while the process is already running. In contrast to the [Change process priority](#change-process-priority) core action you define here the new priority by a user input.

> [Info] The process priority can be defined in the workflow configuration by a trigger, see [Create a trigger](../Operation/02_ManageTriggers.md#create-a-trigger).

**Configuration**

*User input priority*   
Enter the absolute priority number or add the relative number to the existing process priority, for example, +2 (increase the existing priority, that is the process gets a higher priority) or -3 (decrease the existing priority, that is the process gets a lower priority).



## Manual action

![Manual action](../../Assets/Screenshots/ActindoWorkFlow/Workflows/CoreActions/ManualAction.png "[Manual action]")

The *Manual action* core action is used to control the workflow by a manual user interaction. Depending on the user's decision made in the *Process orchestration >Processes > Process ID* view, a different workflow path may than be taken. If a workflow contains a manual action, the corresponding process is stopped until the user has done the decision.      
For example, it allows you to implement approval procedures in your workflows such as that each purchase order that exceeds a certain amount is to be checked by a user, before it is released or canceled. For this example, you can use the [Split by criterion](#split-by-criterion) action before to define the business document amounts for which a manual action is required.   


### Configuration

- *Time out*   
    Define a time period within which the user decision must be made. If this time period is exceeded, you can use the output port **timeout** to define a default/fallback action.   
     Use PHP code to define the time period. For detailed information, see the [strtotime.php function](https://www.php.net/manual/en/function.strtotime.php "https://www.php.net/manual/en/function.strtotime.php ") on the PHP foundation website.
      
- *Output ports 0-8*   
    Define up to 9 submissions to control the decision-making process. For each submission, a different workflow path may than be taken. For example, for a simple approval process you will need two output ports: **Accept** and **Reject**.

**Static inputs**    
The *Manual action* core action has two input ports:
- data_input: Entity that can be used to make a decision, for example a business document. 
- event-id: ID of the task event that can be used to make a decision.   

It is possible to include a static input via the unconnected input port. You can use the *data_input* or the *event_id* input port to define a static input in the *Static inputs* section in the settings sidebar. For detailed information, see [Insert a static input](../Operation/06_InsertStaticInput.md).






## Execute PHP code

![Execute PHP code](../../Assets/Screenshots/ActindoWorkFlow/Workflows/CoreActions/ExecutePHPCode.png "[Execute PHP code]")

The *Execute PHP code* core action is used to execute a custom PHP code defined in the configuration.
As the complete functionality of the PHP code is accessible, this core action enables complete variability in programming. Therefore, it is often used when more complex actions which require more logic need be executed within a workflow step.   
Depending on which ports are connected to the places and which ports are defined in the PHP code, the data runs via the *in0* to *in9* input ports into the process action and is output via the *out0* to *out9* output ports.   
It is also possible to include a static input via the unconnected input ports. These inputs must be defined in the *Static inputs* section in the settings sidebar, see [Transitions](../Overview/04_WorkflowProcessElements#transitions).

> [Info] It is recommended to give the action a name that describes what the PHP code does.

### Configuration   

- *PHP Code*   
    Click this field to display the code editor and enter the desired PHP code. There are no restrictions in the PHP code. Remember to include the input ports whose data should be read using **$in0** for the *in0* input port, **$in1** for the *in1* input port, etc. as well as to specify the output via the output ports using the *return [output1, output2];* return array. The first value within the array is output via the *out0* output port, the second value via the *out1* output port, etc.  

    ![PHP code editor](../../Assets/Screenshots/ActindoWorkFlow/Workflows/CoreActions/PHPCodeEditor.png "[PHP code editor]")



## Split by criterion

![Split by criterion](../../Assets/Screenshots/ActindoWorkFlow/Workflows/CoreActions/SplitByCriterion.png "[Split by criterion]")

The core action *Split by criterion* is used to compare the input value with a defined criterion and output it via a different branch depending on whether the input value matches or not.
The data runs via the *in* input port into the process action and is output either via the *match* output port if the input value matches the criterion to be compared with, or via the *noMatch* output port if the input value does not match the criterion to be compared with.   
The criterion to be compared with is defined in the configuration.

> [Info] It is recommended to give the action a name that describes with which criterion the input value is compared.

### Configuration  

- *Path*   
    Enter the path to the property of the input object to be compared with. If the input data is of a primitive type, for instance *string* or *number*, you can also leave the path blank to compare the input data directly.

    > [Info] The properties of an entity you can refer to are described in the relevant API documentation.

- *Operator*   
    Enter the applicable operator for the comparison. The following operators are available:
    - **=**  
        It is a match if the input value equals the defined value.
    - **!=**    
        It is a match if the input value does not equal the defined value.
    - **<=**   
        It is a match if the input value is less than / equal to the defined value.
    - **<**   
        It is a match if the input value is less the defined value.
    - **>=**   
        It is a match if the input value is greater than / equal to the defined value.
    - **>**   
        It is a match if the input value is greater the defined value.
    - **in**    
        It is a match if the input value is included within the defined values. For this operator, it is possible to enter an array in the *Value* field.
    - **notIn**   
        It is a match if the input value is not included within the defined values. For this operator, it is possible to enter an array in the *Value* field.
    - **regexp**   
        It is a match if the input value equals the regular expression entered in the *Value* field.    
        For detailed information about regular expressions, see https://regex101.com/.

- *Value*   
    Enter the value to be compared with the input value. The value must be valid JSON and is type strict, for example a string must be specified as a string (**\"example\"**), an integer as an integer (**123**), and so on.



## Start subprocess

![Start subprocess](../../Assets/Screenshots/ActindoWorkFlow/Workflows/CoreActions/StartSubprocess.png "[Start subprocess]")

The *Start subprocess* core action is used to start a different subprocess within the currently running process.       
The data runs via the *p* input port into the process action and is output via the *p* output port. However, the action does not wait until the subprocess has been finished, but outputs the data after having started the subprocess. The input data is also the data put in the start place of the subprocess.   
The subprocess to be started is defined in the configuration.

### Configuration

- *Process orchestration Key*   
    Enter the workflow key of the workflow that will be started as a subprocess. Always the latest published version of the specified workflow will be started.



## Switch case action

![Switch case action](../../Assets/Screenshots/ActindoWorkFlow/Workflows/CoreActions/SwitchCaseAction.png "[Switch case action]")

The *Switch case action* core action is used to compare the input value with up to 6 criteria and output this value via a different branch for each case. Additionally, this core action enables to output the input value via a separate branch if the input value does not match any of the specified cases or to output the input value without any match by a separate branch.    
The data runs via the *in* input port into the process action and can be output via each connected output port. The *origin* output port must be connected and the input value is always output via this port without any further action. Additionally, if one or several of the *case1* to *case6* output ports are connected, the input value is compared with the criterion specified in the respective case and output via the output port of the case where the criterion matches the input value. If no criterion of the cases matches the input value, the input value is output via the *default* output port, or, if the *default* output port is not connected, the action fails.    
The criteria to be compared with are defined in the configuration. Further, you can set the comparison to be stopped after a match. Otherwise all remaining cases are evaluated.

### Configuration  

- *Path*   
    Enter the path to the property of the input object to be compared with. If the input data is of a primitive type, for instance *string* or *number*, you can also leave the path blank to compare the input data directly.

    > [Info] The properties of an entity you can refer to are described in the relevant API documentation.

- ![Toggle](../../Assets/Icons/Toggle.png "[Toggle]") *Stop on match*   
    Enable this toggle to stop comparing the input value with the specified cases once the input value matches the first case. Disable the toggle to compare the input value with all specified cases, regardless of whether a case matches or not. By default, this toggle is disabled.

- *Case X*    
    Enter the value to be compared with the input value. The value must be valid JSON and is type strict, for example a string must be specified as a string (**\"example\"**), an integer as an integer (**123**), and so on. You can enter a single value or an array with multiple values. If you enter single value, it is checked if the input value equals the specified value. If you enter an array, it is checked if the input value equals one of the values in the array.   
    You can specify up to 6 different cases. The cases are checked in order, that means, first *Case 1*, then *Case 2*, etc.



## Update process name and search string

![Update process name and search string](../../Assets/Screenshots/ActindoWorkFlow/Workflows/CoreActions/UpdateProcessNameAndSearchString.png "[Update process name and search string]")

The *Update process name and search string* core action is used to change the preconfigured name of a process and its search string while the process is already running.  
The data runs via the input port into the process action. The input value must be a string representation, which is replacing the current process name and its corresponding search string. The new string representation is output via the output port.

### Configuration

This core action has no further configuration settings.



## Wait for criterion

![Wait for criterion](../../Assets/Screenshots/ActindoWorkFlow/Workflows/CoreActions/WaitForCriterion.png "[Wait for criterion]")

The *Wait for criterion* core action is used to insert a breakpoint when you must wait that the data input matches a certain criterion.   
The data runs via the *in* input port into the process action and is output via the *match* output port once the input value matches the criterion to be compared with. If the input value does not match the criterion to be compared with after a defined timeout, the data is, depending on the configuration, output via the *timeout* output port, or the actions fails.   
The criterion to be compared with as well as the wait time settings are defined in the configuration.

> [Info] It is recommended to give the action a name that describes which input value the criterion is waiting for.

### Configuration  

- *Initial wait time*   
    Enter the time in minutes to wait until the next comparison if the criterion does not initially match the input data.

    > [Info] The initial wait time defines the time after the initial comparison, not until the initial comparison. The initial comparison is executed automatically when the action is triggered for the first time.

- *Wait time interval*   
    Enter the time in minutes to wait for each additional comparison attempt if the criterion does not yet match the input data.

- *Timeout*   
    Enter the time in minutes after which no further attempts should be started. Depending on the configuration, either the input data will be output via the *timeout* output port or the action will fail.

- ![Toggle](../../Assets/Icons/Toggle.png "[Toggle]") *Fail on timeout*   
    Enable this toggle to make the action fail after the defined timeout. Disable the toggle to output the current input value via the *timeout* output port after the defined timeout. By default, this toggle is disabled.

- *Path*   
    Enter the path to the property of the input object to be compared with. Use objects or models whose values change by external influences between the tries as input type, since simple input data of a primitive type, for instance *string* or *number*, are static and will never change.

    > [Info] The properties of an entity you can refer to are described in the relevant API documentation.

- *Operator*   
    Enter the applicable operator for the comparison. The following operators are available:
    - **=**  
        It is a match if the input value equals the defined value.
    - **!=**    
        It is a match if the input value does not equal the defined value.
    - **<=**   
        It is a match if the input value is less than / equal to the defined value.
    - **<**   
        It is a match if the input value is less the defined value.
    - **>=**   
        It is a match if the input value is greater than / equal to the defined value.
    - **>**   
        It is a match if the input value is greater the defined value.
    - **in**    
        It is a match if the input value is included within the defined values. For this operator, it is possible to enter an array in the *Value* field.
    - **notIn**   
        It is a match if the input value is not included within the defined values. For this operator, it is possible to enter an array in the *Value* field.
    - **regexp**   
        It is a match if the input value equals the regular expression entered in the *Value* field.    
        For detailed information about regular expressions, see https://regex101.com/.

- *Value*   
    Enter the value to be compared with the input value. The value must be valid JSON and is type strict, for example a string must be specified as a string (**\"example\"**), an integer as an integer (**123**), and so on.



## Wait for parallel input

![Wait for parallel input](../../Assets/Screenshots/ActindoWorkFlow/Workflows/CoreActions/WaitForParallelInput.png "[Wait for parallel input]")

The *Wait for parallel input* core action is used to insert a breakpoint when you must wait for certain data in order to synchronize branches running in parallel in a workflow.  
The data runs via the *p_data* input port into the process action and is output via the *p* output port. However, the data is only output when data has also been incoming via the *p_trigger* input port.

### Configuration  
<!---TO BE ENHANCED-->
**Static inputs**
The *Wait for parallel input* core action has two input ports:
- p_data:
- p_trigger





## Waiting action

![Waiting action](../../Assets/Screenshots/ActindoWorkFlow/Workflows/CoreActions/WaitingAction.png "[Waiting action]")

The *Waiting action* core action is used to insert a breakpoint when you want to wait for a certain time before proceeding to the next action within the process. The data runs via the *p* input port into the process action and is output via the *p* output port. However, the data is only output after a defined period of time.    
This period of time is defined in the configuration.

### Configuration  

- *Wait time modifier*   
    Enter the period of time the action must wait before the value is output. The modifier must be a valid PHP date and time format, for example **"+ 1 day"** .    
    For detailed information about the valid PHP modifiers, see [Supported PHP DateTime formats](https://www.php.net/manual/en/datetime.formats.php).
