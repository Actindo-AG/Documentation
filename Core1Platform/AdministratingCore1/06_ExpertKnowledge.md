# Expert knowledge

This section contains procedures that you only should use, if you really know the consequences of your actions well.



## Switch on and switch off feature flags
The Entwicklermodus (Development mode) of the engine room allows to switch off and switch on again specific system behavior fundamentally. For example, this can be special caching functions, the event system, or the import of orders and other module-specific features. You can use this function for testing purposes or, for example, to temporarily switch off a connection, because you are informed about a downtime of the third-party application. Each action in the development mode is logged.

> [WARNING] Switching off features can lead to data loss. If you are not really sure about the consequences of switching off a feature, you should not use it. <!---Julian, stimmt das, oder arbeitet das System alles nach, wenn Funktion wieder eingeschaltet?-->

The development mode contains core features as well as engine-, module-, and driver-specific feature flags. For example, if you switch off the workflow, the following will happen:
- The workflow is stopped.
- All current processes do no longer import and 
output data. 
<!---Julian, gibt es noch ein anderes, drastisches Beispiel?-->

#### Prerequisites

- You have administrator rights for the current instance.
- You know the consequences of switching off a feature.

#### Procedure

*Actindo Core1 Platform > Any workspace*

![Core1 Platform](../../Assets/Screenshots/Core1Platform/Core1.png "[Core1 Platform]")


1. Click the ![Engine room](../../Assets/Icons/EngineRoom.png "[Engine roome]") (Engine room) button center top.  
The engine room is opened. The current workspace is overlapped.

   ![Engine room](../../Assets/Screenshots/Core1Platform/AdministratingCore1/Engineroom.png "[Engine room]")

2. Click the *Entwicklermodus (Development mode)* drop down top right.   
The list of feature flags is expanded. The list of filter chips with toggles contains general feature flags of the *Core1 Platform* as well as engine-, module-, and driver-specific feature flags.

   ![Feature flags](../../Assets/Screenshots/Core1Platform/AdministratingCore1/EngineRoomDevelopmentMode.png "[Feature flags]")

3. Switch off the required feature flag by disabling the corresponding filter chip toggle.   
The following warning message is displayed.

    ![Warning message](../../Assets/Screenshots/Core1Platform/AdministratingCore1/EngineRoomDevelopmentModeWarning.png "[Warning message]")
<!---Hallo Julian, ist die Meldung nicht ein bisschen schwach?-->
4. If desired, click the [OK] button.  
The processing of the related feature is stopped. The following notification is output.

   ![Feature flag notification](../../Assets/Screenshots/Core1Platform/AdministratingCore1/EngineroomFeatureFlagNotification.png "[Feature flag notification]")

5. Switch on the feature flag again by enabling the corresponding filter chip toggle later.   
The instance works as designed again. This action is logged as well.