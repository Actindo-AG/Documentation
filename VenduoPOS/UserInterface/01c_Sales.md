# Cash Register

*Venduo POS > Sales > Select Store and Pay Desk > Tab CASH REGISTER*

![Cash Register](/Assets/Screenshots/VenduoPOS/Sales/CashRegister/CashRegister.png "[Cash Register]")

The tab *Cash Register* is divided into two parts:
- [Payment Tally](#payment-tally)
- [Cash In/Out](#cash-in-out)

## Payment Tally

![Payment Tally](/Assets/Screenshots/VenduoPOS/Sales/CashRegister/PaymentTally.png "[Payment Tally]")

- ![Drawer](/Assets/Icons/Drawer.png "[Drawer]") (Open Drawer)  
  Click this button to open the cash drawer.

- [CLOSE REGISTER]   
  Click this button to close the pay desk. The pay desk can be closed only if an amount is entered in the field in the column *Counted*.

- *Payment Type*   
  Type of the cash amount in the pay desk. By default, the type is **Cash**. This field is read-only.

- *Currency*   
  Currency of the cash amount in the pay desk. A single row is displayed for each [available currency](02a_Management.md#available-currencies) defined in the global settings. This field is read-only.

- *Expected*   
  Cash amount in the pay desk expected by all transactions during the shift. If the setting *Erwarteten Betrag verbergen* in the [Global Settings](02a_Management.md#erwarteten-vertrag-verbergen) is active, the expected cash amount is hidden and a dash **-** is displayed. This field is read-only.

- *Counted*   
  Enter the counted cash amount in the pay desk by entering the amount directly in the field or clicking the button ![Calculator](/Assets/Icons/Calculator01.png "[Calculator]") (Calculator). The *Count cash* view is displayed.

- *Difference*   
  Difference amount between the expected and the counted cash amount in the pay desk. If no expected amount is displayed, no difference amount is displayed, but a dash **-**.

- *Skim to*   
  Enter a cash amount up to which the pay desk is skimmed after closing. If you have predefined a [skimming amount](02a_Management.md#abschöpfen-bis-betrag) in the global settings, the field is preset with this amount.


### Count Cash

*Venduo POS > Sales > Select Store and Pay Desk > Tab CASH REGISTER > Button Calculator*

![Count Cash](/Assets/Screenshots/VenduoPOS/Sales/CashRegister/CountCash.png "[Count Cash]")

- ![Back](/Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to cancel the cash counting and close the *Count cash* view.

- *Type*   
  Type of coins or banknotes of the default currency. The displayed types of coins and banknotes are defined by the [currencies](02a_Management.md#währungen) in the global settings.

- *Amount*   
  Enter the amount counted of the selected type of coins or banknotes by using the buttons or entering the amount directly into the field.

- ![Delete](/Assets/Icons/Trash06.png "[Delete]") (Delete)   
  Click this button to delete the entered amount of the selected type of coins or banknotes.

- [ +1 ]   
  Click this button to increase the counted amount of the selected type of coins or banknotes by 1.

- [ +5 ]   
  Click this button to increase the counted amount of the selected type of coins or banknotes by 5.

- [ +10 ]   
  Click this button to increase the counted amount of the selected type of coins or banknotes by 10.

- [ +50 ]   
  Click this button to increase the counted amount of the selected type of coins or banknotes by 50.

- [OK]   
  Click this button to confirm the counted cash amount and close the *Count cash* view.


## Cash In/Out

![Cash In/Out](/Assets/Screenshots/VenduoPOS/Sales/CashRegister/CashInOut.png "[Cash In/Out]")

- [ ![Drawer](/Assets/Icons/Drawer.png "[Drawer]") Open Drawer]  
  Click this button to open the cash drawer.

- [Cash in]   
  Click this button to post a cash in. The *Cash in* view is displayed.

- [Cash out]   
  Click this button to post a cash out. The *Cash out* view is displayed.

- *Description*   
  Short description of the cash in or cash out process. The first row always lists the opening float of the pay desk.

- *Currency*   
  Currency of the cash in or cash out process. This field is read-only.

- *Date*   
  Date and time of the cash in or cash out process.

- *Amount*   
  Cash amount of the cash in or cash out process.


### Cash in

*Venduo POS > Sales > Select Store and Pay Desk > Tab CASH REGISTER > Button Cash in*

![Cash In](/Assets/Screenshots/VenduoPOS/Sales/CashRegister/CashIn.png "[Cash In]")

- *Description*   
  Enter a short description for the cash in.

- *Amount*   
  Enter the cash amount of the cash in.

- [Currency]    
  Click this button to select the currency of the cash in. A single button is displayed for each [available currency](02a_Management.md#available-currencies) defined in the global settings.    

- ![Delete](/Assets/Icons/Trash03.png "[Delete]") (Delete)    
  Click this button to delete the entered cash in or cancel the cash in process and close the *Cash in* view.

- [Cash in]   
  Click this button to save the cash in and close the *Cash in* view.


### Cash out

*Venduo POS > Sales > Select Store and Pay Desk > Tab CASH REGISTER > Button Cash out*

![Cash Out](/Assets/Screenshots/VenduoPOS/Sales/CashRegister/CashOut.png "[Cash Out]")

- *Description*   
  Enter a short description for the cash out.

- *Amount*   
  Enter the cash amount of the cash out.

- [Currency]     
  Click this button to select the currency of the cash out. A single button is displayed for each [available currency](02a_Management.md#available-currencies) defined in the global settings.

- ![Delete](/Assets/Icons/Trash04.png "[Delete]") (Delete)    
  Click this button to delete the entered cash out or cancel the cash in process and close the *Cash out* view.

- [Cash in]   
  Click this button to save the cash out and close the *Cash out* view.
