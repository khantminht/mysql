>## choose database
   USE wdf7780;

>## show Table
>    SHOW TABLES;

>    SHOW FULL TABLES;       (tablename | tabletype)
>    SHOW TABLES FROM wdf7780;
>    SHOW FULL TABLES FROM wdf7780;

==> show precise only one tablename
 => Method1
    DESCRIBE tablename;    (table structure in phymyadmin)
    DESC tablename;

 => Method2
    SHOW COLUMNS FROM tablename;
    SHOW COLUMNS FROM databasename.tablename;  *(from current db to another db)
    SHOW COLUMNS FROM tablename IN databasename;

==> Create Table
    CREATE TABLE tablenames(
        column1 datatype,
        column2 datatype,
        column3 datatype,
        .
        .
        .
        column'n' datatype
    );

    CREATE TABLE persons(
        personid INT,
        firstname VARCHAR(225),
        lastname VARCHAR(225),
        city VARCHAR(225),
        address VARCHAR(225)
    );

==> Drop table 
    DROP TABLE tablename;
    DROP TABLE databasename.table;