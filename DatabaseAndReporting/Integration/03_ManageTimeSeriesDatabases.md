[!!Manage the queries](./01_ManageQueries.md)
[!!Manage the connection](./04_ManageConnections.md)
[!!Manage the time series group](./06_ManageTimeSeriesGroups.md)
[!!User interface Time series databases](../UserInterface/01b_TimeSeriesDatabases.md)

# Manage the time series databases

After a predefined query has been created to query data from your databases, the result can be written in a time series database like InfluxDB&trade;[^1], which allows you to collect and process a series of data points over time. For detailed information about InfluxDB&trade;, see the [InfluxDB&trade; website](https://influxdata.com/).

> [Info] We currently support the versions 1 and 2 of InfluxDB&trade;. We are not affiliated with, endorsed or sponsored by InfluxData or its affiliates in any way.

Once the data has been written to the time series database, it can be easily visualized and monitored using tools like Grafana&trade;[^2]. For detailed information, see the [Grafana&trade; website](https://grafana.com).

You can create, edit or delete a time series database for any predefined query.

## Create a time series database

Create a time series database for a specific predefined query.

#### Prerequisites

- A connection to a time series database has been established, see [Create a connection](./04_ManageConnections.md#create-a-connection). 
- At least one query has been created, see [Create a query](./01_ManageQueries.md#create-a-query). 
- At least one time series group has been created, see [Create a time series group](./06_ManageTimeSeriesGroups.md#create-a-time-series-group). 

#### Procedure

*Database and reporting > Managed queries > Tab TIME SERIES DATABASES*

![List of time series databases](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/TimeSeriesDatabases/ListTimeSeriesDatabases.png "[List of time series databases]")

We want to illustrate this with the example of measuring the number of orders placed in the last hour grouped by country. The corresponding query (simplified) would look like this:

SELECT count(*) AS `count`, `country` FROM `orders` WHERE `created` > NOW() - INTERVAL 1 HOUR GROUP BY `country`

1. Click the ![Add](../../Assets/Icons/Plus01.png "[Add]") (Add) button in the bottom right corner.   
    The *Create time series database* view is displayed.

    ![Create time series database](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/TimeSeriesDatabases/CreateTimeSeriesDatabase.png "[Create time series database]")

2. Enter a descriptive name for the time series database in the *Title* field.

    > [Info] This column has no logic behind it and offers a possibility to provide a sensible title for the measurement performed. In our example we could use "Number of orders in the last hour by country".

3. Click the *Group* drop-down list and select the applicable time series group. The group defines at which interval the data is measured. All available time series groups are displayed in the list. Note that every time series database must be assigned to a group to be executed at regular intervals. If you do not want the time series database to be executed at regular intervals within a group, select the **N/A** option. 

    > [Info] The time series group can be assigned while creating the time series database or later on, and can be edited anytime.

4. Enter the name for the measurement the data has to be written to in the *Measurement* field.  
If the measurement does not exist yet, it will be created automatically with the specified fields and tags. If the measurement already exists, the fields and tags of the existing table will be added to the specified measurement. 

   > [Info] In analogy to a relational database system, the measurement corresponds to a table. In our example we could name the measurement "NumberOfOrdersLastHourByCountry".
                                             
5. Click the *Connections* drop-down list and select the appropriate connection. All available connections are displayed in the list.

6. Click the *Queries* drop-down list and select the appropriate query. All available predefined queries are displayed in the list.

7. If desired, click the ![Add](../../Assets/Icons/Plus03.png "[Add]") (Add) button in the *Tag columns* box.  
    A new input line is displayed.

    > [Info] In analogy to a relation database system, the tag corresponds to an index column which is used in WHERE/GROUP BY statements. In our example a tag would contain the name of the country, as we want to measure the number of orders PER COUNTRY.

8. Enter the desired tag in the new input line. The name of a tag has to correspond to a result column of the selected query.

    > [Info] Repeat steps **7** and **8** to add further tags if necessary. 
     
9. Click the ![Add](../../Assets/Icons/Plus03.png "[Add]") (Add) button in the *Field columns* box.  
    A new input line is displayed.

    > [Info] The fields contain the actual data, that is, the values being measured (shown in the Y-axis). In our example the field would be the number of orders, as we want to measure the NUMBER OF ORDERS per country.

10. Enter the desired field in the new input line.    

    > [Info] Repeat steps **9** and **10** to add further fields if necessary.

11. Click the [SAVE] button in the upper right corner.  
    The *Submitting data...* view is displayed shortly while saving. The times series database has been saved. The *Create time series database* view is closed. The new times series database is displayed in the list of time series databases. 



## Edit a time series database

Once a time series database has been created, it can be edited to change any previously set values.

#### Prerequisites

At least one time series database has been created, see [Create a time series database](#create-a-time-series-database).

#### Procedure

*Database and reporting > Managed queries > Tab TIME SERIES DATABASE*

![List of time series databases](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/TimeSeriesDatabases/ListTimeSeriesDatabases.png "[List of time series databases]")

1. Click the time series database to be edited in the list of time series databases. Alternatively, select the checkbox of the time series database to be edited and click the [EDIT] button in the editing toolbar.  
    The *Edit time series database* view is displayed.

    ![Edit time series database](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/TimeSeriesDatabases/EditTimeSeriesDatabase.png "[Edit time series database]")

2. Edit the time series database set values as necessary in the corresponding fields.

3. Click the [SAVE] button.   
    The *Submitting data...* view is displayed shortly while saving. The changes have been saved. The *Edit time series database* view is closed. The edited time series database is displayed in the list of time series databases. 



## Delete a time series database 

A time series database can be deleted if it is no longer in use.

#### Prerequisites

At least one time series database has been created, see [Create a time series database](#create-a-time-series-database).

#### Procedure

*Database and reporting > Managed queries > Tab TIME SERIES DATABASES*

![List of time series databases](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/TimeSeriesDatabases/ListTimeSeriesDatabases.png "[List of time series databases]")

1. Select the checkbox of the time series database to be deleted.   
    The editing toolbar is displayed.

2. Click the [DELETE] button in the editing toolbar.  
    The *Time series has been deleted* pop-up window is displayed. The deleted time series database is removed from the list of time series databases.

    ![Deleted time series database](../../Assets/Screenshots/DatabaseAndReporting/ManagedQueries/TimeSeriesDatabases/TimeSeriesDeleted.png "[Deleted time series database]")

[^1]: **Disclaimer:** InfluxDB&trade; is a trademark owned by InfluxData, which is not affiliated with, and does not endorse, this site.  

[^2]: **Disclaimer:** The Grafana Labs Marks are trademarks of Grafana Labs, and are used with Grafana Labs’ permission. We are not affiliated with, endorsed or sponsored by Grafana Labs or its affiliates.