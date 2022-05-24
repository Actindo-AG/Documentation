[!!Workflows](ActindoWorkFlow)

# Overview
*Workflows > Queue Types > Tab OVERVIEW*

![Queue types](/Assets/Screenshots/ActindoWorkFlow/QueueTypes/Overview.png "[Queue types]")

**Queue Type List**

- [KILL WORKER]   
  Click this button to stop all workers in all processes that are currently executing a job.   
  For detailed information, see [Kill all workers](/ActindoWorkFlow/Integration/01_ConfigureQueueTypes.md#kill-all-workers).

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of queue types.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
  Select the checkbox to display the editing toolbar.

- [DELETE]   
  Click this button to delete the selected queue type. The *QueueType has been deleted* pop-up window is displayed. The *Default* queue type cannot be deleted.  
  For detailed information, see [Delete a queue type](/ActindoWorkFlow/Integration/01_ConfigureQueueTypes.md#delete-a-queue-type).

- [KILL WORKER OF THIS QUEUE TYPE]   
  Click this button to stop all workers of the selected process that are currently executing a job.    
  For detailed information, see [Kill the workers of a single queue type](/ActindoWorkFlow/Integration/01_ConfigureQueueTypes.md#kill-the-workers-of-a-single-queue-type).

The list displays all queue types. All fields are read-only. Depending on the settings, the displayed columns may vary. Click a queue type in the list to display the *Edit Queue Type* view.   
For detailed information, see [Edit a queue type](/ActindoWorkFlow/Integration/01_ConfigureQueueTypes.md#edit-a-queue-type).


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


- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)   
  Click this button to create a queue type. The *Create Queue Type* view is displayed.   
  For detailed information, see [Create a queue type](/ActindoWorkFlow/Integration/01_ConfigureQueueTypes.md#create-a-queue-type).



## Create Queue Type

*Workflows > Queue Types > Tab OVERVIEW > Button Add*

![Create queue type](/Assets/Screenshots/ActindoWorkFlow/QueueTypes/CreateQueueType.png "[Create queue types]")

- ![Back](/Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *Create Queue Type* view and return to the queue type list. All changes are rejected.

- [SAVE]   
  Click this button to save the new queue type.

- *Name*   
  Enter a name for the queue type.  

- *Number of workers*   
  Enter the number of workers for the queue type.

  > [Info] The number of workers you can assign to queue types depends on the number of booked vCores. -- Formel einfügen --

- *Execution Prio*   
  Click the drop-down list and select the execution priority for the queue type. The following options are available:
  - **Oldest executable action**: The oldest executable actions within all existing processes is executed first by the workers.
  - **Executable actions of oldest process**: The executable actions within the oldest process are executed first by the workers.



## Edit Queue Type

*Workflows > Queue Types > Tab OVERVIEW > Select queue type*

![Edit queue type](/Assets/Screenshots/ActindoWorkFlow/QueueTypes/EditQueueType.png "[Edit queue types]")


- ![Back](/Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *Edit Queue Type* view and return to the queue type list. All changes are rejected.

- [SAVE]   
  Click this button to save all changes to the queue type.

- *Name*   
  Click this field to edit the name for the queue type.  

- *Number of workers*   
  Click this field to edit the number of workers for the queue type. To edit the number of workers, no more workers must be active.   
  For detailed information, see [Edit the workers number](/ActindoWorkFlow/Integration/01_ConfigureQueueTypes.md#edit-the-workers-number).

  > [Info] The number of workers you can assign to queue types depends on the number of booked vCores. For one worker, 4 vCores are needed. Additionally, 10 % of the booked vCores, but at least 4 vCores are blocked for the daily business and cannot be used for workers. The number of vCores needed always refers to the total number of workers in all queue types. For example, for a queue type with 2 workers and a queue type of 4 workers, 28 vCores are needed:   
  *4 vCores per worker (4 * 6 = 24) plus 4 vCores blocked for the daily business (24 + 4 = 28)*

- *Execution Prio*   
  Click the drop-down list to change the execution priority for the queue type. The following options are available:
  - **Oldest executable action**: The oldest executable actions within all existing processes is executed first by the workers.
  - **Executable actions of oldest process**: The executable actions within the oldest process are executed first by the workers.
