Steps to Install MySQL 8.x.xx ( Community Edition) on windows operating system
=========================================================

1. Go to mysql.com website
2. Select Downloads option
3. Select MySQL community Edition  (https://dev.mysql.com/downloads/)
4. Download MySQL community server 8.0.13 (https://dev.mysql.com/downloads/windows/installer/8.0.html)

While installing 

-> choose setup Type: custom  (Next)
-> + MySQL servers
		+ MySQL server 8
			+ MySQL server 8.0.13 (select)
	+ Applications
		+ MySQL workbench
			+ MySQL server 8.0.13 (select)

	Next
    -> Install other essential software required
							
										    Requirement
	select 	 	MySQL Server 8.0.13      Microsoft visual c++ 2015 Redistribution
	Select    	MySQL Workbench 8.0.13   Microsoft visual c++ 2015 Redistribution

	Next

-> Click Execute Button

-> Product Configuration
	Click Next

-> Group Replication 
	Select Standalone MySQL server / Classic MySQL replication

	Click Next

-> Type and Networking
	
	Config Type: Development Computer

	Connectivity:
	Check TCP/IP		PORT 3306 (Default)

	Click Next

-> Authentication Method

	Use strong password Encryption for Authentication (select)

	Click Next

-> Account And Roles
	
	MySQL root password : Enter password
	Repeat Password: reenter it

	Optional : You can add new user and set the roles here

	Click Next

-> Windows Service 

	check the box: start the MySQL server at system start
	Run Windows service as:

	standard system account

	Click Next

-> Execute it

- Open Workbench
- Create A connection as `imdb`
- open the COnnection and a Query Editor
- run below command to create a DataBase
- `create database imdb;`
- then use run below command,
- `use imdb;`
- then open the IMDB.sql file and copy the sql code and paste it in the Query editor and click on Thunder icon to execute the script.
The DataBase is ready to use.
