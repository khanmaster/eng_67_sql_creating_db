creating DB using Azure Studio

``` sql 
-- Create a new database called 'SHAHRUKH'
-- Connect to the 'master' database to run this snippet
USE Northwind
GO
-- Create the new database if it does not exist already
IF NOT EXISTS (
    SELECT [name]
        FROM sys.databases
        WHERE [name] = N'SHAHRUKH'
)
CREATE DATABASE SHNorthwind
```