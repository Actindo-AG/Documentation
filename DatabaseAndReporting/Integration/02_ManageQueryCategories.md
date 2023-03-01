[!!User interface Query categories](../UserInterface/03b_QueryCategories.md)
[!!Manage the query categories](./02_ManageQueryCategories.md)
[!!Manage the user rights](./05_ManageUserRights.md)

# Manage the query categories

Query categories serve the logical organization of the managed queries. The managed queries are then organized in a tree structure of folders and subfolders.

[comment]: <> (with a maximum depth of X levels...Julian: Wie viele Ebenen sinnvoll? Vgl. ACD-315/PIM/Integration/03_ManageAttributeGroups.md) 

Query categories can be created, edited, and deleted as necessary, and assigned to the individual queries, see [Create a query](./01_ManageQueries.md#create-a-query). As in the case of the managed queries, access can also be restricted depending on the user role, see [Manage the user rights](./05_ManageUserRights.md).

[comment]: <> (Procedure Assign a query category? Spezifischer Unterkapitel in User rights?)

## Create a query category

Create a query category for manage queries to be assigned to a certain category.

#### Prerequisites 

No prerequisites to fulfill.

#### Procedure

*Database and reporting > Settings > Tab QUERY CATEGORIES*

![Query categories](../../Assets/Screenshots/DatabaseAndReporting/Settings/QueryCategories/QueryCategories.png "[Query categories]")

[comment]: <> (Julian: Neben Edit tree gibt es ein Back Pfeil. Ist dieses Bildschirm Ausgangssituation oder soll es noch einen geben?)

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    A plus sign is displayed in the query category column.

    ![Add query category](../../Assets/Screenshots/DatabaseAndReporting/Settings/QueryCategories/AddQueryCategory.png "[Add query category]")

2. Click the plus sign in the query category column.    
    The *Add element* window is displayed in the query category column.

    ![Add element](../../Assets/Screenshots/DatabaseAndReporting/Settings/QueryCategories/AddElement.png "[Add element]")

3. Enter a name for the query category in the *Name* field.

4. Enter a key for the query category in the *Key* field. The number of characters is limited to 190.

5. Click the [SAVE] button.   
    The query category has been created. The *Add element* window is closed. The new query category is displayed in the query category column.

    ![Query category created](../../Assets/Screenshots/DatabaseAndReporting/Settings/QueryCategories/QueryCategoryCreated.png "[Query category created]")

    > [Info] To add an additional category, repeat the steps 1 to 5. To add a sub-category, see [Create a query sub-category](#create-a-query-sub-category).

6. Click the [SAVE] button in the upper right corner.   
    The new query category has been saved. The *Edit query categories* view is closed.


## Edit a query category

After you have created a query category, you can edit it. You can edit the query category details, change the order of query categories, delete categories, and add sub-categories to it.

[comment]: <> (Julian: change the order?)

### Edit the query category details

Edit the query category name and key as necessary.

[comment]: <> (Kann man auch das Key ändern? Sinnvoll zu beschreiben?)

#### Prerequisites 

At least one query category has been created, see [Create a query category](#create-a-query-category).

#### Procedure

*Database and reporting > Settings > Tab QUERY CATEGORIES*

![Query categories](../../Assets/Screenshots/DatabaseAndReporting/Settings/QueryCategories/QueryCategoryCreated.png "[Query categories]")

1. Click the ![Edit](../../Assets/Icons/Edit03.png "[Edit]") (Edit) button to the right of the query category name.   
    The *Edit element* view is displayed. 

    ![Query categories](../../Assets/Screenshots/DatabaseAndReporting/Settings/QueryCategories/EditElement.png "[Query categories]")

[comment]: <> (Man sieht den existierenden Namen nicht. Bug.)

2. Modify the query category details as necessary.

3. Click the [SAVE] button in the *Edit element* window.  
    The changes have been saved to the query category column.
    > [Info] The changes must be saved again to the query categories tree by clicking the [SAVE] button in the upper right corner. Otherwise, the changes will be lost.

4. Click the [SAVE] button in the upper right corner.  
    The changes have been saved to the query categories tree. The modified query categories tree is then displayed in the *Queries* view.

    > [Info] It may be necessary to press the **F5** key to initialize the *Core1 Platform* for the changes to be displayed in the *Queries* view. 


### Change order of query categories

[comment]: <> (Julian: Momentan funktioniert es nicht. Ist es so gewollt? Vgl. PIM/DataHub)

The query categories are displayed in the order in which they are created. However, you can change the order of the query categories if necessary.

The procedure to change the order of query categories and sub-categories is identical. Just select a sub-category instead of a category and follow the steps described below.

#### Prerequisites 

At least two query categories have been created, see [Create a query category](#create-a-query-category). 

#### Procedure

![Query categories](../../Assets/Screenshots/DatabaseAndReporting/Settings/QueryCategories/QueryCategoriesCreated.png "[Query categories]")

1. Click and hold the ![Sort](../../Assets/Icons/Sort01.png "[Sort]") (Sort) button to the left of the query category you want to move to another position in the list.

2. Move the selected query category to the desired position in the list by using drag and drop.

3. Click the [SAVE] button in the upper right corner.  
    The new query category order has been saved. 


## Delete a query category

You can delete a query category if it no longer in use. Note that you just delete the query category but not the queries assigned to it. 

#### Prerequisites 

At least one query category has been created, see [Create a query category](#create-a-query-category).

#### Procedure

*Database and reporting > Managed queries > Tab QUERY CATEGORIES*

![Query categories](../../Assets/Screenshots/DatabaseAndReporting/Settings/QueryCategories/QueryCategoriesCreated.png "[Query categories]")


1. Click the ![Edit](../../Assets/Icons/Edit03.png "[Edit]") (Edit) button to the right of the query category name.   
    The *Edit element* view is displayed. 

    ![Query categories](../../Assets/Screenshots/DatabaseAndReporting/Settings/QueryCategories/EditElement.png "[Query categories]")

[comment]: <> (Man sieht den existierenden Namen nicht immer. Bug?)

2. Click the ![Delete](../../Assets/Icons/Trash01.png "[Delete]") (Delete) button in the upper left corner of the *Edit element* window.   
    The deleted query category is removed from the query category column.

3. Click the [SAVE] button in the upper right corner.  
    The changes have been saved to the query categories tree. The modified query categories tree is then displayed in the *Queries* view.

    > [Info] It may be necessary to press the **F5** key to initialize the *Core1 Platform* for the changes to be displayed in the *Queries* view. 


### Create a query sub-category

At least one query category has been created, see [Create a query category](#create-a-query-category).

#### Procedure

*Database and reporting > Settings > Tab QUERY CATEGORIES*

![Query categories](../../Assets/Screenshots/DatabaseAndReporting/Settings/QueryCategories/QueryCategory.png "[Query categories]")

1. Click the name of the category to which you want to create a sub-category.  
    A query sub-category column, and any existing sub-categories, are displayed in a column to the right of the query category column.

    ![Query categories](../../Assets/Screenshots/DatabaseAndReporting/Settings/QueryCategories/QueryCategoryCreated.png "[Query categories]")

2. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    Plus signs are displayed in the query category and the query sub-category column. 

    ![Query categories](../../Assets/Screenshots/DatabaseAndReporting/Settings/QueryCategories/AddQuerySubcategory.png "[Query categories]")

3. Click the plus sign in the query sub-category column.  
    The *Add element* window is displayed in the sub-category column.

4. Click the plus sign in the attribute sub-group column.    
    The *Add element* window is displayed in the attribute sub-group column.

    ![Query categories](../../Assets/Screenshots/DatabaseAndReporting/Settings/QueryCategories/AddElementSubcategory.png "[Query categories]")

5. Enter a name for the attribute sub-group in the *Name* field.

6. Enter a key for the query sub-category in the *Key* field. The number of characters is limited to 190.

7. Click the [SAVE] button.   
    The query sub-category has been created. The *Add element* window is closed. The new query sub-category is displayed in the query sub-category column.

    ![Query sub-category](../../Assets/Screenshots/DatabaseAndReporting/Settings/QueryCategories/QuerySubcategoryCreated.png "[Query sub-category]")

    > [Info] If you want to change the order of the query sub-categories in the list, see [Change the order of query categories](#change-the-order-of-attribute-groups).

8. Click the [SAVE] button in the upper right corner.   
    The new query sub-categories has been saved. The *Edit query categories* view is closed.

    
   [comment]: <> (Check with Julian -> Edit tree view? Work in progress)

