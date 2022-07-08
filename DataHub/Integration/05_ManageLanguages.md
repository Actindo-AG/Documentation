[!!DataHub](DataHub)

# Manage the languages

The different languages are needed to be able to maintain attributes in different languages. By default, the languages *English (United States)* and *German (Germany)* are preset. If you want to maintain further languages, you have to create and activate the respective languages. You can create an unlimited number of languages.

## Create a language

Create a language to maintain attributes in the desired language.

#### Prerequisites

No prerequisites to fulfill.

#### Procedure
*DataHub > Settings > Tab LANGUAGES*

![Language list](/Assets/Screenshots/DataHub/Settings/Languages/LanguageList.png "[Language list]")

1. Click the ![Add](/Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
  The *Create language* view is displayed.

  ![Create language](/Assets/Screenshots/DataHub/Settings/Languages/CreateLanguage.png "[Create language]")

2. Enter a name for the language in the *Name* field.

3. Enter a key for the language in the *Key* field. The key is required for API access and must be system wide unique.

4. Enable the *Active* toggle to set the language directly after creation to active.

  > [Info] The language must be activated to be used.

5. Click the [SAVE] button in the upper right corner.   
  The new language is saved. The *Create language* view is closed.  



## Edit a language

After you have created a language, you can edit its name or key.

#### Prerequisites

At least one language is created, see [Create a language](/DataHub/Integration/CreateLanguage.md).

> [Info] By default, the languages *English (United States)* and *German (Germany)* are created.

#### Procedure
*DataHub > Settings > Tab LANGUAGES*

![Language list](/Assets/Screenshots/DataHub/Settings/Languages/LanguageList.png "[Language list]")

1. Click the language you want to edit in the list of languages.   
  The *Edit language* view is displayed.

  ![Edit language](/Assets/Screenshots/DataHub/Settings/Languages/EditLanguage.png "[Edit language]")

2. Edit the desired data of the language in the corresponding fields.

3. Click the [SAVE] button in the upper right corner.   
  The changes are saved. The *Edit language* view is closed.  



## Deactivate a language

Deactivate a language when it should not be used for a certain time. The language is no longer available when it is inactive. Further, it is recommended to deactivate a language instead of deleting it to prevent any problems because of existing dependencies.

#### Prerequisites

At least one language is created, see [Create a language](#create-a-language).

> [Info] By default, the languages *English (United States)* and *German (Germany)* are created.

#### Procedure
*DataHub > Settings > Tab LANGUAGES*

![Language list](/Assets/Screenshots/DataHub/Settings/Languages/LanguageList.png "[Language list]")

1. Click the language you want to edit in the list of languages.   
  The *Edit language* view is displayed.

  ![Edit language](/Assets/Screenshots/DataHub/Settings/Languages/EditLanguage.png "[Edit language]")

2. Disable the *Active* toggle.

3. Click the [SAVE] button in the upper right corner.   
  The language is deactivated. The *Edit language* view is closed.



## Delete a language

You can delete a language if it is no longer needed. As there are usually existing dependencies, it is highly recommended not to delete a language. Instead, you can deactivate a language and thus prevent its use.

#### Prerequisites

At least one language is created, see [Create a language](#create-a-language).

> [Info] By default, the languages *English (United States)* and *German (Germany)* are created. Both languages cannot be deleted.

#### Procedure
*DataHub > Settings > Tab LANGUAGES*

![Language list](/Assets/Screenshots/DataHub/Settings/Languages/LanguageList.png "[Language list]")

1. Select the checkbox of the language you want to delete in the list of languages.    
  The editing toolbar is displayed above the language list.

2. Click the [Delete] button in the toolbar.  
  The language is deleted. The deletion cannot be undone.

  > [Info] If the selected language cannot be deleted, an error message is displayed in the upper right corner. To prevent the languages use, it is recommended to [deactivate the language](#deactivate-a-language) instead of delete it.



## Related content

- [User Interface DataHub](/DataHub/UserInterface/02f_Languages.md)
- [Configure the language settings](/PIM/Integration/ConfigureLanguages.md)
