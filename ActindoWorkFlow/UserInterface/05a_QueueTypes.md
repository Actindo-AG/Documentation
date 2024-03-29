[!!Configure the queue types](../Integration/01_ConfigureQueueTypes.md)

# Overview

*Workflows > Queue types > Tab OVERVIEW*

![Queue types](../../Assets/Screenshots/ActindoWorkFlow/QueueTypes/Overview.png "[Queue types]")

**Queue type list**

- [KILL WORKER]   
    Click this button to stop all workers that are currently executing actions in all processes.   

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
    Click this button to update the list of queue types.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
    Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]      
    Select the checkbox to display the editing toolbar.

- [DELETE]   
    Click this button to delete the selected queue type. The *Queue type has been deleted* pop-up window is displayed. The *Default* queue type cannot be deleted.  

- [KILL WORKER OF THIS QUEUE TYPE]   
    Click this button to stop all workers that are currently executing an action of the selected queue type.   

The list displays all queue types. All fields are read-only. Depending on the settings, the displayed columns may vary. Click a queue type in the list to display the *Edit queue type* view.    

- *ID*   
    Queue type identification number. The ID number is automatically assigned by the system when the queue type is created.

- *Name*   
    Queue type name.  

- *Number of workers*   
    Number of the workers assigned to the queue type.

- *Sort mode of actions*   
    Execution priority assigned to the queue type. The following options can be displayed:   
    - **Oldest executable action**
    - **Executable actions of oldest process**

- ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add)   
    Click this button to create a queue type. The *Create queue type* view is displayed, see [Create a queue type](../Integration/01_ConfigureQueueTypes.md#create-a-queue-type).



## Create queue type

*Workflows > Queue types > Tab OVERVIEW > Button Add*

![Create queue type](../../Assets/Screenshots/ActindoWorkFlow/QueueTypes/CreateQueueType.png "[Create queue types]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *Create queue type* view and return to the queue type list. All changes are rejected.

- [SAVE]   
    Click this button to save the new queue type.

- *Name*   
    Enter a name for the queue type.  

- *Number of workers*   
    Enter the number of workers for the queue type.

    > [Info] The number of workers you can assign to queue types depends on the number of booked vCores. For one worker, 4 vCores are needed. Additionally, 10 % of the booked vCores, but at least 4 vCores are blocked for the daily business and cannot be used for workers. The number of vCores needed always refers to the total number of workers in all queue types. For example, for a queue type with 2 workers and a queue type of 4 workers, 28 vCores are needed:    
    *4 vCores per worker (4 \* 6 = 24) plus 4 vCores blocked for the daily business (24 + 4 = 28)*

- *Execution priority*   
    Click the drop-down list and select the execution priority for the queue type. The following options are available:
    - **Oldest executable action**   
        The oldest executable actions within all existing processes is executed first by the workers.
    - **Executable actions of oldest process**   
        The executable actions within the oldest process are executed first by the workers.



## Edit queue type

*Workflows > Queue types > Tab OVERVIEW > Select queue type*

![Edit queue type](../../Assets/Screenshots/ActindoWorkFlow/QueueTypes/EditQueueType.png "[Edit queue types]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to close the *Edit queue type* view and return to the queue type list. All changes are rejected.

- [SAVE]   
    Click this button to save all changes to the queue type.

- *Name*   
    Click this field to edit the name for the queue type.  

- *Number of workers*   
    Click this field to edit the number of workers for the queue type. To edit the number of workers, no more workers must be active.   

    > [Info] The number of workers you can assign to queue types depends on the number of booked vCores. For one worker, 4 vCores are needed. Additionally, 10 % of the booked vCores, but at least 4 vCores are blocked for the daily business and cannot be used for workers. The number of vCores needed always refers to the total number of workers in all queue types. For example, for a queue type with 2 workers and a queue type of 4 workers, 28 vCores are needed:   
   *4 vCores per worker (4 \* 6 = 24) plus 4 vCores blocked for the daily business (24 + 4 = 28)*

- *Execution priority*   
    Click the drop-down list to change the execution priority for the queue type. The following options are available:
    - **Oldest executable action**   
        The oldest executable actions within all existing processes is executed first by the workers.
    - **Executable actions of oldest process**   
        The executable actions within the oldest process are executed first by the workers.
