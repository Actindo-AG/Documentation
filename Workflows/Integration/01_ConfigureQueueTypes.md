[!!Workflows](Workflows)

# Configure the queue types

Configure an arbitrary number of individual queue types to be able to process certain actions faster. You can configure an unlimited number of queue types with a defined number of workers and the and a defined sequence of how actions are to be processed. The total number of workers that can be assigned to the queue types is limited by the number of booked vCores.
The *Default* queue type is predefined and is assigned by default to all actions. It can manually be overrridden by individual queue types.


beliebig viele queue types konfigurieren, ein queue type kann bestimmte Anzahl an workern haben, die ihn abarbeiten,  reihenfolge, in der worker queue types abarbeiten sollen.
Default Queue mit 2 workern, die älteste aktion ausführen vordefiniert. Per default allen actions zugewiesen. Kann übersteuert werden.

queue type pro action

worker = job, der die action ausführt


## Create a queue type

Create an individual queue type, assign a certain number of workers to it and define the sequence in which the actions are to be processed.

### Prerequisites

No prerequisites to fulfill.

### Procedure

*Workflows > Queue Types > Tab OVERVIEW*

[comment]: <> (Insert image)

1. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The *Create Queue Type* view is displayed.

  ![New workflow](/Assets/Screenshots/Workflows/Workflows/NewWorkflow.png "[New workflow]")

2. Enter a name for the queue type in the *Name* field.

3. Enter the desired number of workers for the queue type in the *Number of workers* field.

  > [Info] The total number of workers of all queue types depends on the number of booked vCores.

4. Click the *Executing Prio* drop-down list and select the appropriate sequence of processing. The following options are available:
  - **Oldest executable action**: The oldest executable actions within all existing processes is processed first by the workers.
  - **Executable actions of oldest process**: The executable actions within the oldest process are processed first by the workers.


5. Click the [SAVE] button in the upper right corner.   
  The *Create Queue Type* view is closed. The new queue type is created and displayed in the list of queue types. The *QueueType has been created* pop-up window is displayed.

  > [Info] An error notice is displayed when the number of booked vCores is not sufficient to create the queue type with the selected number of workers.

### Next steps

- [Edit a queue type](#edit-a-queue-type)
- [Delete a queue type](#delete-a-queue-type)
- [Kill a worker](#kill-a-worker)

### See also



## Edit a queue type

Edit a queue type to modify its name, the number of workers assigned to it or the processing sequence.

### Prerequisites

At least one queue type is created, see [Create a queue type](#create-a-queue-type).

### Procedure

*Workflows > Queue Types > Tab OVERVIEW*

[comment]: <> (Insert image)

1. Click the queue type you want to edit in the list of queue types.   
  The *Edit queue type* view is displayed.

2. Edit the desired data of the queue type in the corresponding fields. You can change the name, the number of workers or the execution priority of the queue type.

3. Click the [SAVE] button in the upper right corner.
  The changes are saved. The *Edit queue type* view is closed.  

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

[comment]: <> (Insert image)

1. Select the checkbox of the queue type you want to delete in the list of queue types.  
The editing toolbar is displayed above the queue types list.

2. Click the ![Delete](/Assets/Icons/Trash03.png "[Delete]") (Delete) button in the toolbar.
The queue type is deleted. The *QueueType has been deleted* pop-up window is displayed.

### Next steps

- [Kill a worker](#kill-a-worker)

### See also

- [Create a queue type](#create-a-queue-type)
- [Edit a queue type](#edit-a-queue-type)



## Kill workers


> [Warning] Problems may occur when killing workers. Only kill the workers when you are qualified to restart the queue type actions.  

### Kill the workers of a single queue type


#### Prerequisites

At least one queue type is created, see [Create a queue type](#create-a-queue-type).

#### Procedure

*Workflows > Queue Types > Tab OVERVIEW*

[comment]: <> (Insert image)

1. Select the checkbox of the queue type whose workers you want to kill.   
The editing toolbar is displayed above the queue types list.

2. Click the [KILL WORKER OF THIS QUEUE TYPE] button in the toolbar.
The workers of the selected queue type are killed. The process actions of the selected queue type will not continue until you restart the queue type actions.

#### See also

- [Create a queue type](#create-a-queue-type)
- [Edit a queue type](#edit-a-queue-type)
- [Delete a queue type](#delete-a-queue-type)
- [Kill a worker](#kill-a-worker)



### Kill all workers

#### Prerequisites

At least one queue type is created, see [Create a queue type](#create-a-queue-type).

#### Procedure

*Workflows > Queue Types > Tab OVERVIEW*

[comment]: <> (Insert image)

1. Click the [KILL WORKER] button above the queue types list.

[comment]: <> (Was dann? Wie restart?)

#### See also

- [Create a queue type](#create-a-queue-type)
- [Edit a queue type](#edit-a-queue-type)
- [Delete a queue type](#delete-a-queue-type)
- [Kill a worker](#kill-a-worker)
