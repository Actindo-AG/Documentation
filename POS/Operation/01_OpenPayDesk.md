[!!Manage the cash register](./05_ManageCashRegister.md)
[!!User interface Sales](../UserInterface/01_Sales.md)

# Open a pay desk

The pay desk is the most important tool in the *Venduo POS* module.
For instance, in the pay desk you can select offers, make payments, give discounts, choose between different payment methods and have the possibility to park purchases for a later date.
To perform any operation on the pay desk, you must first open one.

#### Prerequisites

- A store including a pay desk is created, see [Create a store in POS](../Integration/06_CreateStore.md).
- The user logged in must be assigned to a POS group, see [Assign users to the POS groups](../Integration/04_AssignUsers.md).
- Depending on the assigned POS group, the user must fulfill the following requirements:
    - A POS admin does not need to meet any further requirements.
    - A store manager has to be assigned to the corresponding store, see [Configure the store details](../Integration/06_CreateStore.md#configure-the-store-details).
    - A cashier has to be assigned to the pay desk, see [Configure the pay desk details](../Integration/06_CreateStore.md#configure-the-pay-desk-details).
- The pay desk is not in use, see [Remove an inactive cashier from the pay desk](../Troubleshooting/03_RemoveInactiveCashier.md).

#### Procedure

*Venduo POS > Sales > Tab CASHPOINT*

![POS Sales Select](../../Assets/Screenshots/POS/Sales/Select.png "[POS Sales Select]")

1. Select a store in the *Select store* drop-down list.

2. Select a pay desk in the *Select pay desk* drop-down list.

3. Click the [Use] button in the bottom right corner.   
    A window to edit the opening float is displayed. The opening float is the amount of cash available in the pay desk.

    ![Opening Float](../../Assets/Screenshots/POS/Sales/OpeningFloat.png "[Opening Float]")

4. Enter the opening float in the *Opening float* field.

    > [Info] If the opening float differs from the closing float of the pay desk, an opening difference is recorded in the payment tally of the cash register, which is synced to the *Accounting* module. The opening difference is also indicated in the shift summary.

5. Click the [Open] button in the bottom right corner.   
    The selected pay desk is opened. The selected tab is displayed.
