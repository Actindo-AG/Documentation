# Connections

*Cloudinary > Settings > Tab CONNECTIONS*

![Connections](/Assets/Screenshots/Cloudinary/Settings/Connections.png "[Connections]")

- ![Refresh](/Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of Cloudinary connections.

- ![Columns](/Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- [x]     
  Select the checkbox to display the editing toolbar.

- ![Edit](/Assets/Icons/Edit01.png "[Edit]") (Edit)         
  Click this button to edit the selected connection. This button is only displayed, when the checkbox of a single connection is selected. Alternatively, you can click directly a row in the list to edit a connection.

The list displays all Cloudinary connections. All fields are read-only. Depending on the settings, the displayed columns may vary.

- *ID*   
  Connection identification number. The ID number is automatically assigned by the system.

- *Name*   
  Connection name.


- ![Add](/Assets/Icons/Plus01.png "[Add]") (Add)   
  Click this button to add a Cloudinary connection. The *Connection* view is displayed.   


## Create connection

*Cloudinary > Settings > Tab CONNECTIONS > Button Add*

![Create connection](/Assets/Screenshots/Cloudinary/Settings/CreateConnection.png "[Create connection]")

- *Name*   
  Enter a name for the Cloudinary connection.

- *Driver*   
  Click the drop-down list and select the approriate driver for the Cloudinary connection. All available drivers are displayed. The *Credentials* section is displayed.

  > [Info] Currently, the *Cloudinary Default Driver* is configured as a standard driver for Cloudinary. Further drivers that differ in their behavior may be created for specific customer needs.

**Credentials**

This section is only displayed when a driver has been selected in the *Driver* drop-down list.

![Credentials](/Assets/Screenshots/Cloudinary/Settings/Credentials.png "[Credentials]")

- *Cloud-Name*   
  Enter the cloud name from the Cloudinary account to which you want to establish a connection. The cloud name is displayed on the dashboard of your Cloudinary account.

- *API-Key*   
  Enter the API key from the Cloudinary account to which you want to establish a connection. The API key is displayed on the dashboard of your Cloudinary account.

- *API-Secret*   
  Enter the API secret from the Cloudinary account to which you want to establish a connection. The API secret is displayed on the dashboard of your Cloudinary account.

- [SAVE]   
  Click this button to establish the connection to the indicated Cloudinary account. The *Connection* view is closed. The new connection is displayed in the list of connections.
