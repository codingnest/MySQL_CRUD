Problem Statement:

1. Download MYSQL Server and Client from https://dev.mysql.com/downloads/installer/
2. Install Mysql Server and Client
3. Create a Config File using ConfigParser Module.

connection.ini

[Mysql]

HOSTNAME=localhost

USERNAME=root

PASSWORD=****

PORT=3306

DATABASE=db1

4. Create a Connection Object Module by reading details from connection.ini
5. Write all SQL Queries on a file and save with queries.xml

<?xml version="1.0"?>

<queries>

<query id="drop">drop table if exists persons;</query>

<query id="persons">create table persons(P_Id int, LastName varchar(255), FirstName varchar(255), Address varchar(255),
        City varchar(255), primary key(P_Id));</query>

<query id="insert-1">insert into persons values(1,'Hansen','Ola','Timoteivn 10','Sandnes');</query>

<query id="insert-2">insert into persons values(2,'Svendson','Tove','Brogvn 23','Sandnes');</query>

<query id="insert-3">insert into persons values(3,'Pettersen','Kari','Strogt 20','Stavanger');</query>

<query id="select">select * from persons;</query>

</queries>

6. Perform CRUD Operation
7. Log all the Events
