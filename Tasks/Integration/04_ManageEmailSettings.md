[!!User interface Email settings](../UserInterface/to-be-determined)

# Manage the email settings

The *E-MAIL SETTINGS* tab allows you configure how a user is notified per email when a task is created. 

This tab is only displayed if the *Email* (1.6.1) module is installed.



## Create a connection in the *Email* module

*Email > Settings > Connections*

![Email connections](../../Assets/Screenshots/Tasks/Settings/EmailSettings/EmailConnections.png "[Email connections]")



## Create an email type in the email connection

*Email > Settings > Connections > Select a connection > Email types*

![Email types](../../Assets/Screenshots/Tasks/Settings/EmailSettings/EmailTypes.png "[Email types]")



## Configure the general settings

In this menu option, you can configure the email type that is used to send email notifications, and the email address from which the email notification is sent.

#### Prerequisites

- The *Task Tracker Email Connection* 1.1.0 plugin is installed.
- At least one connection has been established in the *Email* module.
- At least one email type has been defined in the email connection.

[comment]: <> (Stimmt das so? Wo erstellt man die Email-Adresse fürs Feld "From"?)

#### Procedure

*Tasks > Settings > Tab E-MAIL SETTINGS*

![Email general settings](../../Assets/Screenshots/Tasks/Settings/EmailSettings/EmailSettingsGeneral.png "[Email general settings]")

1. Click the *Email type* drop-down list in the *General settings* menu option and select the desired option. All available email types are .

2. Click the *From* field and enter the desired email address, such as in the following example.

    ![General settings example](../../Assets/Screenshots/Tasks/Settings/EmailSettings/EmailSettingsGeneralExample.png "[General settings example]")

[comment]: <> (Wo wird diese Email-Adresse erstellt?)

3. If necessary, click the *Email sending per event* menu option to configure further settings, see [Configure the email sending per event](#configure-the-email-sending-per-event). Otherwise, go to step 4.

4. Click the [SAVE] button.  
    A confirmation message is displayed. The email general settings have been saved.



## Configure the email sending per event

In this menu option, you can enable or disable email notification per event. By default, email notification is enabled for all events.

#### Prerequisites

The general settings have been configured, see [Configure the general settings](#configure-the-general-settings).

#### Procedure

*Tasks > Settings > Tab E-MAIL SETTINGS > Email sending per event*

![Email sending per event](../../Assets/Screenshots/Tasks/Settings/EmailSettings/EmailSettingsSending.png "[Email sending per event]")

1. Disable the *Apply from default* toggle to be able to modify the predefined email sending per event settings.  
    The email sending per event settings are unlocked.

2. Disable or enable the desired event toggle to deactivate or activate email notification when a event occurs.

3. Click the [SAVE] button.  
    A confirmation message is displayed. The email sending settings have been saved.
