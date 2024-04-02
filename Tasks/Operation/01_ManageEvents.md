[!!User interface Events](../UserInterface/03_Events.md)
[!!Process Orchestration](../../ActindoWorkFlow/Overview/01_General.md)

# Manage the events

An event is an occurrence that creates a task/causes a task to be created. For example, when inconsistencies in stock are found, the *Differences in stock* event creates a task to check the stock inconsistencies manually.

[comment]: <> (Initiate or create a task? Ist die Task, also, was zu tun ist, schon definiert? Klären: Trigger, event, task)

[comment]: <> (trigger: entity/data model that, together with the occurrence of an event, initiates a process; event: occurrence that initiates/creates? a task; task: instruction / action to be performed)

You can create events manually in the *Tasks* module. However, there are also some events that are automatically created by the system, for instance when installing a plugin or module, such as the *Actindo Workflow Process Execution Failed*.

When the *Process Orchestration* (also known as *Workflows*) module is installed, the *Actindo Workflow Process Execution Failed* event is automatically created in the *Task* module. This event creates a task as soon as an error occurs in a process action. The workflow process in the *Process Orchestration* module is then stopped until the specified task is performed manually by the responsible person. For detailed information about the workflow processes, see the [Process Orchestration](../../ActindoWorkFlow/Overview/01_General.md) documentation. 

[comment]: <> (Stimmt das so? Aus Worfklows automatisch beim Installieren, aber die anderen? Fulfillment, Omni-Channel?)

You can create an event manually, edit an existing event, and delete an event that is no longer needed.



## Create an event

You can create an event to determine the moment when a task must be performed.

#### Prerequisites

No prerequisites to fulfill.

#### Procedure

*Tasks > Events*

![List of events](../../Assets/Screenshots/Tasks/Events/ListEvents.png "[List of events]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    The *Create event* view is displayed.

    ![Create event](../../Assets/Screenshots/Tasks/Events/CreateEvent.png "[Create event]")

2. Enter a name for the event in the *Name* field.

3. Enter an identifier for the event in the *Identifier* field. The event identifier works like an attribute key. A key is required for API access and must be system wide unique. Just like a key, the identifier must fulfill the following criteria:
    - valid characters are **a-z** (upper and lower case), **0-9** and the underscore ( **_** )
    - the key must not start with a number
    - a double underscore ( **___** ) and a trailing underscore are forbidden

[comment]: <> (Stimmt das so? Wie Key in attributes?)

4. Click the *Attribute set for tasks* drop-down list and select the desired attribute set for tasks. All available attribute sets for tasks are displayed in the list.

5. As you are creating the task manually, the *Plugin* drop-down list is locked.

    > [Info] After saving the event, the value **Manually created** is displayed in the *Plugin* column.

6. Click the *Responsible user* drop-down list and select the user who should take care of the task by default. All users that are registered in the current system instance are displayed in the list. 

[comment]: <> (Müssen sie Admin sein? Rechte/Roles hier relevant?)

7. Click the *Responsible user group* drop-down list and select the user group that should take care of the task by default. All users that are registered in the current system instance are displayed in the list.

    > [Info] If necessary, you can further define in the task itself who the responsible user should be.

8. Click the [SAVE] button.  
    A confirmation message is displayed. The event has been saved. The *Create event* view is closed.  



## Edit an event

Once an event has been created, you can edit it. However, only some event properties are editable. For instance, the identifier, the attribute set, and the plugin cannot be subsequently modified.

#### Prerequisites
 
At least one event has been created, see [Create an event](#create-an-event).

#### Procedure

*Tasks > Events*

![List of events](../../Assets/Screenshots/Tasks/Events/ListEvents.png "[List of events]")

1. Click the event you want to edit in the list of events.   
    The *Edit event* view is displayed. 

    ![Edit event](../../Assets/Screenshots/Tasks/Events/EditEvent.png "[Edit event]")

    > [Info] Be aware that you can only edit the event name, the responsible user, and the responsible user group. All other fields are locked.

2. Edit the desired data of the event in the corresponding fields.

3. Click the [SAVE] button in the upper right corner.   
   A confirmation message is displayed. The changes have been saved. The *Edit event* view is closed.  



## Delete an event

You can delete an event that is no longer needed. 

> [Caution] **Loss of data**   
    Deleting will permanently remove the selected data. The deletion cannot be undone and the deleted data cannot be restored.       
    Problems may occur due to unresolved dependencies.   
    Make sure you really want to delete the selected data.

#### Prerequisites

At least one event has been created, see [Create an event](#create-an-event).

#### Procedure

*Tasks > Events*

![General settings example](../../Assets/Screenshots/Tasks/Events/ListEvents.png "[General settings example]")


1. Click the checkbox of the event you want to delete.  
    The editing toolbar is displayed.

    > [Caution] Deleting will permanently remove the selected data. The deletion cannot be undone and the deleted data cannot be restored. Problems may occur due to unresolved dependencies. 

2. Click the [DELETE] button.  
    The selected event is deleted and removed from the list of events.

