# Engine room

The engine room contains some dashlets with information on vCore utilization, database storage utilization, request and error statistics, and jobs currently running.



## Open and close the engine room

Access to the engine room is available in any workspace you have opened in the *Core1 Platform*.

#### Prerequisites

You have administrator rights for the current instance.

#### Procedure

*Actindo Core1 Platform > Any workspace*
 
   ![Core1 Platform](../../Assets/Screenshots/Core1Platform/Core1.png "[Core1 Platform]")

1. Click the ![Engine room](../../Assets/Icons/EngineRoom.png "[Engine roome]") (Engine room) button in the upper center of the workplace.  
   The engine room is opened with the current workspace overlapped. It contains four dashlets.

   ![Engine room](../../Assets/Screenshots/Core1Platform/AdministratingCore1/Engineroom.png "[Engine room]")

2. Click the ![Engine room](../../Assets/Icons/EngineRoom.png "[Engine room]") (Engine room) button again to close it.
   The workspace is visible again.



## Clear tenant cache

Clearing the tenant cache removes all entries that are currently in the cache of the instance. It is used if there is a general issue in processing, and if changes are made directly through the database rather than through system logic.   
It is recommended to use this function only if it is really necessary. Clearing the cache will slow down the instance considerably. 

#### Prerequisites

You have administrator rights for the current instance.

#### Procedure
  
*Actindo Core1 Platform > Any workspace*

![Core1 Platform](../../Assets/Screenshots/Core1Platform/Core1.png "[Core1 Platform]")


1. Click the ![Engine room](../../Assets/Icons/EngineRoom.png "[Engine roome]") (Engine room) button in the upper center of the workplace of the workspace.  
   The engine room is opened. The current workspace is overlapped.

   ![Engine room](../../Assets/Screenshots/Core1Platform/AdministratingCore1/Engineroom.png "[Engine room]")

2. Click the [CLEAR TENANT CACHE] button in the upper right corner.   
   The following warning message is displayed:   

   ![Warning message](../../Assets/Screenshots/Core1Platform/AdministratingCore1/ClearCacheWarning.png "[Warning message]")

3. Click the [CANCEL] button if you want to cancel the action. 

4. If desired, click the [CONTINUE] button to clear the cache.   
   The cache is cleared. Afterwards, it will be rebuilt again. The processes on the instance are significantly slowed down.



## Check warnings and notices

The platform console provides instance-relevant notices and warnings. In contrast to the notifications (see [Check notifications](../UsingCore1/04_GeneralUIFunctions.md#check-notifications)), these notices and warnings are intended for developers.

#### Prerequisites

You have administrator rights for the current instance.

#### Procedure

*Actindo Core1 Platform > Any workspace*

![Core1 Platform](../../Assets/Screenshots/Core1Platform/Core1.png "[Core1 Platform]")


1. Click the ![Engine room](../../Assets/Icons/EngineRoom.png "[Engine roome]") (Engine room) button in the upper center of the workplace.  
   The engine room is opened. The current workspace is overlapped.

   ![Engine room](../../Assets/Screenshots/Core1Platform/AdministratingCore1/Engineroom.png "[Engine room]")

2. Click the [Platform console] button.   
   The *Platform console* window is opened.

   ![Platform console](../../Assets/Screenshots/Core1Platform/AdministratingCore1/EngineroomPlatformConsole.png "[Platform console]")

3. Check the messages.



## Check vCores

Your company has purchased a certain number of vCores assigned to the main account. vCores define the computing power of an instance for the execution of parallel processes as well as database queries. It does not include idle times such as calls that are waiting for a response from external service providers.      
If an instance has not enough vCore capacity, the processor then starts to run the processes and database queries one after the other instead of running them in parallel. 
This means that if the number of vCores assigned is not sufficient, the processing speed is slowed down significantly.  

> [Info] The vCores define the power for running parallel processes. They do not define the power for running a single process. Assigning more vCores will not speed up single processes!    

If a sandbox is created, it is assigned a number of vCores from the main account. This reduces the number of vCores available for the main account.   
Note that the transfer of vCores from the main account to a sandbox may take some time (about 5 minutes).   

The engine room allows you to monitor the required vCores of the current instance. With the vCore dashlet, you can monitor the needs of the last two hours.  
The vCores are analyzed as average over several seconds. The dashlet displays the totals per every 30 seconds in a curve diagram. 

 > [Info] Since *Actindo* displays an average value every 30 seconds, it may happen that the limit is exceeded for a brief time but is not displayed in the dashlet. This leads to a temporary slowdown of the processing speed.


#### Prerequisites

You have administrator rights for the current instance.

#### Procedure

*Actindo Core1 Platform > Any workspace*

![Core1 Platform](../../Assets/Screenshots/Core1Platform/Core1.png "[Core1 Platform]")

1. Click the ![Engine room](../../Assets/Icons/EngineRoom.png "[Engine roome]") (Engine room) button in the upper center of the workplace.  
   The engine room is opened. The current workspace is overlapped. 

   ![Engine room](../../Assets/Screenshots/Core1Platform/AdministratingCore1/Engineroom.png "[Engine room]")

2. Focus your attention to the dashlet at the first position from the left.  
   The vCore utilization is displayed in a curve diagram.

3. Check the limit of vCores assigned to the current instance. To do this, move the mouse pointer over the white line.   
   The limit of vCores for this instance is displayed in a callout.   
     
   ![vCore dashlet](../../Assets/Screenshots/Core1Platform/AdministratingCore1/EngineRoomvCores.png "[vCore dashlet]")

4. Check the vCores for any deviations. If desired, move the mouse on a peak of the curve.   
   The number of vCores is displayed in a callout shape. Used vCores are shown in green, required vCores above the limit for a given time are shown in red.

    ![Number of vCores](../../Assets/Screenshots/Core1Platform/AdministratingCore1/EngineRoomvCoresCurve.png "[Number of vCores]")



## Check database utilization

Your company has purchased a certain amount of data storage space assigned to the main account. If a sandbox is created, it is assigned an amount of storage space from the main account. This reduces the number of storage space available on the main account.   

Actindo has an eye on your data storage utilization. Isolated overruns will have no effect. But if your data storage utilization is permanently over the limit, *Actindo* will contact you.   

#### Prerequisites

You have administrator rights for the current instance.

#### Procedure

*Actindo Core1 Platform > Any workspace*

![Core1 Platform](../../Assets/Screenshots/Core1Platform/Core1.png "[Core1 Platform]")


1. Click the ![Engine room](../../Assets/Icons/EngineRoom.png "[Engine roome]") (Engine room) button in the upper center of the workplace.  
   The engine room is opened. The current workspace is overlapped. 

    ![Engine room](../../Assets/Screenshots/Core1Platform/AdministratingCore1/Engineroom.png "[Engine room]")

2. Focus your attention to the dashlet at the second position from the left.  
   The data storage utilization is displayed in a circle diagram.
   In the middle of the circle, the current utilization is displayed in percent as well as in gigabyte.

    ![Data storage](../../Assets/Screenshots/Core1Platform/AdministratingCore1/EngineroomDataStorage.png "[Data storage]")

   >[Info] Note that these figures are evaluated once a day.   

3. If desired, refresh the current dashlet by clicking the [REFRESH] button to get the current figures.

4. Move your mouse pointer over the circle diagram.   
   The current data storage utilization is displayed in a callout shape.
    


## Check request statistics

 The request statistics dashlet displays what is going on the current instance. It shows the number of internal requests (jobs) and requests executed from a browser. Additionally, it shows the number of errors occurred during the request processing.   
 The statistic is evaluated per each hour.
 

#### Prerequisites

You have administrator rights for the current instance.

#### Procedure

*Actindo Core1 Platform > Any workspace*

![Core1 Platform](../../Assets/Screenshots/Core1Platform/Core1.png "[Core1 Platform]")

1. Click the ![Engine room](../../Assets/Icons/EngineRoom.png "[Engine roome]") (Engine room) button in the upper center of the workplace.  
   The engine room is opened. The current workspace is overlapped. 

   ![Engine room](../../Assets/Screenshots/Core1Platform/AdministratingCore1/Engineroom.png "[Engine room]")

3. Focus your attention to the dashlet at the third position from the left.  
   The diagram has two y-axes. The left y-axis defines the number of requests, the right one defines the number of errors.   
   The x-axis defines the time from midnight to the current time in UTC. Depending on the time passed since midnight, the figures are displayed per hour or per every second/third hour.  
   The number of requests is presented in a green curve diagram, the number of errors is presented in a red line diagram.

    ![Request statistics](../../Assets/Screenshots/Core1Platform/AdministratingCore1/EngineRoomRequestStatistic.png "[Request statisics]")

4. Move your mouse pointer over the top of green curve diagram.   
   The number of requests is displayed in a callout shape. 

    ![Request per hour](../../Assets/Screenshots/Core1Platform/AdministratingCore1/EngineRoomRequests.png "[Requests per hour]")

5. Move your mouse pointer over the red line diagram.   
   The number of errors is displayed in a callout.

   ![Errors per hour](../../Assets/Screenshots/Core1Platform/AdministratingCore1/EngineRoomErrors.png "[Errors per hour]")


## View current jobs

The Job dashlet displays all asynchronous jobs that are currently running.

#### Prerequisites

You have administrator rights for the current instance.

#### Procedure

*Actindo Core1 Platform > Any workspace*

![Core1 Platform](../../Assets/Screenshots/Core1Platform/Core1.png "[Core1 Platform]")

1. Click the ![Engine room](../../Assets/Icons/EngineRoom.png "[Engine roome]") (Engine room) button in the upper center of the workplace of the workplace.  
   The engine room is opened. The current workspace is overlapped. 

   ![Engine room](../../Assets/Screenshots/Core1Platform/AdministratingCore1/Engineroom.png "[Engine room]")

2. Focus your attention to the dashlet at the fourth position from the left.

3. Click the *JOBS* tab.   
   The currently running asynchronous jobs as well as the jobs waiting are displayed. On top, the number of jobs is output as well as the percentage ratio of finished jobs. If no jobs are running, the *No running jobs* message is displayed.

   ![Current jobs](../../Assets/Screenshots/Core1Platform/AdministratingCore1/EngineRoomJobs.png "[Current jobs]")

<!--- Beim Drücken von Cron jobs passiert nichts, darum besser weggelassen-->