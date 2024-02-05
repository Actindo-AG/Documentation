# EXECUTION LOG

*Workflows > Logs > Tab EXECUTION LOG*

![Execution log](../../Assets/Screenshots/ActindoWorkFlow/Logs/ExecutionLog.png "[Execution log]")

The list displays all logs that have been created for each transition that has been processed. It displays all logs that have been created within the time period defined for the *Lifetime execution log in days* setting. For detailed information, see [Configure the logging settings](../Integration/02_ConfigureLoggingSettings.md).

- *Queue type*   
   The drop-down list contains all queue types that have been defined. For detailed information, see [Create a queue type](../Integration/01_ConfigureQueueTypes.md#create-a-queue-type).

- ![Only with profiling](../../Assets/Icons/Toggle.png "[Only with profiling]") Only with profiling   
    Enable this toggle if you only want to view logs with profiling. 

- *Start*   
   Time stamp when action processing started.

- *Waited for execution*   
   Time in seconds to wait before processing the action

- *Duration*    
   Processing time of the action in seconds.

- *Outcome*    
   The following outcomes are available:

   - **Success**   
    The action has been processed successfully.   

   - **Deferred**   
    The action has run through, but it needs to wait for something. It will start automatically again when the expected event or data is available.  

   - **Retry**    
    The action failed, but will be retried after a period of time has elapsed. 

    - **Error**   
    The action has finally failed.

- *Profile*   
    A profiling has been activated for this action. Click the link to open a detailed report on the execution of this transition.

- *Queue type*   
   Queue type of this transition.

- *Worker number*   
  Number of the worker who has processed this action.
  <!--- Julian, oder sind es Amount of workers? also anzahl der Worker die gearbeitet haben-->

- *Transition*   
   Key of the transition.

- *Process*    
<!--- Hallo Julian, Spalte ist leer, was wird hier angezeigt? -->   

- *ID*   
<!--- Hallo Julian, was ist das für eine ID?>
 