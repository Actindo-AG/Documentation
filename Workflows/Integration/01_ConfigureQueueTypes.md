[!!Workflows](Workflows)

# Configure the queue types

Configure an arbitrary number of individual queue types to be able to execute certain actions faster. You can configure an unlimited number of queue types with a defined number of workers and the and a defined sequence of how actions are to be executed. The total number of workers that can be assigned to the queue types is limited by the number of booked vCores.
The *Default* queue type is predefined and is assigned to all actions by default. It can manually be overridden by individual queue types. A different queue type may be assigned for each action.


## Create a queue type

Create an individual queue type, assign a certain number of workers to it and define the sequence in which the actions are to be executed.

### Prerequisites

No prerequisites to fulfill.

### Procedure

*Workflows > Queue Types > Tab OVERVIEW*

![Overview](/Assets/Screenshots/Workflows/QueueTypes/Overview.png "[Overview]")

1. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The *Create Queue Type* view is displayed.

  ![Create queue type](/Assets/Screenshots/Workflows/QueueTypes/CreateQueueType.png "[Create queue type]")

2. Enter a name for the queue type in the *Name* field.

3. Enter the desired number of workers for the queue type in the *Number of workers* field.

  > [Info] A worker is a job that is executing the action within a process. One worker can only execute one job at the same time. By assigning multiple workers to a queue type, this queue type may execute several jobs at the same time. Consequently, actions with a queue type with more workers are executed faster that actions with queue types with less workers. The total number of workers of all queue types depends on the number of booked vCores.

4. Click the *Executing Prio* drop-down list and select the appropriate executing priority. The following options are available:
  - **Oldest executable action**: The oldest executable actions within all existing processes is executed first by the workers.
  - **Executable actions of oldest process**: The executable actions within the oldest process are executed first by the workers.


5. Click the [SAVE] button in the upper right corner.   
  The *Create Queue Type* view is closed. The new queue type is created and displayed in the list of queue types. The *QueueType has been created* pop-up window is displayed.

  ![Queue type created](/Assets/Screenshots/Workflows/QueueTypes/QueueTypeCreated.png "[Queue type created]")

  > [Info] An error notice is displayed when the number of booked vCores is not sufficient to create the queue type with the selected number of workers.

  ![Maximum total workers](/Assets/Screenshots/Workflows/QueueTypes/MaximumTotalWorkers.png "[Maximum total workers]")

### Next steps

- [Edit a queue type](#edit-a-queue-type)
- [Delete a queue type](#delete-a-queue-type)
- [Kill a worker](#kill-a-worker)

### See also



## Edit a queue type

Edit a queue type to modify its name, the number of workers assigned to it or the executing priority.

### Prerequisites

At least one queue type is created, see [Create a queue type](#create-a-queue-type).

### Procedure

#### Edit the name or the execution priority

*Workflows > Queue Types > Tab OVERVIEW*

![Overview](/Assets/Screenshots/Workflows/QueueTypes/Overview.png "[Overview]")

1. Click the queue type you want to edit in the list of queue types.   
  The *Edit queue type* view is displayed.

  ![Edit queue type](/Assets/Screenshots/Workflows/QueueTypes/EditQueueType.png "[Edit queue type]")

2. Edit the desired data of the queue type in the corresponding fields. You can change the name and the execution priority of the queue type as described below:

  + Click the *Name* field and edit the name of the queue type.

  + Click the *Execution Prio* drop-down list and select the appropriate execution priority in the list.

3. Click the [SAVE] button in the upper right corner.
  The changes are saved. The *Edit queue type* view is closed. The *QueueType has been saved* pop-up window is displayed.  

  ![Queue type saved](/Assets/Screenshots/Workflows/QueueTypes/QueueTypeSaved.png "[Queue type saved]")


#### Edit the workers number

*Workflows > Queue Types > Tab OVERVIEW*

![Overview](/Assets/Screenshots/Workflows/QueueTypes/Overview.png "[Overview]")

1. Click the queue type you want to edit in the list of queue types.   
  The *Edit queue type* view is displayed.

  ![Edit queue type](/Assets/Screenshots/Workflows/QueueTypes/EditQueueType.png "[Edit queue type]")

2. Click the flag in the upper center.   
   The engine room panel is unfolded.

  ![Engine room](/Assets/Screenshots/Workflows/QueueTypes/EngineRoom.png "[Engine room]")

3. Click the arrow right to the *Developer mode*.   
  The developer mode settings are displayed.

4. Enable the *Disable Workflow* toggle in the *Actindo Work Flow Engine* box.

  ![Disable workflow](/Assets/Screenshots/Workflows/QueueTypes/DisableWorkflow.png "[Disable workflow]")

5. Click the flag at the bottom of the engine room.    
  The engine room panel is folded.

6. Edit the number of workers in the *Number of workers* field.

7. Click the [SAVE] button in the upper right corner.    
  The changes are saved. The *Edit queue type* view is closed. The *QueueType has been saved* pop-up window is displayed.  

  ![Queue type saved](/Assets/Screenshots/Workflows/QueueTypes/QueueTypeSaved.png "[Queue type saved]")

8. Unfold the engine room panel, disable the *Disable Workflow* toggle in the *Actindo Work Flow Engine* box and fold the engine room panel again.

  ![Enable workflow](/Assets/Screenshots/Workflows/QueueTypes/EnableWorkflow.png "[Enable workflow]")

[comment]: <> (Soll das überhaupt beschrieben werden? Wegen entwicklermodus und so...)

### Next steps

- [Delete a queue type](#delete-a-queue-type)
- [Kill a worker](#kill-a-worker)

### See also

- [Create a queue type](#create-a-queue-type)



## Delete a queue type

### Prerequisites

At least one queue type is created, see [Create a queue type](#create-a-queue-type).

### Procedure

*Workflows > Queue Types > Tab OVERVIEW*

![Overview](/Assets/Screenshots/Workflows/QueueTypes/Overview.png "[Overview]")

1. Select the checkbox of the queue type you want to delete in the list of queue types.  
The editing toolbar is displayed above the queue types list.

  ![Toolbar](/Assets/Screenshots/Workflows/QueueTypes/Toolbar.png "[Toolbar]")

2. Click the ![Delete](/Assets/Icons/Trash03.png "[Delete]") (Delete) button in the toolbar.
The queue type is deleted. The *QueueType has been deleted* pop-up window is displayed.

  ![Queue type deleted](/Assets/Screenshots/Workflows/QueueTypes/QueueTypeDeleted.png "[Queue type deleted]")

### Next steps

- [Kill a worker](#kill-a-worker)

### See also

- [Create a queue type](#create-a-queue-type)
- [Edit a queue type](#edit-a-queue-type)



## Kill workers

Sometimes it may be necessary to stop certain process actions. Therefore, you have to kill the workers to avoid that these actions are executed. You can either kill the workers of a single queue type or kill all workers regardless their queue type.

> [Warning] Problems may occur when killing workers. Only kill the workers when you are qualified to restart the stopped process actions.  


### Kill the workers of a single queue type

Kill the workers of a single queue types to stop only certain actions.

#### Prerequisites

At least one queue type is created, see [Create a queue type](#create-a-queue-type).

#### Procedure

*Workflows > Queue Types > Tab OVERVIEW*

![Overview](/Assets/Screenshots/Workflows/QueueTypes/Overview.png "[Overview]")

1. Select the checkbox of the queue type whose workers you want to kill.   
The editing toolbar is displayed above the queue types list.

  ![Toolbar](/Assets/Screenshots/Workflows/QueueTypes/Toolbar.png "[Toolbar]")

2. Click the [KILL WORKER OF THIS QUEUE TYPE] button in the toolbar.
The workers of the selected queue type are killed. The process actions of the selected queue type will not continue until you restart the workflow processes. The *Worker will shutdown* pop-up window is displayed.

  ![Worker shutdown](/Assets/Screenshots/Workflows/QueueTypes/WorkerShutdown.png "[Worker shutdown]")


#### See also

- [Create a queue type](#create-a-queue-type)
- [Edit a queue type](#edit-a-queue-type)
- [Delete a queue type](#delete-a-queue-type)
- [Kill a worker](#kill-a-worker)



### Kill all workers

Kill all workers to stop all actions.

#### Prerequisites

At least one queue type is created, see [Create a queue type](#create-a-queue-type).

#### Procedure

*Workflows > Queue Types > Tab OVERVIEW*

![Overview](/Assets/Screenshots/Workflows/QueueTypes/Overview.png "[Overview]")

Click the [KILL WORKER] button above the queue types list.    
All workers are killed. The process actions will not continue until you restart the workflow processes. The *Worker will shutdown* pop-up window is displayed.

  ![Worker shutdown](/Assets/Screenshots/Workflows/QueueTypes/WorkerShutdown.png "[Worker shutdown]")

[comment]: <> (Was dann? Wie restart?)

#### See also

- [Create a queue type](#create-a-queue-type)
- [Edit a queue type](#edit-a-queue-type)
- [Delete a queue type](#delete-a-queue-type)
- [Kill a worker](#kill-a-worker)
