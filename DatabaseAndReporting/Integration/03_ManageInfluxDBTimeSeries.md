[!!User interface InfluxDB time series](../UserInterface/01b_InfluxDBTimeSeries.md)
[!!Manage the connection](./04_ManageConnections.md)
[!!Manage the queries](./01_ManageQueries.md)

# Manage the InfluxDB time series

An InfluxDB time series is a sequence of data points collected in time intervals, allowing to track changes over time. Once a a MySQL query has been created to extract any required data, this data can be written to an InfluxDB to be collected and processed over a period of time. For detailed information about InfluxDB, see [InfluxDB](https://docs.influxdata.com/influxdb/v2.6/).

Besides, once the data has been written to InfluxDB, it can be easily visualize using Grafana, see [Get started with Grafana and InfluxDB](https://grafana.com/docs/grafana/latest/getting-started/get-started-grafana-influxdb/).

You can create, edit or delete an InfluxDB time series for any predefined query.


## Create an InfluxDB time series

Create an InfluxDB time series for a specific predefined query.

#### Prerequisites

- The applicable connection to the InfluxDB time series software has been established, see [Create a connection](../Integration/04_ManageConnections.md#create-a-connection). 
- The relevant predefined query have been created, see [Create a query](./01_ManageQueries.md#create-a-query). 

#### Procedure

*Database and reporting > Managed queries > Tab INFLUXDB TIME SERIES*

![List of InfluxDB time series](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/InfluxDBTimeSeries/ListInfluxDBTimeSeries.png "[List of InfluxDB time series]")

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    The *Create InfluxDB time series* view is displayed.

    ![Create InfluxDB time series](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/InfluxDBTimeSeries/CreateInfluxDBTimeSeries.png "[Create InfluxDB time series]")

2. Enter a description for the InfluxDB time series in the *Title* field.

3. Enter a valid cron expression in the *Cronline* field to specify the time interval in which data are to be written to the InfluxDB. If you need help creating  a cron expression, you can check a cron expression editor, such as [Crontab guru](https://crontab.guru/).
    > [Info] Note that each execution puts a certain amount of load on the database. Therefore, it is recommended to execute the query only as often as necessary. As a rule of thumb consider: The more complex the query, the less often the execution.

4. Enter a description for the table where the data is to be written in the *Measurement* field. 
    > [Info]  If the measurement does not exist yet, it will be created automatically with the specified fields and tags. If the measurement already exists, the fields and tags of the existing table will be added to the specified measurement. 

5. Click the drop-down list and select the appropriate connection.  
    All available connections established in the *CONNECTIONS* tab of the *Settings* menu entry are displayed in the list.

6. Click the drop-down list and select the appropriate query.   
    All available queries specified in the *QUERIES* tab are displayed in the list.

7. If desired, click the ![Add](../../Assets/Icons/Plus03.png "[Add]") (Add) button in the *Tag columns* box.  
    A new input line is displayed.

8. Enter the desired tag in the new input line.   
    If desired, repeat steps **7** and **8** to add further tags. 

9. Click the ![Add](../../Assets/Icons/Plus03.png "[Add]") (Add) button in the *Field columns* box.  
    A new input line is displayed.

    > [Info] The fields contain the actual data, that is the values being measured. The tags, on the other hand, can be used for metadata, that is, to categorize the data. This means that at least one field needs to be specified, whereas tags are optional.

10. Enter the desired field in the new input line.    
    If desired, repeat steps **9** and **10** to add further fields.

11. Click the [SAVE] button in the upper right corner.  
    The *Submitting data...* view is displayed shortly while saving. 

    ![Submitting data](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/InfluxDBTimeSeries/SubmittingData.png "[Submitting data]")

    [comment]: <> (Screenshot aus NoE test account. OK?)

    The InfluxDB times series has been saved. The *Create InfluxDB time series* view is closed. The new InfluxDB times series is displayed in the list of InfluxDB time series. 


## Edit an InfluxDB time series

Once an InfluxDB time series has been created, you can edit it.

#### Prerequisites

At least one InfluxDB time series has been created, see [Create an InfluxDB time series](#create-an-influxdb-time-series).

#### Procedure

*Database and reporting > Managed queries > Tab INFLUXDB TIME SERIES*

![List of InfluxDB time series](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/InfluxDBTimeSeries/ListInfluxDBTimeSeriesCreated.png "[List of InfluxDB time series]")

1. Click the InfluxDB time series to be edited in the list of InfluxDB time series. Alternatively, select the checkbox of the InfluxDB time series to be edited and click the ![Edit](../../Assets/Icons/Edit01.png) (Edit) button in the editing toolbar.  
    The *Edit InfluxDB time series* is displayed.

    ![Edit InfluxDB time series](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/InfluxDBTimeSeries/EditInfluxDBTimeSeries.png "[Edit InfluxDB time series]")

[comment]: <> (Keine Beispiele noch in JS account. Bei NoE button heißt EDIT. Standard oder Kd-spezifisch?)

2. Modify the InfluxDB time series set values as necessary.

3. Click the [SAVE] button.   
    The *Submitting data...* view is displayed shortly while saving. 

    ![Submitting data](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/InfluxDBTimeSeries/SubmittingData.png "[Submitting data]")

    [comment]: <> (Screenshot aus NoE test account. OK?)

    The changes have been saved. The *Edit InfluxDB time series* view is closed. The modified InfluxDB times series is displayed in the list of InfluxDB time series. 


## Delete an InfluxDB time series 

An InfluxDB time series can be deleted if it no longer in use.

#### Prerequisites

At least one InfluxDB time series has been created, see [Create an InfluxDB time series](#create-an-influxdb-time-series).

#### Procedure

*Database and reporting > Managed queries > Tab INFLUXDB TIME SERIES*

![List of InfluxDB time series](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/InfluxDBTimeSeries/ListInfluxDBTimeSeriesCreated.png "[List of InfluxDB time series]")


1. Click the InfluxDB time series to be deleted in the list of InfluxDB time series. Alternatively, select the checkbox of the InfluxDB time series to be deleted and click the ![Delete](../../Assets/Icons/Trash03.png) (Delete) button in the editing toolbar.  
    The *Deleted InfluxDB time series xxxx* window is displayed. The number indicates the identifier of the deleted InfluxDB time series as displayed in the *ID* column. The deleted InfluxDB time series is removed from the list of InfluxDB time series. 

[comment]: <> (Nicht getestet. Text aus Queries. Prüfen, ob Löschprozedur gleich! Keine Beispiele noch in JS account. Bei NoE button heißt DELETE. Standard oder Kd-spezifisch?)



[comment]: <> (Bei NoE, EXECUTE button in Editing toolbar. Bedeutung? Standard?)