[!!Manage a catalog](../Integration/06_ManageCatalogs.md)

# Catalogs

[comment]: <> (UI buggy -> will be changed)

*PIM > Settings > Tab CATALOGS*

![Catalogs](../../Assets/Screenshots/PIM/Settings/Catalogs/Catalogs.png "[Catalogs]")

**Catalogs**

- *"Catalog name"*   
    Click the drop-down list to select a catalog. All available catalogs are displayed in the drop-down list. By default, the catalog **Product Categories** is preselected.

- ![Points](../../Assets/Icons/Points01.png "[Points]") (Points)  
    Click this button to display the context menu and either create a catalog or edit the selected catalog.


## Context menu

*PIM > Settings > Tab CATALOGS > Button Points*

![Context menu](../../Assets/Screenshots/PIM/Settings/Catalogs/ContextMenu.png "[Context menu]")

- ![Plus](../../Assets/Icons/Plus06.png "[Plus]") Create new   
    Click this menu entry to create a catalog. The *Create new catalog* view is displayed.

- ![Edit](../../Assets/Icons/Edit02.png "[Edit]") Edit   
    Click this menu entry to edit the selected catalog. The *Edit catalog* view is displayed.



## Create new catalog

*PIM > Settings > Tab CATALOGS > Button Points > Entry Create new*

![Create new catalog](../../Assets/Screenshots/PIM/Settings/Catalogs/CreateNewCatalog.png "[Create new catalog]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to cancel creating a catalog. The *Create new catalog* is closed.

- *"Catalog name"*   
    Enter a catalog name.

- [CANCEL]   
    Click this button to cancel creating a catalog. The *Create new catalog* view is closed.

- [SAVE]   
    Click this button to save the new catalog. The *Create new catalog* view is closed.

- ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add)   
    Click this button to add a category to the catalog. A plus sign is displayed in each column. Click the plus sign to add a category or sub-category. The *Add element* window is displayed.   

    > [Info] If you add a category, a second column is displayed. When you click the button ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) again, you can also create a sub-category in the second column. Each time, you add a new sub-category, the next column is displayed. You can add an unlimited number of sub-categories in an unlimited number of levels.

[comment]: <> (number of levels depends on screen size -> should it not be limited to a certain number of level? -> FETA-20)

The following buttons and fields are only displayed when you have added a category.

- ![Sort](../../Assets/Icons/Sort01.png "[Sort]") (Sort)   
    Click and hold this button to move the selected category to another position in the list using drag and drop.

- ![Edit](../../Assets/Icons/Edit03.png "[Edit]") (Edit)   
    Click this button to edit the selected category. The category data is displayed. This button is only displayed if you hover over the category.

- *First level category name*   
    Top level category. Click the category to display the second level column and all assigned sub-categories. Hover over the category to display the ![Edit](../../Assets/Icons/Edit03.png "[Edit]") (Edit) button.

- *"Second level category name"*   
    Sub-category to the selected first level category. Click the category to display the third level column and all assigned sub-categories. Hover over the category to display the ![Edit](../../Assets/Icons/Edit03.png "[Edit]") (Edit) button.

- *"x level category name"*   
    Sub-category to the selected category. Click the category to display the next lower level column and all assigned sub-categories. Hover over the category to display the ![Edit](../../Assets/Icons/Edit03.png "[Edit]") (Edit) button.



## Edit catalog

*PIM > Settings > Tab CATALOGS > Button Points > Entry Edit*

![Edit catalog](../../Assets/Screenshots/PIM/Settings/Catalogs/EditCatalog.png "[Edit catalog]")

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
    Click this button to cancel editing the selected catalog. The *Edit catalog* view is closed.

- *"Catalog name"*   
    Click this field to edit the catalog name.

- [CANCEL]   
    Click this button to cancel editing the selected catalog. The *Edit catalog* view is closed.

- [SAVE]   
    Click this button to save the changes. The *Edit catalog* view is closed.

- ![Sort](../../Assets/Icons/Sort01.png "[Sort]") (Sort)   
    Click and hold this button to move the selected category to another position in the list using drag and drop.

- ![Edit](../../Assets/Icons/Edit03.png "[Edit]") (Edit)   
    Click this button to edit the selected category. The category data is displayed. This button is only displayed if you hover over the category.

- *"First level category name"*   
    Top level category. Click the category to display the second level column and all assigned sub-categories. Hover over the category to display the ![Edit](../../Assets/Icons/Edit03.png "[Edit]") (Edit) button.

- *"Second level category name"*   
    Sub-category to the selected first level category. Click the category to display the third level column and all assigned sub-categories. Hover over the category to display the ![Edit](../../Assets/Icons/Edit03.png "[Edit]") (Edit) button.

- *"x level category name"*   
    Sub-category to the selected category. Click the category to display the next level column and all assigned sub-categories. Hover over the category to display the ![Edit](../../Assets/Icons/Edit03.png "[Edit]") (Edit) button.

- ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add)   
    Click this button to add a category to the catalog. A plus sign is displayed in each column. Click the plus sign to add a category or sub-category. The *Add element* window is displayed.   



## Add element

*PIM > Settings > Tab CATALOGS > Button Points > Entry Create new > Button Add*   
*PIM > Settings > Tab CATALOGS > Button Points > Entry Edit > Button Add*

![Add element](../../Assets/Screenshots/PIM/Settings/Catalogs/AddElement.png "[Add element]")

> [Info] The *Add element* window for categories and sub-categories is identical.

- *Name*   
    Enter a category name.

- *Key*   
    Enter a category key. The key is required for API access and must be system wide unique.

- [CANCEL]   
    Click this button to cancel adding a category. The *Add element* window is closed.

- [SAVE]   
    Click this button to add the new category. The *Add element* window is closed.

    > [Info] You have to click the [SAVE] button in the *Create new catalog* or *Edit catalog* view to save the added category.


### Edit category data

*PIM > Settings > Tab CATALOGS > Button Points > Entry Create new > Button Edit*   
*PIM > Settings > Tab CATALOGS > Button Points > Entry Edit > Button Edit*

![Group data](../../Assets/Screenshots/PIM/Settings/Catalogs/CategoryData.png "[Group data]")

- *Name*   
    Click the field to edit the category name.

- *Key*   
    Click the field to edit the category key. The key is required for API access and must be system wide unique.

- ![Delete](../../Assets/Icons/Trash01.png "[Delete]") (Delete)   
    Click this button to remove the selected category.

    > [Info] You have to click the [SAVE] button in the *Create new catalog* or *Edit catalog* view to permanently delete the group.

    > [Caution] Be aware that as soon as you delete a category, you also delete all assigned sub-categories.

- [CANCEL]   
    Click this button to cancel editing the category. The *Edit category data* window is closed.

- [SAVE]   
    Click this button to save any changes to the category. The *Edit category data* the window is closed.

    > [Info] You have to click the [SAVE] button in the *Create new catalog* or *Edit catalog* view to save the changes.
