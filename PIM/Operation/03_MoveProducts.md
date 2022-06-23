[!!PIM](PIM)

# Move a product

Move a product to either archive it, move it to the recycle bin, delete it finally or restore it.

## Archive a product

You can archive products that you are not currently using, but that you still want to access and may want to use again at a later time. Archived products cannot be finally deleted but must first be moved to the recycle bin.

### Prerequisites

At least one product is created, see [Create a product](01_ManageProducts.md#create-a-product).

### Procedure

*PIM > Products > Tab LIST*    
*PIM > Products > Tab RECYCLE BIN*

![List and recycle bin](/Assets/Screenshots/PIM/Products/ListRecycleBin.png "[List and recycle bin]")

> [Info] You can archive products from the product list or from the recycle bin. The procedure to archive them is identical. To archive a product from the recycle bin, start in the *RECYCLE BIN* tab instead of in the *LIST* tab and follow the steps described below.

1. Select the checkboxes of the products you want to archive.   
  The editing toolbar is displayed above the products list.

2. Click the [ARCHIVE PRODUCTS] button in the toolbar.   
  The button changes to [ARCHIVING...]. The *Product moved to archive* pop-up window is displayed, indicating the number of archived products.

  ![Product moved to archive](/Assets/Screenshots/PIM/Products/List/ProductMovedToArchive.png "[Product moved to archive]")

  The selected products are archived.

  > [Info] You find the archived products in the *ARCHIVE* tab where you can either restore or delete them.

### Next steps

- [Delete a product](#delete-a-product)
- [Finally delete a product](#finally-delete-a-product)
- [Restore a product](#restore-a-product)
- [Manage the view](04_ManageView.md)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Manage the products](01_ManageProducts.md)
- [Manage the variants](02_ManageVariants.md)



## Delete a product

You can delete products that are no longer needed by moving them to the recycle bin. Products in the recycle bin can still be restored or archived but they also can be finally deleted.

### Prerequisites

At least one product is created, see [Create a product](01_ManageProducts.md#create-a-product).

### Procedure

*PIM > Products > Tab LIST*   
*PIM > Products > Tab ARCHIVE*

![List and archive](/Assets/Screenshots/PIM/Products/ListArchive.png "[List and archive]")

> [Info] You can delete products from the product list or from the archive. The procedure to delete them is identical. To delete a product from the archive, start in the *ARCHIVE* tab instead of in the *LIST* tab and follow the steps described below.

1. Select the checkboxes of the products you want to delete.   
  The editing toolbar is displayed above the products list.

2. Click the [MOVE TO RECYCLE BIN] button in the toolbar.   
  The button changes to [DELETING...]. The *Product deleted* pop-up window is displayed, indicating the number of deleted products.

  ![Product deleted](/Assets/Screenshots/PIM/Products/List/ProductDeleted.png "[Product deleted]")

  The selected products are moved to the recycle bin.

  > [Info] You find the deleted products in the *RECYCLE BIN* tab where you can either restore or finally delete them.

### Next steps

- [Finally delete a product](#finally-delete-a-product)
- [Restore a product](#restore-a-product)
- [Manage the view](04_ManageView.md)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Archive a product](#archive-a-product)
- [Manage the products](01_ManageProducts.md)
- [Manage the variants](02_ManageVariants.md)



## Finally delete a product

You can permanently delete products Products that have been moved to the recycle bin unless they have any existing dependencies. Be aware that once deleted products cannot be restored as the deletion process cannot be undone.

### Prerequisites

At least one product is moved to the recycle bin, see [Delete a product](#delete-a-product).

### Procedure

*PIM > Products > Tab RECYCLE BIN*

![Recycle bin](/Assets/Screenshots/PIM/Products/RecycleBin/RecycleBin.png "[Recycle bin]")

1. Select the checkboxes of the products you want to delete.   
  The editing toolbar is displayed above the products list.

2. Click the [FINALLY DELETE PRODUCTS] button in the toolbar.   
  The button changes to [DELETING...]. The *Products finally deleted* pop-up window is displayed, indicating the number of finally deleted products.

  ![Product finally deleted](/Assets/Screenshots/PIM/Products/RecycleBin/ProductFinallyDeleted.png "[Product finally deleted]")

  The selected products are permanently deleted.

  > [Info] If the deletion is not possible, the *Products deleted* pop-up window is indicating an error for the number of products unable to delete. An error message with further information is displayed in the notifications.

  ![Product deleted error](/Assets/Screenshots/PIM/Products/List/ProductDeletedError.png "[Product deleted error]")

### Next steps

- [Restore a product](#restore-a-product)
- [Manage the view](04_ManageView.md)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Archive a product](#archive-a-product)
- [Delete a product](#delete-a-product)
- [Manage the products](01_ManageProducts.md)
- [Manage the variants](02_ManageVariants.md)



## Restore a product

You can restore products that have been moved to the archive or the recycle bin in order to use them again.

### Prerequisites

At least one product is moved to the archive or the recycle bin, see [Archive a product](#archive-a-product) or [Delete a product](#delete-a-product).

### Procedure

*PIM > Products > Tab ARCHIVE*   
*PIM > Products > Tab RECYCLE BIN*

![Archive and recycle bin](/Assets/Screenshots/PIM/Products/ArchiveRecycleBin.png "[Archive and recycle bin]")

> [Info] You can restore products from the archive or from the recycle bin. The procedure to restore them is identical. To restore a product from the recycle bin, start in the *RECYCLE BIN* tab instead of in the *ARCHIVE* tab and follow the steps described below.

1. Select the checkboxes of the products you want to restore.   
  The editing toolbar is displayed above the products list.

2. Click the [RESTORE PRODUCTS] button in the toolbar.   
  The button changes to [RESTORING ...]. The *Products restored* pop-up window is displayed, indicating the number of restored products.

  ![Products restored](/Assets/Screenshots/PIM/Products/List/ProductsRestored.png "[Products restored]")

  The selected products are restored.

  > [Info] You find the restored products in the *LIST* tab.

### Next steps

- [Manage the view](04_ManageView.md)

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Archive a product](#archive-a-product)
- [Delete a product](#delete-a-product)
- [Finally delete a product](#finally-delete-a-product)
- [Manage the products](01_ManageProducts.md)
- [Manage the variants](02_ManageVariants.md)
