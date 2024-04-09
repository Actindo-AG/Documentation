
[!!User interface Tasks](../UserInterface/01a_List.md)
[!!User interface Events](../UserInterface/03a_List.md)
[!!Process Orchestration](../../ActindoWorkFlow/Overview/01_General.md)

# Manage the tasks

A task is an activity that needs to be completed by a responsible user. Tasks are defined and configured in the *Process Orchestration* (*Workflows*) module. 

[comment]: <> (Evtl. Link auf Workflows)

The *Tasks* menu entry in the *Tasks* module displays all tasks created in your system. You can assign a task to a specific user, filter tasks by different criteria, mark a task as done, or reopen a closed task.



## Assign a task

Every task is related to an event. This means that when an event occurs, a task is created. For example, when the event "Difference in stock" occurs, a task is automatically created for the responsible user to check the inconsistencies manually and, if necessary, take further action. 

You can define the user and/or user group who, by default, are responsible for an event, and all tasks related to it, in the *Events* menu entry, see [Manage the events](./01_ManageEvents.md). However, you can further assign an individual or several tasks to a specific user in the *Tasks* menu entry.

You can assign assign to yourself or to other users registered in the current system instance.

### Assign a task to yourself

You can assign one or several tasks at once to yourself.

#### Prerequisites

A task has been created.

#### Procedures

*Tasks > Menu entry Tasks > Tab LIST*

![List of tasks](../../Assets/Screenshots/Tasks/Tasks/ListTasks.png "[List of tasks]")

1. Click the task(s) you want to assign to yourself.  
    The editing toolbar is displayed.

2. Click the [ASSIGN TO ME] button in the editing toolbar.  
    The task(s) is/are assigned to yourself. Your username is displayed as assignee in the *Assignee* column of the selected task(s).


### Assign a task to another user

You can assign one or several tasks at once to other users registered in the current system instance.

#### Prerequisites

- A task has been created.

#### Procedures

*Tasks > Menu entry Tasks > Tab LIST*

![List of tasks](../../Assets/Screenshots/Tasks/Tasks/ListTasks.png "[List of tasks]")

1. Click the task(s) you want to assign to a specific user.  
    The editing toolbar is displayed.

2. Click the *Unassigned* drop-down list.  
    All users available in the current instance of your system are displayed in the list.

3. Select the user you want to assign the task to.
    
4. Click the [ASSIGN] button.  
    The username of the new user responsible is displayed as assignee in the *Assignee* column of the selected task(s).


## Check the assigned tasks

You can filter the tasks by different criteria using the drop-down menus provided in the list view. For detailed information, see [User Interface Tasks](../UserInterface/01a_List.md). You can combine the different filters to narrow down your results.

In the following, an example procedure on how to check and filter your assigned tasks in explained.

#### Prerequisites

A task has been assigned to you. 

#### Procedures

*Tasks > Menu entry Tasks > Tab LIST*

![List of tasks](../../Assets/Screenshots/Tasks/Tasks/ListTasks.png "[List of tasks]")

1. Click the *Assignees* drop-down list and select one of the following options:
    - **Assigned to me directly**  
        This means that the task has been assigned specifically to you via the [ASSIGN] button in the *Tasks* menu entry or in the *Events* menu entry.
    - **Assigned to me via groups**    
        This means that you are part of a group to which the task/event (?) has been assigned in the *Events* menu entry.

2. If desired, select an event in the *Events* drop-down list to display only the tasks that are linked to a specific event. All events configured in the *Events* menu entry are displayed in the list.

3. If desired, select the task status in the *Status* drop-down list. the following options are available:
    - **Open tasks**  
        Select this option to display only pending tasks, that is, tasks that are not done yet.
    - **Open and closed tasks**  
        Select this option to display all tasks.



## Mark a task as done

Once you have performed the assigned task, you can mark it as done.

#### Prerequisites

A task has been assigned to you, see [Assign a task](#assign-a-task).

#### Procedures

*Tasks > Menu entry Tasks > Tab LIST*

![List of tasks](../../Assets/Screenshots/Tasks/Tasks/ListTasks.png "[List of tasks]")

1. Click the checkbox of the task you want to mark as done.  
    The editing toolbar is displayed.

2. Click the [MARK AS DONE] button.  
    The selected task is marked as done and therefore closed. The status icon in the *Status* column changes from ![Cross](../../Assets/Icons/Cross05.png "[Cross]") to ![Check](../../Assets/Icons/Check02.png "[Check]"). The date on *Done date* column is updated.


## Reopen a task

You can reopen as task that has been marked as done if necessary.

#### Prerequisites

As task has been marked as done, see [Mark a task as done](#mark-a-task-as-done).

#### Procedures

*Tasks > Menu entry Tasks > Tab LIST*

![List of tasks](../../Assets/Screenshots/Tasks/Tasks/ListTasks.png "[List of tasks]")

1. Click the checkbox of the task you want to reopen.  
    The editing toolbar is displayed.

2. Click the [REOPEN] button.  
    The selected task is reopened. The status icon in the *Status* column changes from ![Check](../../Assets/Icons/Check02.png "[Check]") to ![Cross](../../Assets/Icons/Cross05.png "[Cross]"). The date on *Done date* column is removed.