[!!Manage InfluxDB time series](./01b_InfluxDBTimeSeries.md)

#  InfluxDB time series

*Database and reporting > Managed queries > Tab INFLUXDB TIME SERIES*

![List InfluxDB time series](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/InfluxDBTimeSeries/ListInfluxDBTimeSeries.png "[List InfluxDB time series]")

**List of InfluxDB time series**

- *Title*  
    Description of the InfluxDB time series.

- *CronLine*  
    Cron expression used to specify the time interval in which the InfluxDB time series must be executed.

- *Connection*  
    InfluxDB connection selected to write data in InfluxDB.

- *Query*  
    Predefined query to be executed in the InfluxDB time series.

- *Measurement*  
    Name of the table where the data is to be written.

- *Tags*  
    Tags specified to categorize the data written to InfluxDB. Tags are optional and therefore this column may be empty.

- *Fields*  
    Fields (values) specified to be written to InfluxDB. Fields are mandatory. 

- *ID*  
    InfluxDB time series identification number. The ID number is automatically assigned by the system.

- [EXECUTE]  
    Click this button to execute the InfluxDB time series immediately, that is, without waiting for the next scheduled run. This button is only displayed if a single checkbox in the list of InfluxDB time series is selected.

- [EDIT]  
    Click this button to edit a selected InfluxDB time series. This button is only displayed if a single checkbox in the list of InfluxDB time series is selected.

- [DELETE]  
    Click this button to delete a selected InfluxDB time series. It is possible to delete several queries at once. This button is displayed if at least one checkbox in the list of queries is selected.

[comment]: <> (Julian: Ich gehe davon aus, dass es so stimmt. Bitte bestätigen.)


## Create an InfluxDB time series

*Database and reporting > Managed queries > Tab INFLUXDB TIME SERIES*

![Create InfluxDB time series](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/InfluxDBTimeSeries/CreateInfluxDBTimeSeries.png "[Create InfluxDB time series]")

- *Title*  
    Enter a description for the InfluxDB time series.

- *CronLine*  
    Enter a valid cron expression to specify the time interval in which the InfluxDB time series must be executed.

- *Measurement*  
    Enter the name of the table where the data is to be written. 
    
    > [Info] If the measurement does not exist yet, it will be created automatically with the specified fields and tags. If the measurement already exists, the fields and tags of the existing table will be added to the specified measurement.

- *Connections*  
    Click the drop-down list and select the desired connection. The available connections are displayed in the list.  

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)  
    Click this button to refresh the *Connections* drop-down list to display any newly created connection.

- *Queries*  
    Click the drop-down list and select the desired predefined query.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)  
    Click this button to refresh the *Queries* drop-down list to display any newly created query.

- *Tag columns*  
    Enter the relevant tag(s) in this box to categorize the data to be written to InfluxDB according to you desired criteria. Tags represent metadata and are therefore optional.

- ![Add](../../Assets/Icons/Plus03.png "[Add]") (Add)  
    Click this button to add a new input line to the *Tag columns* box.

- ![Delete](../../Assets/Icons/Trash01.png "[Delete]") (Delete)  
    Click this button to remove a tag from the *Tag columns* box. This button is displayed to the right of a newly added input line.
    
- *Field columns*  
    Enter the relevant field(s) in this box to define the data to be written to InfluxDB. Fields represent the actual values and are therefore mandatory.

- ![Add](../../Assets/Icons/Plus03.png "[Add]") (Add)  
    Click this button to add a new input line to the *Field columns* box.

- ![Delete](../../Assets/Icons/Trash01.png "[Delete]") (Delete)  
    Click this button to remove a field from the *Field columns* box. This button is displayed to the right of a newly added input line.
- [SAVE]  
    Click this button to save the InfluxDB time series. The *Create InfluxDB time series* view is closed. The new InfluxDB time series is displayed in the list of InfluxDB time series.

## Edit an InfluxDB time series

*Database and reporting > Managed queries > Tab INFLUXDB TIME SERIES*

![Edit InfluxDB time series](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/InfluxDBTimeSeries/EditInfluxDBTimeSeries.png "[Edit InfluxDB time series]")

- *Title*  
    Edit the description for the InfluxDB time series.

- *CronLine*  
    Edit the cron expression to specify the time interval in which the InfluxDB time series must be executed.

- *Measurement*  
    Edit the name of the table where the data is to be written. 

- *Connections*  
    Click the drop-down list and select the appropriate connection. The available connections are displayed in the list.  

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)  
    Click this button to refresh the *Connections* drop-down list to display any newly created connection.
    
- *Queries*  
    Click the drop-down list and select the desired predefined query.

- ![Refresh](../../Assets/Icons/Refresh01.png "[Refresh]") (Refresh)  
    Click this button to refresh the *Queries* drop-down list to display any newly created query.
  
- *Tag columns*  
    Edit the tag(s) in this box to categorize the data to be written to InfluxDB according to you desired criteria. Tags represent metadata and are therefore optional.

- ![Add](../../Assets/Icons/Plus03.png "[Add]") (Add)  
    Click this button to add a new input line to the *Tag columns* box.

- ![Delete](../../Assets/Icons/Trash01.png "[Delete]") (Delete)  
    Click this button to remove a tag from the *Tag columns* box. This button is displayed to the right of a newly added input line.
    
- *Field columns*  
    Edit the field(s) in this box to define the data to be written to the InfluxDB. Fields represent the actual values and are therefore mandatory.

- ![Add](../../Assets/Icons/Plus03.png "[Add]") (Add)  
    Click this button to add a new input line to the *Field columns* box.

- ![Delete](../../Assets/Icons/Trash01.png "[Delete]") (Delete)  
    Click this button to remove a field from the *Field columns* box. This button is displayed to the right of a newly added input line.

- [SAVE]  
    Click this button to save any changes made. The *Edit InfluxDB time series* view is closed. All changes have been applied.