# Project Log

![](/images/raw.png)
* Prepared data
* See [ssis_data_preparation_project_0](https://github.com/timamero/ssis_data_preparation_project_0) for example 
* Loaded data to the OFFICESUPPLIES database in SQL Server
<br/>
<br/>
![](/images/wrk.png)
* Created the stored procedures to create and update WRK_CustomerList and WRK_TransactionalData tables
<br/>
<br/>
![](/images/wrktables.png)
* The Customer ID columns in WRK_CustomerList and WRK_TransactionalData need to match.  Will update the stored procedure in WRK_CustomerList to add the leading zeros in CustomerID.
<br/>
<br/>
* Created template to create future stored procedures: __tmpl__BLD_WRK_TableName
<br/>
<br/>
* Archived previous version of stored prodcures: zzz_bckp_20200313_BLD_WRK_TransactionalData
* Started file name with 'zzz' so that file is displayed at bottom of list
* Note that there are different ways to archive stored procedures
<br/>
<br/>
![](/images/drv.png)
* Created stored procedure to create and update DRV table
* The DRV table created will prepare the data to allow the user to compare purchases between genders.  Must combine data from the tables WRK_CustomerList and WRK_TransactionalData
<br/>
<br/>
![](/images/final.png)
* Final tables and stored procedures