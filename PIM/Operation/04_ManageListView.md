# Manage the list view

The tab *LIST* is the view where you can see and manage the products. To have a customized view for all purposes, you can modify various settings to adjust the list view to your requirements and save individual views to quickly access the view you need.


## Select a language

You can select the language for which the attribute values of the products are displayed. Only multi-language attributes can have different values in different languages. Otherwise, the value remain the same in all languages. Note that the selected language only refers to the display language of the attribute values but does not equal to the user interface language. To change the interface language, you have to [change the user language settings](to_be_completed).

### Prerequisites

At least two languages must be created and activated in the *PIM* module, see [Create a language](/DataHub/Integration/CreateLanguage.md) and [Configure the language settings](/PIM/Integration/04_ConfigureLanguages.md).

> [Info] By default, the languages *English (United States)* and *Deutsch (Deutschland)* are created and activated in the *PIM* module.

### Procedure
*PIM > Products > Tab LIST*

![Product list](/Assets/Screenshots/PIM/Products/List/Products.png "[Product list]")

1. Click the drop-down list *Language* in the left column.  
  All languages that are activated in the *PIM* module are displayed in the list.   

  > [Info] For detailed information about activating a language in the *PIM* module, see [Configure the language settings](/PIM/Integration/04_ConfigureLanguages.md).

2. Select the desired language in the drop-down list *Language* .   
  The multi-language values in the columns change to the values in the selected language. All single language values remain unchanged.

  > [Info] If a product has no attribute value defined in the selected language, the value in the corresponding columns remains blank.

### Next steps

- [Select a scope](#select-a-scope)
- [Select a product category](#select-a-product-category)
- [Select a variant view](#select-a-variant-view)
- [Create a view](#create-a-view)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Configure the language settings](/PIM/Integration/04_ConfigureLanguages.md)
- [Create a language](/DataHub/Integration/CreateLanguage.md)
- [Select the UI language](to_be_completed)



## Select a scope

You can select the scope for which the attribute values of the products are displayed. Only multi-scope attributes can have different values in different scopes. Otherwise, the value remain the same in all scopes.

### Prerequisites

At least two scopes must be created and activated in the *PIM* module, see [Create a scope](/DataHub/Integration/CreateScope.md) and [Configure the scope settings](/PIM/Integration/05_ConfigureScopes.md).

> [Info] By default, the scope *Actindo Basic* is created and activated in the *PIM* module.

### Procedure
*PIM > Products > Tab LIST*

![Product list](/Assets/Screenshots/PIM/Products/List/Products.png "[Product list]")

1. Click the drop-down list *Scope* in the left column.  
  All scopes that are activated in the *PIM* module are displayed in the list.   

  > [Info] For detailed information about activating a scope in the *PIM* module, see [Configure the scope settings](/PIM/Integration/05_ConfigureScopes.md).

2. Select the desired scope in the drop-down list *Scope* .   
  The multi-scope values in the columns change to the values in the selected scope. All single scope values remain unchanged.

  > [Info]  If a product has no attribute value defined in the selected language, the value in the corresponding column remains blank.

### Next steps

- [Select a product category](#select-a-product-category)
- [Select a variant view](#select-a-variant-view)
- [Create a view](#create-a-view)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Configure the scope settings](/PIM/Integration/05_ConfigureScopes.md)
- [Create a scope](/DataHub/Integration/CreateScope.md)
- [Select a language](#select-a-language)



## Select a product category

You can select a product category to limit the number of products to those products that are assigned to a certain category. You can assign a product to one or multiple categories and catalogs in the product view.

### Prerequisites

- At least one catalog is created, see [Create a catalog](/PIM/Integration/06_ManageCatalogs.md##create-a-catalog).
- At least one category is created within the catalog, see [Create a category](/PIM/Integration/06_ManageCatalogs.md##create-a-category).
- At least one product is assigned to a category, see [Assign a product to a catalog category](/PIM/Integration/06_ManageCatalogs.md##assign-a-product-to-a-catalog-category)

### Procedure
*PIM > Products > Tab LIST*

![Product list](/Assets/Screenshots/PIM/Products/List/Products.png "[Product list]")

1. Click the drop-down list *Catalog* in the left column.  
  All available catalogs are displayed in the list.   

  > [Info] For detailed information about creating a catalog or categories, see [Manage the catalogs](/PIM/Integration/06_ManageCatalogs.md).

2. Select the desired catalog in the drop-down list *Catalog* .      
  All corresponding categories and sub-categories are displayed below the selected catalog.

  ![Select catalog](/Assets/Screenshots/PIM/Products/List/SelectCatalog.png "[Select catalog]")

3. Select the desired category or sub-category in the left column.   
  Only those products that are assigned to the selected category or sub-category are displayed in the list of products on the right side.

  ![Select category](/Assets/Screenshots/PIM/Products/List/SelectCategory.png "[Select category]")

  > [Info] When you create a product, it is automatically assigned to the currently selected category.

### Next steps

- [Select a variant view](#select-a-variant-view)
- [Create a view](#create-a-view)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Manage the catalogs](/PIM/Integration/06_ManageCatalogs.md)
- [Select a language](#select-a-language)
- [Select a scope](#select-a-scope)



## Select a variant view

Switch the variant view to either display only the master products in the product list or all products including all product variants.

### Prerequisites

No prerequisites to fulfill.

### Procedure
*PIM > Products > Tab LIST*

![Product list](/Assets/Screenshots/PIM/Products/List/Products.png "[Product list]")

1. Click the drop-down list *Variants* at the top of the products list.   
  The options below are displayed:
  - **Hide child products**: No product variants are displayed in the product list.
  - **List all products**: All products and their variants are displayed in the product list.


2. Select the desired variant view in the drop-down list *Variants* .
  Depending on the selection, the product list displays all products or only the master products.

### Next steps

- [Create a view](#create-a-view)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Configure the scope settings](/PIM/Integration/05_ConfigureScopes.md)
- [Create a scope](/DataHub/Integration/CreateScope.md)
- [Select a language](#select-a-language)
- [Select a scope](#select-a-scope)
- [Select a product category](#select-a-product-category)



## Create a view

Create a view with a predefined selection of the language, the scope, the product category, the variant view and the order of columns in the product list.

### Prerequisites

No prerequisites to fulfill.

> [Info]  Depending on the view you want to create, it is necessary to fulfill the corresponding prerequisites in the chapters [Select a language](#select-a-language), [Select a scope](#select-a-scope) or [Select a product category](#select-a-product-category).

### Procedure
*PIM > Products > Tab LIST*

![Product list](/Assets/Screenshots/PIM/Products/List/Products.png "[Product list]")

1. Select the desired catalog in the drop-down list *Produktkategorie* in the left column.   
  All available categories and sub-categories are displayed below the selected catalog.

  ![Select catalog](/Assets/Screenshots/PIM/Products/List/SelectCatalog.png "[Select catalog]")

2. Select the desired category or sub-category in the left column.   
  Only products that are assigned to the selected category or sub-category are displayed in the list of products on the right side.

  ![Select category](/Assets/Screenshots/PIM/Products/List/SelectCategory.png "[Select category]")


[comment]: <> (Why does the assignment via the mass editing is not working?)


### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Configure the scope settings](/PIM/Integration/05_ConfigureScopes.md)
- [Create a scope](/DataHub/Integration/CreateScope.md)
- [Select a language](#select-a-language)
- [Select a scope](#select-a-scope)
- [Select a product category](#select-a-product-category)
- [Select a variant view](#select-a-variant-view)
