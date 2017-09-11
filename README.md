# Cortex-Test

 Title: Cortex Test
 
 Description: This micro-service project is to build a flow which will collect and parse input data, persist the parsed data and present a report.
 
 Author: Nisha Fadadu

 Date: 9th Sept 2017


This micro-service project is developed in .Net Core using c# WEB API and SQL Server.


Follow the instruction to setup the project :

1. Unzip the Cortex_Test_Code.zip file

2. Find the Cortex_Test.sql file from unzipped folder and run the sql file on SQL server to setup the database.

3. Open the CortexTestMain folder solution in visual studio and run the service (Note: Run as a IIS Express)  (URL: http://localhost:24090/)

4. Open the CollectorService folder solution in visual studio and run the service  (Note: Run as a IIS Express)  (URL: http://localhost:61141/api/values/ReadFile)

5. Open the ParserService folder solution in visual studio and run the service  (Note: Run as a IIS Express) (URL: http://localhost:65183/api/values/ParsedData)

6. Open the PersisterService folder solution in visual studio and you need to change the databse connection string inside the /src/Models/DBHelper.cs class file in getDBConnection() method. After doing that you can run the service. (Note: Run as a IIS Express) (URL: http://localhost:3198/api/values) (POST method)

7. Open the ReporterServic folder solution in visual studio and you need to change the databse connection string inside the /src/Models/DBHelper.cs class file in getDBConnection() method. After doing that you can run the service.  (Note: Run as a IIS Express) (URL: http://localhost:16807/api/values/ReportSchema)

8. After sucessfully runing all 5 solutions go to http://localhost:24090/ which is CortexTestMain result window from where you can check all the 4 services result.

