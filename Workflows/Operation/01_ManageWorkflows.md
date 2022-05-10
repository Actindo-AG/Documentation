[!!Workflows](Workflows)

# Manage the workflows

A workflow is a step-by-step graphical representation of a business processes from a start to an end point. It shows the individual actions and nodes (inputs and outputs), and the different interdependencies between them.

The *Workflows* module allow the customer to define  their own business processes, such as orders, shipments, returns, etc.

Workflows can be created, edited, and deleted, as necessary (bear in mind compatibility restrictions). They can also be tracked for errors to be solved (retry procedure after taking action in the appropriate module, see [Troubleshooting](#to-be-completed)).  





Workflow editor:
  - Nodes
    - Key (read-only)
    - Data container  = Data type? (If data type available/contained in node, actions list only displays compatible actions. When adding a new action with + sign, new compatible action is linked automatically.)
      - anyValue (default?)  
      - Enter value?  
      - ![Cross](/Assets/Icons/Cross02.png "[Cross]") (Cross) to display all available data container
      - ![Search](/Assets/Icons/Search.png "[Search]") (Search) to search?

      (optional/additional information)
      - Arbitrary Data radio button

  - Actions  
    - Action name
    - Key (read-only)
    - Label = action name (editable)
    - Queue type (drop-down list, configurable, see [Configure the queue types](#to-be-completed))
    - Task event (drop-down list)

    (optional/additional information)
    - Configuration, e.g. email where receipt/document must be sent (editable). Not all actions can be configured/have a configuration option. In this case, this option is not displayed.
    - Static inputs (editable)




## Create a workflow

### Prerequisites

### Procedure

Zoom in / out with mouse wheel or Ctrl +/-, move around with drag and drop (mouse link click and moving mouse in desired direction) in Workflow editor.

To link/join nodes together, drag and drop.

### Next steps

- [Edit a workflow](#edit-a-workflow)
- [Delete a workflow](#delete-a-workflow)
- [Publish/unpublish a workflow](#publish-unpublish-a-workflow)

### See also



## Edit a workflow

### Prerequisites

### Procedure

*Workflows > Workflows > Tab OVERVIEW*

1. Click the workflow to be edited.  
The different workflow versions are displayed.

2. Select the version to be edited.  
The workflow diagram is displayed in the workspace. On the right-hand side of the workspace, the workflow editor is displayed.

3.


### Next steps

- [Delete a workflow](#delete-a-workflow)
- [Publish/unpublish a workflow](#publish-unpublish-a-workflow)

### See also



## Delete a workflow

### Prerequisites

### Procedure

### Next steps

- [Delete a workflow](#delete-a-workflow)
- [Publish/unpublish a workflow](#publish-unpublish-a-workflow)

### See also



## Publish/Unpublish a workflow

Workflows overview (manager?) -> List of all existing workflows

Workflows can have different versions e.g. if you want to add/remove steps in a particular version, for testing purposes before publishing, etc. It is possible to change between versions. Versions can be published/unpublished. Per default, the last published version is used.


- Unpublish a workflow

Workflows > Workflows > Tab OVERVIEW > Select checkbox > Button [VERÖFFENTLICHUNG ZURÜCKZIEHEN]

### Prerequisites

### Procedure

### Next steps

- [Delete a workflow](#delete-a-workflow)
- [Publish/unpublish a workflow](#publish-unpublish-a-workflow)

### See also
