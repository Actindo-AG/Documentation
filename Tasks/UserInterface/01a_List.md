[!!User Interface List of events](./03a_List.md)
[!!Manage the tasks](../Operation/02_ManageTasks.md)
[!!User Interface DataHub](../../DataHub/UserInterface/00_UserInterface.md)

# List (Tasks)

*Tasks > Tasks > Tab LIST*

![Tasks](../../Assets/Screenshots/Tasks/Tasks/ListTasks.png "[Tasks]")

**Tasks**

The list displays an overview of all tasks created in the current instance. You can filter the tasks displayed by different criteria using the *Assignees*, *Events*, and *Status* drop-down lists. You can also combine the filters to narrow down the listed tasks. Depending on the settings, the displayed columns may vary. All fields are read-only.

- *Assignees*  
    Click the drop-down list to filter the list of tasks by assignee. The following options are available:  
    - **All**  
        Select this option to display all the tasks, regardless of the assignee.
    - **Assigned directly to me**  
        Select this option to display the tasks assigned specifically to you. 
    - **Assigned to me via groups**  
        Select this option to display the tasks assigned to a user group which you are part of.
    - **Assigned to me directly and via groups**  
        Select this option to display the tasks assigned to you, regardless of whether they are assigned to you specifically or you are part of a user group to which the task is assigned.
    - **Unassigned**  
        Select this option to display the tasks that are not assigned to any user or group.

[comment]: <> (Es sollte Assigned to me directly ODER via groups sein! RS mit Modulexperten) 

- *Events*  
    Click the drop-down list to filter the list of tasks by event. All events created in the *Events* menu entry are displayed.

- *Status*  
    Click the drop-down list to filter the list of tasks by status. The following options are available:  
    - **Open tasks**  
        Select this option to display only the open, that is, pending, tasks.
    - **Open and closed tasks**  
        Select this option to display all tasks, both open (pending) and closed (done).

The following functions are available for the editing toolbar: 

- [MARK DONE]  
    Click this button to mark a task as done. This button is displayed if the checkbox of at least one open task with a ![Cross](../../Assets/Icons/Cross05.png "[Cross] ") (pending) status is selected.

- [REOPEN]  
    Click this button to reopen a task. This button is displayed if the checkbox of at least one closed task with a ![Check](../../Assets/Icons/Check02.png "[Check]") (done) status is selected.

- [ASSIGN TO ME]  
    Click this button to assign a task to yourself. This button is displayed if the checkbox of at least one task is selected.

- *Unassigned*  
    Click the drop-down list to select a user to assign him/her a task. This button is displayed if the checkbox of at least one task is selected. The list displays all users that are registered in your current instance. 

    > [Info] You can assign an unassigned task as well as reassign a task that is currently assigned to another user.

- [ASSIGN]  
    Click this button to assign the task to the user selected in the *Unassigned* drop-down list. This button is displayed if the checkbox of at least one task is selected.


The following fields are available in this view:

- *Created*  
    Date and time of creation.

- *Status*  
    Task status. The following options are available:
    - ![Cross](../../Assets/Icons/Cross05.png "[Cross]") (Cross)   
        The task is pending.  
    - ![Check](../../Assets/Icons/Check02.png "[Check]") (Check)  
        The task is done.

- *Title*  
    Task title.

- *Description*  
    Task description.

- *Plugin*  
    Module or plugin that owns the task.

- *Event*  
    Event to which the task is related.

- *Link*  
    Link to the task in the corresponding owner module or plugin.

- *Done date*  
    Date and time when the task has been done.

- *Assignee*  
    User to which the task is assigned.

- *Group*  
    User group to which the event and all related tasks are assigned.

- *ID*  
    Task identification number. The ID number is automatically assigned by the system.



## Task

*Tasks > Tasks > Tab LIST > Select a task*

![Attributes](../../Assets/Screenshots/Tasks/Tasks/TaskAttributes.png "[Attributes]")

The task details view contains all related information to the selected task. It includes the following tabs:

- [Attributes](#tasks-–-attributes)
- [Dependencies](#tasks-–-dependencies)
- [ETL processes](#tasks-–-etl-processes)

[comment]: <> (Diese Ansicht hat keinen Namen. Es sollte Task 1234 oder XYZ heißen o.ä. Gibt es schon einen FETA Ticket dazu?)

The following fields and functions are available in this view:

- *Created*  
    Date and time of creation.

- *Description*  
    Task description.

- *Link*  
    Link to the task in the corresponding owner module or plugin.

- [MARK DONE]  
    Click this button to mark the task as done. This button is only displayed if the task is open (pending).

- [REOPEN]  
    Click this button to reopen the task. This button is only displayed if the task is closed (done).


## Task &ndash; Attributes

*Tasks > Tasks > Tab LIST > Select a task > Tab Attributes*

![Task Attributes](../../Assets/Screenshots/Tasks/Tasks/TaskAttributes.png "[Task Attributes]")

For a detailed description of this view, see [Attributes tab](../../DataHub/UserInterface/06_AttributesTab.md) in the *DataHub* documentation.

## Task &ndash; Dependencies

*Tasks > Tasks > Tab LIST > Select a task > Tab Dependencies*

![Task Dependencies](../../Assets/Screenshots/Tasks/Tasks/TaskDependencies.png "[Task Dependencies]")

For a detailed description of this view, see [Dependencies tab](../../DataHub/UserInterface/07_DependenciesTab.md) in the *DataHub* documentation.


## Task &ndash; ETL processes

*Tasks > Tasks > Tab LIST > Select a task > Tab ETL processes*

![Task ETL processes](../../Assets/Screenshots/Tasks/Tasks/TaskETLProcesses.png "[Task ETL processes]")

For a detailed description of this view, see [Processes](../../DataHub/UserInterface/02b_Processes.md) in the *DataHub* documentation.