[!!PIM](Actindo/PIM)

# Add a missing defining attribute

## Error Description
A certain attribute is missing in the list of defining attributes for a variant set.

Follow the instructions below to check why the attribute is not displayed and, if applicable, to display the attribute in the list.


## Prerequisites

No prerequisites to fulfill.

## Procedure

*PIM > Settings > Tab ATTRIBUTES*

![Attributes](/Assets/Screenshots/PIM/Settings/Attributes/Attributes.png "[Attributes]")

1. Search for the respective attribute in the attribute list.

2. Click the respective attribute in the attribute list.   
  The *Edit Attribute* view is displayed.

  ![Edit attribute](/Assets/Screenshots/PIM/Settings/Attributes/EditAttribute_Data.png "[Edit attribute]")

3. Check the following attribute settings:
  - ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Multi-language*      
    Check if the toggle is deactivated. Only single language attributes can be used as defining attributes for a variant set.
  - ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Multi-channel*      
    Check if the toggle is deactivated. Only single channel attributes can be used as defining attributes for a variant set.

    > [Info] If the respective attribute is multi-language or multi-channel, it cannot be used as defining attribute. [Create a new attribute](/PIM/Integration/01_ManageAttributes.md#create-an-attribute) which is not multi-language nor multi-channel to use it as a defining attribute.    

4. Check if the ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Active* toggle is activated. Only active attributes are displayed in the list of defining attributes for a variant set. If the toggle is deactivated, activate the toggle by clicking it.

5. Click the [SAVE] button in the upper right corner to save any changes.   
  The changes are applied. The *Edit Attribute* view is closed.

6. Press **F5** to initialize the Core1 Platform.

7. Switch to the *VARIANT SETS* tab: *PIM > Settings > Tab VARIANT SETS* .      
  The variant sets list is displayed.

  ![Variant sets](/Assets/Screenshots/PIM/Settings/VariantSets/VariantSets.png "[Variant sets]")

8. Create a new variant set or select the variant set to which you want to add the defining attribute. For detailed information, see [Create a variant set](/PIM/Integration/07_ManageVariantSets.md#create-a-variant-set) or [Edit a variant set](/PIM/Integration/07_ManageVariantSets.md#edit-a-variant-set).

  ![Formulas](/Assets/Screenshots/PIM/Settings/VariantSets/Formulas.png "[Formulas]")

9. In the *Defining attributes* box, click the ![Add](/Assets/Icons/Plus01.png "[Add]") button.   
  The *Add defining attributes* view is displayed.

  ![Add defining attributes](/Assets/Screenshots/PIM/Settings/VariantSets/AddDefiningAttributes.png "[Add defining attributes]")

10. Check if the respective attribute is displayed in the list.

  > [Info] You may click the ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh) button to update the list of defining attributes.    
  If the attribute is still not displayed, please contact the Customer Support.    

11. Add the attribute to the variant set as described in [Add defining attributes](/PIM/Integration/07_ManageVariantSets.md#add-defining-attributes).


## See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create a variant set](/PIM/Integration/07_ManageVariantSets.md#create-a-variant-set)
- [Edit a variant set](/PIM/Integration/07_ManageVariantSets.md#edit-a-variant-set)
- [Add defining attributes](/PIM/Integration/07_ManageVariantSets.md#add-defining-attributes)
- [Create an attribute](/PIM/Integration/01_ManageAttributes.md#create-an-attribute)
- [Data type list](/PIM/UserInterface/04_DataTypeList.md)


## Was this chapter helpful?

If you need further assistance, please contact the Customer Support.
