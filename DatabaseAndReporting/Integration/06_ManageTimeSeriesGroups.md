[!!User interface Time series groups](../UserInterface/01c_TimeSeriesGroups.md)

# Manage the time series groups

The time series databases can be organized in groups to execute them at certain time intervals or under specific scenarios. The time series databases assigned to a group are then executed sequentially, thereby reducing system load. Different groups running at the same time interval are executed in parallel.  

## Create a time series group

Create a time series group to group together any number of time series databases and determine the desired time interval to execute them.

#### Prerequisites  

No prerequisites to fulfill.

#### Procedure

*Database and reporting > Managed queries > Tab TIME SERIES GROUP*

![List of time series groups](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/TimeSeriesGroups/ListTimeSeriesGroups.png "[List of time series groups]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    The *Create time series group* view is displayed.

    ![Create time series group](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/TimeSeriesGroups/CreateTimeSeriesGroup.png "[Create time series group]")

2. Enter a descriptive name for the time series group in the *Title* field.

3. Enter a valid cron expression in the *CronLine* field to specify the time interval in which the time series databases included in the group are to be executed. If you need help creating a cron expression, you can check a cron expression editor, such as [Crontab guru](https://crontab.guru/).

4. Click the [SAVE] button in the upper right corner.  
    The *Submitting data...* view is displayed shortly while saving. The times series group has been saved. The *Create time series group* view is closed. The new times series group is displayed in the list of time series groups.  



## Edit a time series group

Once a time series group has been created, it can be edited to change any previously set values.

#### Prerequisites  

At least one time series group has been created, see [Create a time series group](#create-a-time-series-group).

#### Procedure

*Database and reporting > Managed queries > Tab TIME SERIES GROUPS*

![List of time series groups](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/TimeSeriesGroups/ListTimeSeriesGroups.png "[List of time series groups]")

1. Click the time series group to be edited in the list of time series groups. Alternatively, select the checkbox of the time series group to be edited and click the [EDIT] button in the editing toolbar.  
    The *Edit time series group* view is displayed.

    ![Edit time series group](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/TimeSeriesGroups/EditTimeSeriesGroup.png "[Edit time series group]")

2. Edit the time series group set values as necessary in the corresponding fields.

3. Click the [SAVE] button.   
    The *Submitting data...* view is displayed shortly while saving. The changes have been saved. The *Edit time series group* view is closed. The edited time series group is displayed in the list of time series groups. 



## Delete a time series group

A time series group can be deleted if it is no longer in use.

#### Prerequisites

At least one time series group has been created, see [Create a time series group](#create-a-time-series-group).

#### Procedure

*Database and reporting > Managed queries > Tab TIME SERIES GROUPS*

![List of time series groups](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/TimeSeriesGroups/ListTimeSeriesGroups.png "[List of time series groups]")

1. Select the checkbox of the time series group to be deleted.   
    The editing toolbar is displayed.

2. Click the [DELETE] button in the editing toolbar.  
    The deleted time series group is removed from the list of time series groups.

[comment]: <> (Julian: Hier kommt keine Bestätigung als Pop-Up Fenster vor, vgl. Time series DB. Wird es noch eingebaut?)