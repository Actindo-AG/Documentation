[!!PIM](Actindo/PIM)

# Issues with the data type

## The decimal places of a field are limited

### Error Description
When entering a floating number in a field with the *Floating point number*, *Stock Value* or *PIM Price Field* data type, the places of decimals are limited.

Follow the instructions below to check why the number of decimals is limited and, if applicable, change the number of decimal places.

[comment]: <> (Not yet working this way -> entering of more decimal places still possible, but the number is rounded to the indicated precision after saving)

### Prerequisites

No prerequisites to fulfill.

### Procedure

*PIM > Settings > Tab ATTRIBUTES*

![Attributes](/Assets/Screenshots/PIM/Settings/Attributes/Attributes.png "[Attributes]")

1. Search for the respective attribute in the attribute list.

2. Click the respective attribute in the attribute list.   
  The *Edit Attribute* view is displayed.

3. Check the following attribute settings:
  - ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Multi-language*      
    Check if the toggle is deactivated. Only single language attributes can be used as defining attributes for a variant set.
  - ![Toggle](/Assets/Icons/Toggle.png "[Toggle]") *Multi-channel*      
    Check if the toggle is deactivated. Only single channel attributes can be used as defining attributes for a variant set.

    > [Info] If the respective attribute is multi-language or multi-channel, it cannot be used as defining attribute. [Create a new attribute](/PIM/Integration/01_ManageAttributes.md#create-an-attribute) which is not multi-language nor multi-channel to use it as a defining attribute.    

### See also

- [User Interface PIM](/PIM/UserInterface/00_UserInterface.md)
- [Create a variant set](/PIM/Integration/07_ManageVariantSets.md#create-a-variant-set)
- [Edit a variant set](/PIM/Integration/07_ManageVariantSets.md#edit-a-variant-set)
- [Add defining attributes](/PIM/Integration/07_ManageVariantSets.md#add-defining-attributes)
- [Create an attribute](/PIM/Integration/01_ManageAttributes.md#create-an-attribute)


### Was this chapter helpful?

If you need further assistance, please contact the Customer Support.
