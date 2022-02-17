# Manage the product view

## Select a language

### Prerequisites

No prerequisites to fulfill.

> [Info] By default, the languages *English (United States)* and *Deutsch (Deutschland)* are created and activated in the *PIM* module.

### Procedure
*PIM > Products > Tab LIST*

![Product list](/Assets/Screenshots/PIM/Products/List/Products.png "[Product list]")

1. Click the drop-down list *Language* in the left column.  
  All languages that are activated in the *PIM* module are displayed in the list.   

  > [Info] For detailed information about activating a language in the *PIM* module, see [Configure the language settings](/PIM/Integration/ConfigureLanguages.md).

2. Select the desired language in the drop-down list *Language* .   
  The values in the rows change to the values in the selected language.

  > [Info] Note that the selected language only refers to the display language of the product attribute values but not to the user interface language. To change the interface language, you have to change the user language settings, see [Select the UI language](to_be_completed).

### Next steps

- [Select a scope](#select-a-scope)
- [Select a product category](#select-a-product-category)
- [Select a variant view](#select-a-variant-view)
- [Create a view](#create-a-view)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Configure the language settings](/PIM/Integration/ConfigureLanguages.md)
- [Create a language](/DataHub/Integration/CreateLanguage.md)



## Select a scope

### Prerequisites

No prerequisites to fulfill.

> [Info] By default, the scope *Actindo Basic* is created and activated in the *PIM* module.

### Procedure
*PIM > Products > Tab LIST*

![Product list](/Assets/Screenshots/PIM/Products/List/Products.png "[Product list]")

1. Click the drop-down list *Scope* in the left column.  
  All scopes that are activated in the *PIM* module are displayed in the list.   

  > [Info] For detailed information about activating a scope in the *PIM* module, see [Configure the scope settings](/PIM/Integration/ConfigureScopes.md).

2. Select the desired scope in the drop-down list *Scope* .   
  The values in the rows change to the values in the selected scope.

### Next steps

- [Select a product category](#select-a-product-category)
- [Select a variant view](#select-a-variant-view)
- [Create a view](#create-a-view)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Configure the scope settings](/PIM/Integration/ConfigureScopes.md)
- [Create a scope](/DataHub/Integration/CreateScope.md)
- [Select a language](#select-a-language)
- [Select a scope](#select-a-scope)



## Select a product category

### Prerequisites

- At least one catalog is created, see [Create a catalog](#create-a-catalog).
- At least one category is created within the catalog, see [Create a category](#create-a-category).
- At least one product is assigned to the category, see [Assign a product to a catalog category](#assign-a-product-to-a-catalog-category)

### Procedure
*PIM > Products > Tab LIST*

![Product list](/Assets/Screenshots/PIM/Products/List/Products.png "[Product list]")

1. Click the drop-down list *Product Categories* in the left column.  
  All available catalogs are displayed in the list.   

  > [Info] For detailed information about creating a catalog or categories, see [Manage a catalog](/PIM/Integration/ManageCatalog.md).

1. Select the desired catalog in the drop-down list *Product Categories* .      
  All corresponding categories and sub-categories are displayed below the selected catalog.

  ![Select catalog](/Assets/Screenshots/PIM/Products/List/SelectCatalog.png "[Select catalog]")

2. Select the desired category or sub-category in the left column.   
  Only products that are assigned to the selected category or sub-category are displayed in the list of products on the right side.

  ![Select category](/Assets/Screenshots/PIM/Products/List/SelectCategory.png "[Select category]")

  > [Info] When you create a product, it is automatically assigned to the currently selected category.

### Next steps

- [Select a variant view](#select-a-variant-view)
- [Create a view](#create-a-view)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Manage a catalog](/PIM/Integration/ManageCatalog.md)
- [Select a language](#select-a-language)
- [Select a scope](#select-a-scope)



## Select a variant view

### Prerequisites

No prerequisites to fulfill.

### Procedure
*PIM > Products > Tab LIST*

![Product list](/Assets/Screenshots/PIM/Products/List/Products.png "[Product list]")

1. Click the drop-down list *Variants* at the top of the products list.   
  The options below are displayed
  - **Hide child products**: No product variants are displayed in the product list.
  - **List all products**: All products and their variants are displayed in the product list.

2. Select the desired variant view in the drop-down list *Variants* .
  Depending on the selection, the product list displays all products or only the master products without variants.

### Next steps

- [Select a product category](#select-a-product-category)
- [Select a variant view](#select-a-variant-view)
- [Create a view](#create-a-view)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Configure the scope settings](/PIM/Integration/ConfigureScopes.md)
- [Create a scope](/DataHub/Integration/CreateScope.md)
- [Select a language](#select-a-language)
- [Select a scope](#select-a-scope)


## Create a view

Create a view with a predefined selection of the language, the scope, the product category, the variant view and the order of columns in the product list.

### Prerequisites

- At least one catalog is created, see [Create a catalog](#create-a-catalog).
- At least one category is created within the catalog, see [Create a category](#create-a-category).
- At least one product is assigned to the category, see [Assign a product to a catalog category](#assign-a-product-to-a-catalog-category)

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

### Next steps

- [To be completed](#to_be_completed)
- [To be completed](#to_be_completed)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [To be completed](#to_be_completed)
