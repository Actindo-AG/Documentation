[!!DataHub](Actindo/DataHub)

# Manage the ETL mappings

An ETL attribute set mapping is used to extract the data from an source attribute set, transform it according to a specified method, and load it into a destination attribute set. You can create mappings, edit existing mappings, rerun mappings and check the current ETL processes.

[comment]: <> (ETL mapping description -> what is it used for)

## Create an ETL mapping

Create an ETL mapping to map the attributes of the source attribute set to the attributes of the destination attribute set. The mapping allows to convert the attributes from the source set to fit the attributes required by the destination set.

### Prerequisites

Attribute sets are created, see [Create an attribute set](02_ManageAttributeSets.md#Create-an-attribute-set).

### Procedure
*DataHub > Settings > Tab ETL*

![Attribute set mappings](/Assets/Screenshots/DataHub/Settings/ETL/AttributeSetMappings.png "[Attribute set mappings]")

1. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The *Create ETL Attribute Set Mapping* window is displayed.

  ![Create ETL Attribute Set Mapping](/Assets/Screenshots//DataHub/Settings/ETL/CreateETLAttributeSetMapping.png "[Create ETL Attribute Set Mapping]")

2. Select a source attribute set in the *Source attribute set* drop-down list. All active attribute sets are displayed in the drop-down list.

3. Select a destination attribute set in the *Destination attribute set* drop-down list. All active attribute sets are displayed in the drop-down list.
  If any attribute set with the selected destination attribute set already exists, the *Copy ETL Attribute Set Mapping* drop-down list is unlocked.

4. Select a language in the *Language* drop-down list. All active languages are displayed in the drop-down list.

  > [Info] The selected language defines the language from which the value of an multilingual attribute is taken when mapping it to a single language attribute.

5. Select a channel in the *Channel* drop-down list. All active channels are displayed in the drop-down list.

  > [Info] The selected channel defines the channel from which the value of an multi-channel attribute is taken when mapping it to a single channel attribute.

6. If desired, select an existing ETL attribute set mapping in the *Copy ETL Attribute Set Mapping* drop-down list. All attribute set mappings whose destination attribute set matches or has inheritance relations to the selected destination attribute set are displayed in the drop-down list.

  > [Info] If you select an ETL attribute set mapping in the drop-down list, all matching attribute mappings are applied to the new ETL attribute set mapping.

7. Click the [SAVE] button in the bottom right corner.   
  The new attribute set mapping is saved and displayed in the list of attribute set mappings. The *Create ETL Attribute Set Mapping* window is closed.

### Next steps

- [Edit an ETL mapping](#edit-an-etl-mapping)
- [Rerun an ETL mapping](#rerun-an-etl-mapping)
- [Check the ETL processes](#check-the-etl-processes)

### See also

- [User Interface DataHub](/DataHub/UserInterface/00_UserInterface.md)
- [Manage an attribute set](/DataHub/Integration/02_ManageAttributeSets.md)


## Edit an ETL mapping

After you have created an attribute set mapping, you can edit it. You can edit the

[comment]: <> (to_be_completed)

### Prerequisites

At least one ETL attribute set mapping is created, see [Create an ETL mapping](#create-an-ETL-mapping).

### Procedure
*DataHub > Settings > Tab ETL*

![Attribute set mappings](/Assets/Screenshots/DataHub/Settings/ETL/AttributeSetMappings.png "[Attribute set mappings]")

1. Click the attribute set mapping you want to edit in the list of attribute set mappings.   
  The *Mapping from source Set to destination set* view is displayed.

  ![Mapping](/Assets/Screenshots/DataHub/Settings/ETL/Mapping.png "[Mapping]")

2. Select the row of the attribute you want to map on the left part of the *Mapping* view.   
  The section *Settings* is displayed on the right side.

  ![Mapping settings](/Assets/Screenshots/DataHub/Settings/ETL/MappingSettings.png "[Mapping settings]")

3. Select the appropriate option in the drop-down list *Extension* in the section *Settings*.
  The section *Configuration* is displayed in the section *Settings*.

  > [Info] A list of all mapping extensions and their configuration options can be found ---where---???.

4. Select the appropriate tracking mode in the drop-down list *Override Changetrackingmode*. The following modes are available:
  - **use default**: ---
  - **automatic**: the attribute value is automatically adopted for the mapping. The mapping is rerun automatically when a value changes.  
  - **semi-automatic**: the attribute value is adopted for the mapping after confirmation. The mapping is rerun automatically after it has been confirmed.
  - **manual**: the attribute value is adopted one time for the mapping. Afterwards, the mapping is only rerun if it is started manually.


5. Select the appropriate source attribute that you want to assign to the destination attribute in the drop-down list *Source attribute* .

  > [Info] Only attributes that equal to the selected extension are displayed in the drop-down list *Source attribute*.

6. If required, set the corresponding mapping configurations.

7. Click the [SAVE] button in the upper right corner.   
  The changes are saved. The *Mapping from source Set to destination set* view is closed.  

> [Info] Repeat step **2** to **7** for all attributes you want to map.

### Next steps

- [Rerun an ETL mapping](#rerun-an-etl-mapping)
- [Check the ETL processes](#check-the-etl-processes)


### See also

- [User Interface DataHub](/DataHub/UserInterface/00_UserInterface.md)
- [Create an ETL mapping](#create-an-etl-mapping)
- [Manage an attribute set](/DataHub/Integration/02_ManageAttributeSets.md)




## Rerun an ETL mapping


### Prerequisites


### Procedure
*DataHub > Settings > Tab ETL*


### Next steps

- [Check the ETL processes](#check-the-etl-processes)

### See also

- [User Interface DataHub](/DataHub/UserInterface/00_UserInterface.md)
- [Create an ETL mapping](#create-an-etl-mapping)
- [Edit an ETL mapping](#edit-an-etl-mapping)
- [Manage an attribute set](/DataHub/Integration/02_ManageAttributeSets.md)




## Check the ETL processes


### Prerequisites


### Procedure
*DataHub > Settings > Tab ETL*


### Next steps


### See also

- [User Interface DataHub](/DataHub/UserInterface/00_UserInterface.md)
- [Create an ETL mapping](#create-an-etl-mapping)
- [Edit an ETL mapping](#edit-an-etl-mapping)
- [Rerun an ETL mapping](#rerun-an-etl-mapping)
- [Manage an attribute set](/DataHub/Integration/02_ManageAttributeSets.md)
