[!!Create a language](../Integration/05_ManageLanguages.md#create-a-language)
[!!Edit a language](../Integration/05_ManageLanguages.md#edit-a-language)
[!!Delete a language](../Integration/05_ManageLanguages.md#delete-a-language)
[!!Deactivate a language](../Integration/05_ManageLanguages.md#deactivate-a-language)


# Languages

*DataHub > Settings > Tab LANGUAGES*

![Languages](../../Assets/Screenshots/DataHub/Settings/Languages/LanguageList.png "[Languages]")

**Language list**

- ![Search](../../Assets/Icons/Search.png "[Search]") (Search)   
  Click this button to display the search bar and search for a language.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)   
  Click this button to update the list of languages.

- ![Columns](../../Assets/Icons/Columns.png "[Columns]") Columns (x)   
  Click this button to display the columns bar and customize the displayed columns and the order of columns in the list. The *x* indicates the number of columns that are currently displayed in the list.

- ![Filter](../../Assets/Icons/Filter.png "[Filter]") Filter (x)   
  Click this button to display the filter bar and customize the active filters. The *x* indicates the number of filters that are currently active.

- [x]     
  Select the checkbox to display the editing toolbar. If you click the checkbox in the header, all languages in the list are selected.

- [EDIT]   
  Click this button to edit the selected language. This button is only displayed if a single checkbox of a language is selected. Alternatively, you can click directly a row in the list to edit a language.

- [DELETE]   
  Click this button to delete the selected language. This button is only displayed if the checkbox of at least one language is selected.       

The list displays all language. Depending on the settings, the displayed columns may vary. All fields are read-only.

- *Key*   
  Language key.

- *Language*   
  Language name.

- *ID*   
  Language identification number. The ID number is automatically assigned by the system.

- *Modified on*   
  Date and time of the last modification.

- *Modified by*   
  Name and username of the user who modified the language.

- *Created on*   
  Date and time of the creation.

- *Created by*   
  Name and username of the user who created the language.

- ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add)   
  Click this button to create a language. The *Create language* view is displayed.   



## Create language

*DataHub > Settings > Tab LANGUAGES > Button Add*

![Create language](../../Assets/Screenshots/DataHub/Settings/Languages/CreateLanguage.png "[Create language]")

**Create language**

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *Create language* view and return to the language list. All changes are rejected.

- Language   
  Click the drop-down list and select the language in which the *Name (Language)* field is displayed. The system languages **English (United States)** and **Deutsch (Deutschland)** are available in the drop-down list.

- [SAVE]   
  Click this button to save the language. The *Create language* view is closed.

- *Name (Language)*   
  Enter a language name in the selected language.


- *Key*   
  Enter a language key. The key is required for API access and must be system wide unique. The language key must fulfill the criteria of the language codes according to [RFC 4646](https://www.heise.de/netze/rfc/rfcs/rfc4646.shtml). For instance, keys with the following structure are valid:
  - **en**
  - **en_US**
  - **en-US**

  > [Info] It is recommended to use the two-letter ISO 639-1 code for the language separated by a hyphen with the two-letter ISO 3166-1 code for the country, for instance en-US for English (United States), en-UK for English (United Kingdom) or de-DE for German (Germany).


- ![Toggle](../../Assets/Icons/Toggle.png "[Toggle]") *Active*   
  Enable this toggle to set the language status to active. Disable the toggle to set the language status to inactive. By default, this toggle is disabled.



## Edit language

*DataHub > Settings > Tab LANGUAGES > Select language*

![Edit language](../../Assets/Screenshots/DataHub/Settings/Languages/EditLanguage.png "[Edit language]")

**Edit language**

- ![Back](../../Assets/Icons/Back02.png "[Back]") (Back)   
  Click this button to close the *Edit Language* view and return to the language list. All changes are rejected.

- Language   
  Click the drop-down list and select the language in which the *Name (Language)* field is displayed. The system languages **English (United States)** and **Deutsch (Deutschland)** are available in the drop-down list.

- [SAVE]   
  Click this button to save the language. The *Edit language* view is closed.

- *Name (Language)*   
  Click the field to edit the language name in the selected language.


- *Key*   
  Click the field to edit the language key. It is not recommended to change the language key after creation.   
  The key is required for API access and must be system wide unique. The language key must fulfill the criteria of the language codes according to [RFC 4646](https://www.heise.de/netze/rfc/rfcs/rfc4646.shtml). For instance, keys with the following structure are valid:
  - **en**
  - **en_US**
  - **en-US**

  > [Info] It is recommended to use the two-letter ISO 639-1 code for the language separated by a hyphen with the two-letter ISO 3166-1 code for the country, for instance en-US for English (United States), en-UK for English (United Kingdom) or de-DE for German (Germany).


- ![Toggle](../../Assets/Icons/Toggle.png "[Toggle]") *Active*   
  Enable this toggle to set the language status to active. Disable the toggle to set the language to inactive. By default, this toggle is disabled.
