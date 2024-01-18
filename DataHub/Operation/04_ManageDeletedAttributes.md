# Manage deleted attributes

Attributes that haves been deleted are moved to the *DELETED ATTRIBUTES* tab. They are not irretrievably deleted. You can still recover the attribute and make the deletion undone. Alternatively, you can permanently delete an attribute that is definitely no longer needed.

## Recover an attribute

Recover an attribute and undo the deletion undone for attributes that have been deleted by mistake.

#### Prerequisites

At least one attribute has been moved to the *DELETED ATTRIBUTES* tab, see [Delete an attribute](../Integration/01_ManageAttributes.md#edit-an-attribute).

#### Procedure

*DataHub > Settings > Tab DELETED ATTRIBUTES*

![Attributes](../../Assets/Screenshots/DataHub/Settings/DeletedAttributes/DeletedAttributes.png "[Attributes]")

1. Select the checkbox of the attribute you want to recover in the list of deleted attributes.   
    The editing toolbar is displayed above the deleted attributes list.

2. Click the [RECOVER] button in the editing toolbar.   
    The selected attribute has been recovered and is removed from the list of deleted attributes.



## Permanently delete an attribute

You can permanently delete an attribute if it is no longer needed.
As there are usually dependencies on an attribute, for example through an attribute set or created products, it is recommended to deactivate an attribute instead of deleting it permanently.
Permanently deleted attributes cannot be recovered.

#### Prerequisites

At least one attribute has been moved to the *DELETED ATTRIBUTES* tab, see [Delete an attribute](#delete-an-attribute).

#### Procedure

*DataHub > Settings > Tab DELETED ATTRIBUTES*

![Attributes](../../Assets/Screenshots/DataHub/Settings/DeletedAttributes/DeletedAttributes.png "[Attributes]")

1. Select the checkbox of the attribute you want to permanently delete in the list of deleted attributes.    
    The editing toolbar is displayed above the attributes list.

    > [Info] If the attribute moved to the *DELETED ATTRIBUTES* tab is not yet displayed in the list of deleted attributes, click the ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button to update the list.

2. Click the [Delete] button in the editing toolbar.  
    The attribute has been permanently deleted. The deletion cannot be undone.

    > [Caution] Be aware that problems may occur if you delete an attribute with existing dependencies.