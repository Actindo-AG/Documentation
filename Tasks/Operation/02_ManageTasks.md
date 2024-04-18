
[!!User interface Tasks](../UserInterface/01a_List.md)
[!!User interface Events](../UserInterface/03a_List.md)
[!!Process Orchestration](../../ActindoWorkFlow/Overview/01_General.md)

# Manage the tasks

A task is an activity that needs to be completed by a responsible user. Tasks are defined and configured in the *Process Orchestration* module. 

[comment]: <> (Evtl. Link auf Workflows)

Most tasks are created automatically by modules, such as *Omni-Channel* or *Process Orchestration*, for example, when a process fails. Tasks can also be added during the handling of processes in the *Process Orchestration* module, for instance, for manual clearance of suspicious orders or approving refunds. Tasks are related to an event, which can be assigned by default to a user as well as a user group. Many events are created automatically when installing a module or plugin, but you can also define your own events in the *Tasks* module. For detailed information, see [Manage the events](./01_ManageEvents.md).

The *Tasks* menu entry in the *Tasks* module displays all tasks created in your system. You can assign a task to a specific user, filter tasks by different criteria, mark a task as done, or reopen a closed task.



## Assign a task

Every task is related to an event. This means that when an event occurs, a task is created. For example, when the event "Difference in stock" occurs, a task is automatically created for the responsible user to check the inconsistencies manually and, if necessary, take further action. 

You can define the user and/or user group who, by default, are responsible for an event, and all related tasks, in the *Events* menu entry, see [Manage the events](./01_ManageEvents.md). However, you can further assign an individual or several tasks to a specific user in the *Tasks* menu entry.

You can assign tasks to yourself or to other users registered in your current instance.


### Assign a task to yourself

You can assign yourself one or more tasks at once.

#### Prerequisites

A task has been created.

#### Procedure

*Tasks > Menu entry Tasks > Tab LIST*

![List of tasks](../../Assets/Screenshots/Tasks/Tasks/ListTasks.png "[List of tasks]")

1. Click the task(s) you want to assign to yourself.  
    The editing toolbar is displayed.

2. Click the [ASSIGN TO ME] button in the editing toolbar.  
    The task(s) is/are assigned to yourself. Your username is displayed as assignee in the *Assignee* column of the selected task(s).


### Assign a task to other user

You can assign one or several tasks at once to other users registered in your current instance.

#### Prerequisites

A task has been created.

#### Procedure

*Tasks > Menu entry Tasks > Tab LIST*

![List of tasks](../../Assets/Screenshots/Tasks/Tasks/ListTasks.png "[List of tasks]")

1. Click the task(s) you want to assign to a specific user.  
    The editing toolbar is displayed.

2. Click the *Unassigned* drop-down list.  
    All users registered in the current instance are displayed in the list.

3. Select the user to whom you want to assign the task.
    
4. Click the [ASSIGN] button.  
    The username of the new responsible user is displayed as assignee in the *Assignee* column of the selected task(s).


## Check the assigned tasks

You can filter the tasks by different criteria using the drop-down menus provided in the list view. You can combine the different filters to narrow down your results. For a detailed description, see [User Interface Tasks](../UserInterface/01a_List.md).

In the following, an example procedure on how to check and filter your assigned tasks is explained.

#### Prerequisites

A task has been assigned to you, see [Assign a task](#assign-a-task). 

#### Procedure

*Tasks > Menu entry Tasks > Tab LIST*

![List of tasks](../../Assets/Screenshots/Tasks/Tasks/ListTasks.png "[List of tasks]")

1. Click the *Assignees* drop-down list and select one of the following options:
    - **Assigned to me directly**  
        The task has been assigned specifically to you via the [ASSIGN] button in the *Tasks* menu entry or you are the responsible user for the event in the *Events* menu entry.
    - **Assigned to me via groups**    
        You are a member of the responsible user group for the event in the *Events* menu entry.

2. If desired, select an event in the *Events* drop-down list to display only the tasks that are related to a specific event. All events configured in the *Events* menu entry are displayed in the list.

3. If desired, select the task status in the *Status* drop-down list. The following options are available:
    - **Open tasks**  
        Select this option to display only pending tasks, that is, tasks that are not done yet.
    - **Open and closed tasks**  
        Select this option to display all tasks.



## Mark a task as done

Once you have performed the assigned task, you can mark it as done.

#### Prerequisites

A task has been assigned to you, see [Assign a task](#assign-a-task).

#### Procedure

*Tasks > Menu entry Tasks > Tab LIST*

![List of tasks](../../Assets/Screenshots/Tasks/Tasks/ListTasks.png "[List of tasks]")

1. Click the checkbox of the task you want to mark as done.  
    The editing toolbar is displayed.

2. Click the [MARK AS DONE] button.  
    The selected task is marked as done and therefore closed. The status icon in the *Status* column changes from ![Cross](../../Assets/Icons/Cross05.png "[Cross]") to ![Check](../../Assets/Icons/Check02.png "[Check]"). The *Done date* column is updated.



## Reopen a task

You can reopen a task that has been marked as done if necessary.

#### Prerequisites

As task has been marked as done, see [Mark a task as done](#mark-a-task-as-done).

#### Procedure

*Tasks > Menu entry Tasks > Tab LIST*

![List of tasks](../../Assets/Screenshots/Tasks/Tasks/ListTasks.png "[List of tasks]")

1. Click the checkbox of the task you want to reopen.  
    The editing toolbar is displayed.

2. Click the [REOPEN] button.  
    The selected task is reopened. The status icon in the *Status* column changes from ![Check](../../Assets/Icons/Check02.png "[Check]") to ![Cross](../../Assets/Icons/Cross05.png "[Cross]"). The date in the *Done date* column is removed.