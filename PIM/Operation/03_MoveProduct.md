# Move a product

Move a product to either archive it, move it to the recycle bin, delete it finally or restore it.

## Archive a product

[comment]: <> (Difference between archive and recycle bin)

### Prerequisites

At least one product is created, see [Create a product](01_ManageProducts.md#create-a-product).

### Procedure

*PIM > Products > Tab LIST*    
*PIM > Products > Tab RECYCLE BIN*

![List and recycle bin](/Assets/Screenshots/PIM/Products/ListRecycleBin.png "[List and recycle bin]")

> [Info] You can archive products from the product list or from the recycle bin. The procedure to archive them is identical. To archive a product from the recycle bin, start in the tab *RECYCLE BIN* instead of in the tab *LIST* and follow the steps described below.

1. Select the checkboxes ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") of the products you want to archive.   
  The editing toolbar is displayed above the products list.

2. Click the button [ARCHIVE PRODUCTS] in the toolbar.   
  The button changes to [ARCHIVING...]. The message *Product moved to archive* is displayed, indicating the number of archived products.

  ![Product moved to archive](/Assets/Screenshots/PIM/Products/List/ProductMovedToArchive.png "[Product moved to archive]")

  The selected products are archived.

  > [Info] You find the archived products in the tab *ARCHIVE* where you can either restore or delete them.

### Next steps

- [Delete a product](#delete-a-product)
- [Finally delete a product](#finally-delete-a-product)
- [Restore a product](#restore-a-product)
- [Manage the list view](04_ManageListView.md)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Manage the products](01_ManageProducts.md)
- [Manage the variants](02_ManageVariants.md)



## Delete a product

[comment]: <> (Difference between archive and recycle bin)

### Prerequisites

At least one product is created, see [Create a product](01_ManageProducts.md#create-a-product).

### Procedure

*PIM > Products > Tab LIST*   
*PIM > Products > Tab ARCHIVE*

![List and archive](/Assets/Screenshots/PIM/Products/ListArchive.png "[List and archive]")

> [Info] You can delete products from the product list or from the archive. The procedure to delete them is identical. To delete a product from the archive, start in the tab *ARCHIVE* instead of in the tab *LIST* and follow the steps described below.

1. Select the checkboxes ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") of the products you want to delete.   
  The editing toolbar is displayed above the products list.

2. Click the button [MOVE TO RECYCLE BIN] in the toolbar.   
  The button changes to [DELETING...]. The message *Product deleted* is displayed, indicating the number of deleted products.

  ![Product deleted](/Assets/Screenshots/PIM/Products/List/ProductDeleted.png "[Product deleted]")

  The selected products are moved to the recycle bin.

  > [Info] You find the deleted products in the tab *RECYCLE BIN* where you can either restore or finally delete them.

### Next steps

- [Finally delete a product](#finally-delete-a-product)
- [Restore a product](#restore-a-product)
- [Manage the list view](04_ManageListView.md)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Archive a product](#archive-a-product)
- [Manage the products](01_ManageProducts.md)
- [Manage the variants](02_ManageVariants.md)



## Finally delete a product

Products that have been moved to the recycle bin can be permanently deleted unless they have any existing dependencies. Be aware that the products cannot be restored as the deletion process cannot be undone.

### Prerequisites

At least one product is moved to the recycle bin, see [Delete a product](#delete-a-product).

### Procedure

*PIM > Products > Tab RECYCLE BIN*

![Recycle bin](/Assets/Screenshots/PIM/Products/RecycleBin/RecycleBin.png "[Recycle bin]")

1. Select the checkboxes ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") of the products you want to delete.   
  The editing toolbar is displayed above the products list.

2. Click the button [FINALLY DELETE PRODUCTS] in the toolbar.   
  The button changes to [DELETING...]. The message *Products deleted* is displayed, indicating the number of finally deleted products.

  ![Product deleted](/Assets/Screenshots/PIM/Products/List/ProductDeleted.png "[Product deleted]")

  The selected products are permanently deleted.

  > [Info] If the deletion is not possible, the message *Products deleted* is indicating an error for the number of products unable to delete. An error message with further information is displayed in the notifications.

  ![Product deleted error](/Assets/Screenshots/PIM/Products/List/ProductDeletedError.png "[Product deleted error]")

### Next steps

- [Restore a product](#restore-a-product)
- [Manage the list view](04_ManageListView.md)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Archive a product](#archive-a-product)
- [Delete a product](#delete-a-product)
- [Manage the products](01_ManageProducts.md)
- [Manage the variants](02_ManageVariants.md)



## Restore a product

Products that have been moved to the archive or the recycle bin can be restored in order to offer them again.

### Prerequisites

At least one product is moved to the archive or the recycle bin, see [Archive a product](#archive-a-product) or [Delete a product](#delete-a-product).

### Procedure

*PIM > Products > Tab ARCHIVE*   
*PIM > Products > Tab RECYCLE BIN*

![Archive and recycle bin](/Assets/Screenshots/PIM/Products/ArchiveRecycleBin.png "[Archive and recycle bin]")

> [Info] You can restore products from the archive or from the recycle bin. The procedure to restore them is identical. To restore a product from the recycle bin, start in the tab *RECYCLE BIN* instead of in the tab *ARCHIVE* and follow the steps described below.

1. Select the checkboxes ![Checkbox](/Assets/Icons/Checkbox.png "[Checkbox]") of the products you want to restore.   
  The editing toolbar is displayed above the products list.

2. Click the button [RESTORE PRODUCTS] in the toolbar.   
  The button changes to [RESTORING ...]. The message *Products restored* is displayed, indicating the number of restored products.

  ![Products restored](/Assets/Screenshots/PIM/Products/List/ProductsRestored.png "[Products restored]")

  The selected products are restored.

  > [Info] You find the restored products in the tab *LIST*.

### Next steps

- [Manage the list view](04_ManageListView.md)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Archive a product](#archive-a-product)
- [Delete a product](#delete-a-product)
- [Finally delete a product](#finally-delete-a-product)
- [Manage the products](01_ManageProducts.md)
- [Manage the variants](02_ManageVariants.md)
