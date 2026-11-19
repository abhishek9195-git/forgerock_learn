# 1. Task: Load the schema 
1. Loading a schema creates a user in openidm.
2. Before loading a schema, we can change the default username/password in openidm/db/mysql/conf/datasource.jdbc-default.json file.
4. SQL Scripts are available in openidm/db/mysql/scripts/ folder
5. Execute below 6 SQL scripts.
6. Open the command prompt in folder openidm/db/mysql/scripts

```
> mysql -u root -p
```

```
mysql> source openidm.sql
```

