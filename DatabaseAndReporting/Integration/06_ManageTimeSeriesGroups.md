# Manage the time series groups

The time series databases can be organized in groups to execute them at certain intervals or under specific scenarios. The time series databases included in a group are then executed sequentially, thereby reducing system load. Different groups are executed in parallel.  

## Create a time series group



3. Enter a valid cron expression in the *Cronline* field to specify the time interval in which data is to be written to the time series database. If you need help creating  a cron expression, you can check a cron expression editor, such as [Crontab guru](https://crontab.guru/).

    > [Info] Note that each execution puts a certain amount of load on the database. Therefore, it is recommended to execute the query only as often as necessary. As a rule of thumb consider: The more complex the query, the less often the execution.


## Edit a time series group

## Delete a time series group

