# Engine room


## Open and close the engine room
Access to the engine room is available in any workspace you have opened in the *Core1 Plattform*.


#### Prerequisites

- You are assigned the ActindoAdminGroup.

#### Procedure
*Actindo Core1 Platform > Any workspace*

![Core1 Platform](../../Assets/Screenshots/Core1Platform/UsingCore1/Core1.png "[Core1 Platform]")


1. Click the ![Engine room](../../Assets/Icons/EngineRoom.png "[Engine roome]") (Engine room) button center top.  
The engine room is opened. The current workspace is overlapped.

   ![Engine room](../../Assets/Screenshots/Core1Platform/AdministratingCore1/Engineroom.png "[Engine room]")

2. Click the ![Engine room](../../Assets/Icons/EngineRoom.png "[Engine roome]") (Engine room) button again to close it.
The workspace is visible again.



## Clear tenant cache
Function to clear the cache of the current tenant/instance. This function removes all entries that are currently in the cache of the tenant. It is used if there is a general issue in processing and if changes are made directly through the database rather than through system logic. It is recommended to use this function only if it is really necessary. Clearing the cache will slow down the tenant considerably. 


#### Prerequisites

- You are assigned the ActindoAdminGroup.

#### Procedure
  
*Actindo Core1 Platform > Any workspace*

![Core1 Platform](../../Assets/Screenshots/Core1Platform/Core1.png "[Core1 Platform]")


1. Click the ![Engine room](../../Assets/Icons/EngineRoom.png "[Engine roome]") (Engine room) button center top.  
The engine room is opened. The current workspace is overlapped.

   ![Engine room](../../Assets/Screenshots/Core1Platform/AdministratingCore1/Engineroom.png "[Engine room]")

2. Click the [CLEAR TENANT CACHE] button.   
The following warning message is displayed:   
Clearing the tenant cache will slow down your account considerably. This action will be logged. Do you really want to continue? 

   ![Warning message](../../Assets/Screenshots/Core1Platform/AdministratingCore1/ClearCacheWarning.png "[Warning message]")

3. Click the [ABBRECHEN] (Cancel) button if you want to cancel the action. 

4. If desired, click the [FORTFAHREN] (Continue) button to clear the cache.   
The cache is cleared. It will be rebuilt again. The processes on the system are significantly slowed down.



## Check warnings and notices
The platform console provides tenant-relevant notices and warning. In opposite to the notifications (see [Check notifications](../UsingCore1/03_GeneralUIFunctions.md#check-notifications "Check notifications")), these notices and warnings are targeted for developers.


#### Procedure

*Actindo Core1 Platform > Any workspace*

![Core1 Platform](../../Assets/Screenshots/Core1Platform/Core1.png "[Core1 Platform]")


1. Click the ![Engine room](../../Assets/Icons/EngineRoom.png "[Engine roome]") (Engine room) button center top.  
The engine room is opened. The current workspace is overlapped.

   ![Engine room](../../Assets/Screenshots/Core1Platform/AdministratingCore1/Engineroom.png "[Engine room]")

2. Click the [PLATTFORM-KONSOLE] (Platform console) button.   
The *Platform Console* window is opened.

   ![Platform console](../../Assets/Screenshots/Core1Platform/AdministratingCore1/EngineroomPlatformConsole.png "[Platform console]")

3. Check the messages.



## Check vCores

The CPU core voltage (VCORE) is the power supply voltage supplied to the CPU (which is a digital circuit), GPU, or other device containing a processing core. The amount of power a CPU uses, and thus the amount of heat it dissipates, is the product of this voltage and the current it draws. In modern CPUs, which are CMOS circuits, the current is almost proportional to the clock speed, the CPU drawing almost no current between clock cycles (Source: Wikipedia). 

vCores (CPU core voltage) define the power of an instance for running parallel processes. Your company has bought a specific number of vCores for the main account, which are to be shared with the sandboxes. If a sandbox is created, a number of vCores are assigned from the main account, whereby this number reduces the number of vCores in the main account.   
Note, the vCores define the power for running parallel processes. They do not define the power for running a single process. Assigning more vCores will not speed up single processes!    
If an instance has not enough vCore capacity, the processor then starts to run the processes one after the other instead of running them in parallel. This means that the processing speed is slowed down significantly if the number of vCores assigned is unsufficiently.   
Actindo has an eye on the capacity utilization of your vCores. Isolated overruns will have no other effect than slowing down the speed or your processes. But if your vCore capacity is permanently over the limit, Actindo will contact you.   
The engine room allows you to monitor the required vCores of the current instance. With the vCore dashlet, you can monitor the needs for the last two hours.

<!---hallo Julian, gibt es auch eine Standard-Statistik über einen längeren Zeitraum?-->

#### Prerequisites

- You are assigned the ActindoAdminGroup.

#### Procedure

*Actindo Core1 Platform > Any workspace*

![Core1 Platform](../../Assets/Screenshots/Core1Platform/Core1.png "[Core1 Platform]")


1. Click the ![Engine room](../../Assets/Icons/EngineRoom.png "[Engine roome]") (Engine room) button center top.  
The engine room is opened. The current workspace is overlapped. It contains some dashlets with information on system health, etc.

   ![Engine room](../../Assets/Screenshots/Core1Platform/AdministratingCore1/Engineroom.png "[Engine room]")

3. Check the limit of vCores assigned to the current instance. To do this, move the mouse pointer on the white line.

   ![vCore dashlet](../../Assets/Screenshots/Core1Platform/AdministratingCore1/EngineRoomvCores.png "[vCore dashlet]")

4. Check the vCores for any deviations. If required, move the mouse on the peaks of the curve.