[!!Cloudinary](Cloudinary)
[!!DataHub](DataHub)


# Map a Cloudinary file

The Cloudinary files can be output to web shops or marketplaces from Actindo or be input from an web shop or marketplace to Actindo and Cloudinary by mapping these files via the *DataHub* module. During the mapping process, the images remain stored in Cloudinary, as the ETL mapping uses only the URL and the public ID of the Cloudinary images. In this way, also transformations in the images can be provided.   
The mapping procedure of a Cloudinary attribute is identical to the mapping of any other attribute which is also described in the *DataHub* documentation, see [Manage the ETL mappings](/DataHub/Operation/01_ManageETLMappings.md).
Nevertheless, the possible mappings of a Cloudinary attribute, both, from an external source or to an external source is described in this chapter below.   


## Map a cloudinary source attribute

Map a source attribute set with a Cloudinary attribute to a certain destination attribute set, for instance to transfer the Cloudinary files from the PIM products to an external web shop or marketplace.

#### Prerequisites

- At least one ETL attribute set mapping is created, see [Create an ETL mapping](/DataHub/Operation/01_ManageETLMappings.md#create-an-ETL-mapping).
- The Cloudinary attribute is assigned to the source attribute set of the mapping.

#### Procedure

*DataHub > Settings > Tab ETL*

![Attribute set mappings](/Assets/Screenshots/DataHub/Settings/ETL/AttributeSetMappings.png "[Attribute set mappings]")

> [Info] The following procedure describes exemplary how to map a Cloudinary image attribute. The procedure is largely identical to map a Cloudinary video attribute. The differences are explicitly specified at the appropriate place.

1. Click the attribute set mapping you want to edit in the list of attribute set mappings.   
  The *Mapping from source set to destination set* view is displayed.

  ![Mapping](/Assets/Screenshots/DataHub/Settings/ETL/Mapping.png "[Mapping]")

2. Click the row with the destination attribute to which you want to map the Cloudinary image attribute. The destination attribute must have either the *String* data type or the *Cloudinary image* data type.  
  The *Settings* section is displayed on the right side.

  ![Cloudinary source attribute](/Assets/Screenshots/DataHub/Settings/ETL/CloudinarySourceAttribute.png "[Cloudinary source attribute]")

  > [Info] Depending on the selected row, the fields displayed in the *Settings* section differ:
  - If the selected row contains only a destination attribute, the destination attribute as well as the *Extension* and *Override change tracking mode* drop-down lists are displayed.
  - If the selected row contains an attribute mapping with source, destination attribute and the extension, the destination attribute as well as the *Source attribute*, *Extension* and *Override change tracking mode* drop-down lists are displayed. The *Source attribute*, *Extension* and *Override change tracking mode* drop-down lists are preset. If the selected extension requires further configuration settings, the *Configuration* section is displayed below the *Settings* section.  


3. Select the appropriate option in the *Extension* drop-down list in the *Settings* section. The following extensions are available to map a Cloudinary source attribute with:
  - **Copy cloudinary image value**: Copy the value from the Cloudinary image attribute and map it to another Cloudinary image attribute. This extension is only available for a destination attribute with the *Cloudinary image* data type.
  - **Cloudinary to string**: Map a Cloudinary image to a string attribute. If desired, the image transformation can also be mapped to the destination attribute. This extension is only available for a destination attribute with the *String* data type.

  The *Configuration* section is displayed below the *Settings* section.

  > [Info] For detailed information about the ETL extensions, see [ETL extensions list](/DataHub/UserInterface/03_ETLExtensions.md).   
  For detailed information about the data types, see [Data type list](/PIM/UserInterface/04_DataTypeList.md).

4. Select the appropriate tracking mode in the *Override change tracking mode* drop-down list. By default, the **Use default** option is preselected. The following modes are available:
  - **Use default**: ---
  - **Automatic**: The initial mapping is automatically applied. All value changes or reruns are applied automatically in the mapping.  
  - **Semi-automatic**: The initial mapping is automatically applied. Values changes or reruns are applied after confirmation in the *Omni-Channel* module.
  - **Semi-automatic, changes must be confirmed by another user**: The initial mapping as well as values changes or reruns are applied after confirmation by another user in the *Omni-Channel* module.
  - **Manual**: The initial mapping is automatically applied. Afterwards, the changes in the mapping must be triggered manually to be applied.


5. Select the Cloudinary attribute(s) that you want to assign to the destination attribute. For the *Copy cloudinary image value* ETL extension, you have to select a single Cloudinary source attribute. For the *Cloudinary to string* ETL extension, you can select one to four Cloudinary source attributes and, if desired, add a transformation.

6. When having selected the *Copy cloudinary image value* ETL extension, enter the Cloudinary folder from which the images will be imported in the *Folder* field of the *Configuration* section.    
When having selected the *Cloudinary to string* ETL extension, enable or disable the toggle to export the Cloudinary public ID instead of the Cloudinary image URL.

  > [Info] Note that transformations can only be mapped if the *Export public ID* toggle is disabled.

7. Click the [SAVE] button in the upper right corner.   
  The changes are saved. The *Settings* section is hidden.

  > [Info] Be aware that you have to [rerun the mapping](/DataHub/Operation/01_ManageETLMappings.md#rerun-an-etl-mapping) to apply the changes made to the attribute.



## Map a Cloudinary destination attribute

Map a certain source attribute set to a destination attribute set with a Cloudinary attribute, for instance to transfer the media files from an external web shop or marketplace to the PIM product and import them to Cloudinary.

#### Prerequisites

- At least one ETL attribute set mapping is created, see [Create an ETL mapping](/DataHub/Operation/01_ManageETLMappings.md#create-an-ETL-mapping).
- The Cloudinary attribute is assigned to the destination attribute set of the mapping.

#### Procedure

*DataHub > Settings > Tab ETL*

![Attribute set mappings](/Assets/Screenshots/DataHub/Settings/ETL/AttributeSetMappings.png "[Attribute set mappings]")

> [Info] The following procedure describes exemplary how to map a Cloudinary image attribute. The procedure is largely identical to map a Cloudinary video attribute. The differences are explicitly specified at the appropriate place.

1. Click the attribute set mapping you want to edit in the list of attribute set mappings.   
  The *Mapping from source set to destination set* view is displayed.

  ![Mapping](/Assets/Screenshots/DataHub/Settings/ETL/Mapping.png "[Mapping]")

2. Click the row with the Cloudinary image destination attribute.   
  The *Settings* section is displayed on the right side.

  ![Cloudinary destination attribute](/Assets/Screenshots/DataHub/Settings/ETL/CloudinaryDestinationAttribute.png "[Cloudinary destination attribute]")

  > [Info] Depending on the selected row, the fields displayed in the *Settings* section differ:
  - If the selected row contains only a destination attribute, the destination attribute as well as the *Extension* and *Override change tracking mode* drop-down lists are displayed.
  - If the selected row contains an attribute mapping with source, destination attribute and the extension, the destination attribute as well as the *Source attribute*, *Extension* and *Override change tracking mode* drop-down lists are displayed. The *Source attribute*, *Extension* and *Override change tracking mode* drop-down lists are preset. If the selected extension requires further configuration settings, the *Configuration* section is displayed below the *Settings* section.  


3. Select the appropriate option in the *Extension* drop-down list in the *Settings* section. The following extensions are available for the Cloudinary destination attribute:
  - **Copy cloudinary image value**: Copy the value from the Cloudinary image attribute and map it to another Cloudinary image attribute.
  - **Import from cloudinary folder**: Import all image files within a specified folder in Cloudinary to the Cloudinary attribute.    

  The *Configuration* section is displayed below the *Settings* section.

  > [Info] For detailed information about the ETL extensions, see [ETL extensions list](/DataHub/UserInterface/03_ETLExtensions.md).

4. Select the appropriate tracking mode in the *Override change tracking mode* drop-down list. By default, the **Use default** option is preselected. The following modes are available:
  - **Use default**: ---
  - **Automatic**: The initial mapping is automatically applied. All value changes or reruns are applied automatically in the mapping.  
  - **Semi-automatic**: The initial mapping is automatically applied. Values changes or reruns are applied after confirmation in the *Omni-Channel* module.
  - **Semi-automatic, changes must be confirmed by another user**: The initial mapping as well as values changes or reruns are applied after confirmation by another user in the *Omni-Channel* module.
  - **Manual**: The initial mapping is automatically applied. Afterwards, the changes in the mapping must be triggered manually to be applied.


5. Select the appropriate attribute(s) that you want to assign to the Cloudinary destination attribute. For the *Copy cloudinary image value* ETL extension, you have to select a source attribute with the *Cloudinary image* data type. For the *Import from cloudinary folder* ETL extension, you can select one to four source attributes with the *String* data type.

  > [Info] For detailed information about the data types, see [Data type list](/PIM/UserInterface/04_DataTypeList.md).

6. When having selected the *Copy cloudinary image value* ETL extension, enter the Cloudinary folder from which the images will be imported in the *Folder* field of the *Configuration* section.   

7. Click the [SAVE] button in the upper right corner.   
  The changes are saved. The *Settings* section is hidden.

  > [Info] Be aware that you have to [rerun the mapping](/DataHub/Operation/01_ManageETLMappings.md#rerun-an-etl-mapping) to apply the changes made to the attribute.



## Related content

- [User Interface DataHub](/DataHub/UserInterface/00_UserInterface.md)
- [Manage the ETL mappings](/DataHub/Operation/01_ManageETLMappings.md)
- [ETL extensions list](/DataHub/UserInterface/03_ETLExtensions.md)
- [Data type list](/PIM/UserInterface/04_DataTypeList.md)
