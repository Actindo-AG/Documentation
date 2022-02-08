[!!Einstellungen](Actindo/Einstellungen)

# Assign users to the POS groups

Users must belong to a specific POS group in order to be used as a cashier or store manager in the POS.
The following POS groups are available:
- POS Admin:  
  The POS Admin has all rights in the POS and can configure the settings in all stores, assign store managers and cashiers.
- POS Store Manager:   
  The POS Store Manager can configure the store settings in the assigned store. He/She can assign cashiers, log out cashiers, create pay desks, view the shift summary, etc. He/She has no rights to change the admin settings in the store.
- POS Cashier:   
  The POS cashier can log in and cash out on the assigned pay desk. He/She has no rights to change settings.

The users that belong to a POS group must be assigned to a pay desk or store in order to have the above rights.

> [Info]  Note that you need system administrator rights to be allowed to make the assignment.  

[comment]: <> (The following How-To Guide is not specific for POS and may be reused)

### Prerequisites

- The users have been created, see [Register a user](to_be_completed).
- You have the system admin rights to assign users to a group.

### Procedure

*Einstellungen > Benutzer und Gruppen > Tab GRUPPENVERWALTUNG*

  ![Gruppenverwaltung](/Assets/Screenshots/Einstellungen/BenutzerGruppen/Gruppenverwaltung/Gruppenverwaltung01.png "[Gruppenverwaltung]")

  | (1) | **Group checkboxes** |
  |-----|---------------------|
  |**(2)**| **Button Edit** |

1. Select the checkbox ![Checkbox Active](/Assets/Icons/Checkbox.png "[Checkbox Active]") of the group you want to assign the users to in the list of groups.   
  The editing toolbar is displayed above the list.

2. Click the button ![Icon Edit](/Assets/Icons/Edit01.png "[Icon Edit]") (Edit) in the editing toolbar.   
  The *Edit group* view of the selected group is displayed.

  ![Gruppe](/Assets/Screenshots/Einstellungen/BenutzerGruppen/Gruppenverwaltung/EditGroup01.png "[Gruppe]")

3. Click the button ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) in the bottom right corner.   
    The window *Add User* is displayed.

    ![Add User](/Assets/Screenshots/Einstellungen/BenutzerGruppen/Gruppenverwaltung/AddUser01.png "[Add User]")

  | (1) | **Button Add** |
  |-----|---------------------|
  |**(2)**| **Date field *Valid From*** |
  |**(2)**| **Date field *End Date*** |
  |**(2)**| **Button [SAVE]** |

4. Click the button ![Add](/Assets/Icons/Plus05.png "[Add]") (Add) below the section *Add Users* .   
  The drop-down list *Select User* is displayed.

5. Click the drop-down list *Select User* and select the user you want to assign to the group from the displayed list of users.

  > [Info]  All registered users that are not yet assigned to the group are displayed in the drop-down list.  

6. Repeat step **4** and **5** for all users you want to assign to the selected group.

7. If desired, you can activate the selected users in the group only for a certain period of time. To do so, select the start and end dates of the period in the date fields *Valid From* and *End Date*.

8. Click the button [SAVE] in the upper right corner of the window.   
  The window *Add User* is closed. The selected users are displayed in the list of users.

9. Click the button [SAVE] in the upper right corner of the group edit view.   
  The *Edit group* view is closed. The message *Gruppe gespeichert* is displayed. The new user assignments to the group are saved.

    ![Gruppe gespeichert](/Assets/Screenshots/Einstellungen/BenutzerGruppen/Gruppenverwaltung/GruppeGespeichert.png "[Gruppe gespeichert]")


## Next Steps

- [Configure the global settings for POS](05_ConfigureGlobalSettings.md)
- [Create a store in POS](06_CreateStore.md)
- [Manage offers for POS](07_ManageOffers.md)
- [Manage the POS warehouse](08_ManageWarehouse.md)  

## See also

- [User Interface Einstellungen](/Einstellungen/UserInterface/00_UserInterface.md)
- [Register a user](to_be_completed)
- [Configure the warehouse for POS](01_ConfigureWarehouse.md)
- [Manage the accounts for POS](02_ManageAccounts.md)
- [Configure the printer for POS](03_ConfigurePrinter.md)
