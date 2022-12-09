# Temporal_Tables

SQL Server Temporal Tables
The most requested feature for EF Core 6.0 was support for SQL Server temporal tables. As of RC1, temporal table support is now here!

SQL Server temporal tables automatically keep track of all the data ever stored in a table, even after that data has been updated or deleted. This is achieved by creating a parallel “history table” into which timestamped historical data is stored whenever a change is made to the main table. This allows historical data to be queried, such as for auditing, or restored, such as for recovery after accidental mutation or deletion.

EF Core 6.0 supports:

The creation of temporal tables using EF Core migrations
Transformation of existing tables into temporal tables, again using migrations
Querying historical data
Restoring data from some point in the past



https://devblogs.microsoft.com/dotnet/prime-your-flux-capacitor-sql-server-temporal-tables-in-ef-core-6-0/
