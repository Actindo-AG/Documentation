# Channels

*DataHub > Settings > Tab CHANNELS*

![Channels](../../Assets/Screenshots/DataHub/Settings/Channels/ChannelList.png "[Channels]")

**Channel list**

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for a channel.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of channels.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all channels in the list are selected.

- [EDIT]   
  Click this button to edit the selected channel. This button is only displayed, when a single checkbox of a channel is selected. Alternatively, you can click directly a row in the list to edit a channel.
  For detailed information, see [Edit a channel](../Integration/04_ManageChannels.md#edit-a-channel).

- [DELETE]   
  Click this button to delete the selected channel. This button is only displayed, when the checkbox of at least one channel is selected.       

The list displays all channels. Depending on the settings, the displayed columns may vary. All fields are read-only.

- *Name*   
  Channel name.

- *Key*   
  Channel key.

- *Description*   
  Description to the channel.


- *Status*   
  Channel status. The following statuses are available:
  - ![Status](../../Assets/Icons/Status01.png "[Status]") **Active**
  - ![Status](../../Assets/Icons/Status04.png "[Status]") **Inactive**   


- *ID*   
  Channel identification number. The ID number is automatically assigned by the system.

- *Modified on*   
  Date and time of the last modification.

- *Modified by*   
  Name and username of the user who modified the channel.

- *Created on*   
  Date and time of the creation.

- *Created by*   
  Name and username of the user who created the channel.

- *Name (Language)*   
  Channel name in the selected language. A single *Name (Language)* column is displayed for the system languages *English (United States)* and *Deutsch (Deutschland)*.

- *Description (Language)*   
  Channel description in the displayed language. A single *Description (Language)* column is displayed for the system languages *English (United States)* and *Deutsch (Deutschland)*.

- ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add)   
  Click this button to create a channel. The *Create channel* view is displayed.   



## Create channel

*DataHub > Settings > Tab CHANNELS > Button Add*

![Create channel](../../Assets/Screenshots/DataHub/Settings/Channels/CreateChannel.png "[Create channel]")

**Create channel**

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *Create channel* view and return to the channel list. All changes are rejected.

- Language   
  Click the drop-down list and select the language in which the *Name (Language)* and *Description (Language)* fields are displayed. The system languages **English (United States)** and **Deutsch (Deutschland)** are available in the drop-down list.

- [SAVE]   
  Click this button to save the channel, close the *Create channel* view and return to the channel list.

- *Name (Language)*   
  Enter a channel name in the selected language.

- *Description (Language)*   
  Enter a description to the channel in the selected language.


- *Key*   
  Enter a channel key. The key is required for API access and must be system wide unique. A channel key must fulfill the following criteria:
  - valid characters are **a-z** (upper and lower case), **0-9** and the underscore ( **_** )
  - the key must not start with a number
  - a double underscore ( **___** ) and a trailing underscore are forbidden


- ![Toggle](../../Assets/Icons/Toggle.png "[Toggle]") *Active*   
  Enable this toggle to set the channel status to active. Disable the toggle to set the channel to inactive. By default, this toggle is disabled.



## Edit channel

*DataHub > Settings > Tab CHANNELS > Select channel*

![Edit channel](../../Assets/Screenshots/DataHub/Settings/Channels/EditChannel.png "[Edit channel]")

**Edit channel**

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *Edit channel* view and return to the channel list. All changes are rejected.

- Language   
  Click the drop-down list and select the language in which the *Name (Language)* and *Description (Language)* fields are displayed. The system languages **English (United States)** and **Deutsch (Deutschland)** are available in the drop-down list.

- [SAVE]   
  Click this button to save the channel, close the *Edit channel* view and return to the channel list.

- *Name (Language)*   
  Click the field to edit the channel name in the selected language.

- *Description (Language)*   
  Click the field to edit the description to the channel in the selected language.


- *Key*   
  Click the field to edit the channel key. It is not recommended to change the channel key after creation.   
  The key is required for API access and must be system wide unique. A channel key must fulfill the following criteria:
  - valid characters are **a-z** (upper and lower case), **0-9** and the underscore ( **_** )
  - the key must not start with a number
  - a double underscore ( **___** ) and a trailing underscore are forbidden


- ![Toggle](../../Assets/Icons/Toggle.png "[Toggle]") *Active*   
  Enable this toggle to set the channel status to active. Disable the toggle to set the channel to inactive. By default, this toggle is disabled.
