# Azure Data Studio

1. Install Azure Data Studio from the [Link](https://docs.microsoft.com/en-us/sql/azure-data-studio/download-azure-data-studio?view=sql-server-ver15)

2. Install below extension in Azure Data Studio
   * `SQL Database Project`
   * `SQL Server Schema Compare`

3. Connect your Azure account from Azure Data Studio

4. Create connection to one Database and one Server placing them in different groups and providing user friendly names.

5. Create new project using SQL Database project extension.

6. Create new schema folder (dbo), another folder for Tables (Tables) and create a new table using below script.
    ```
    CREATE TABLE dbo.stores (
      store_id INT IDENTITY (1, 1),
      store_name VARCHAR (255) NOT NULL,
      phone VARCHAR (25),
      email VARCHAR (255),
      street VARCHAR (255),
      city VARCHAR (255),
      state VARCHAR (10),
      zip_code VARCHAR (5)
    );
    ```

7. Create a clustered index on store_id and a Non clusteded index on phone & email. 

8. Generate dummy data in above table.

9. Create a jupyter notebook with below scripts:
    * Script to get count of Indexes on each table
    * Script to get current fragmentation status
    * Script to optimize the indexes
    Include the instructions in the notebook to run optimization script only if fragmentation is >30%

10. Test your jupyter notebook on above database.

11. Customize dashboard for Server by adding below widget(s)
    * CPU utilization report by databases in table form
  
12. Customize dashboard for Database by adding below widget(s)
    * Top 10 expensive queries by CPU
    * Top 10 fragmented indexes

13. Create customized snippets:
    * Sample Get stored procedure for a table using Id as input
    * Sample Delete stored procedure for a table using Id as Input
    
14.     
