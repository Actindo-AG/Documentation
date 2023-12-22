[!!Exports](../UserInterface/01_Exports.md)

# Manage mapping settings

The mapping settings define some basic data that is needed to be able to send EDIFACT message the *Actindo* to your business partner.

## Create mapping setting
 Create the mapping settings.

#### Prerequisites
At least one definition setting has been created, see [Create basic definition settings](#create-basic-definition-settings).
>[INFO] The *Mapping settings* tab is visible only if you have created and saved a basic definition setting. 

#### Procedure
*DataHub Exporter > Exports*

![Export definitions](../../Assets/Screenshots/EDI/Operation/ExportDefinitions.png "[Export definitions]")

1. Click the exporter definition for which you want to define the mapping settings.   
    The *Edit definition "Definition name"* view is displayed. The last selected tab is displayed by default.

2. Click the *Mapping settings* tab.   
    The mapping settings are displayed.

    ![Mapping settings](../../Assets/Screenshots/EDI/Operation/MappingSettingsCreate.png "[Mapping settings]")

3. Click the *Return format* drop-down list and select **EDI**. 

4. Enter the standard encoding (for example, UTF-8) required by your business partner in the *Convert to charset (iconv)* field. The *DataHub exporter* need it to process the conversion. 

5. Enter your company's GLN (Global location number) in the *Sender* field. This information is used for the EDIFACT UNB S002 (Interchange sender) segment that is automatically filled by the exporter.

6. If your business partner requires it, enter the identification code qualifier in the *Sender identification code qualifier* field. 

7. Enter the GLN number of the receiver's company in the *Receiver* field. This information is used for the EDIFACT UNB S003 (Interchange recipient) segment that is automatically filled by the exporter.
  
8. Click the [SAVE] button.   
   The *Exporter definitions* view is displayed. 


## Edit mapping setting

Edit the mapping settings.

#### Prerequisites
- At least one definition setting has been created, see [Create basic definition settings](#create-basic-definition-settings).
- The mapping setting for a definition has been created.

#### Procedure
*DataHub Exporter > Exports*

![Export definitions](../../Assets/Screenshots/EDI/Operation/ExportDefinitions.png "[Export definitions]")

1. Click the exporter definition for which you want to define the mapping settings.   
    The *Edit definition "Definition name"* view is displayed. The *Settings* tab is displayed by default.

2. Click the *Mapping settings* tab.   
    The already defined mapping settings are displayed.

    ![Mapping settings](../../Assets/Screenshots/EDI/Operation/MappingSettingsCreated.png "[Mapping settings]")

3. If desired, change your settings.

4. Click the [SAVE] button.   
   The *Exporter definitions* view is displayed. 
