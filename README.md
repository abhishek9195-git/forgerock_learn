# 1. Task: Load the OpenIDM schema into mysql database

Step 1. Loading a schema creates a user in openidm.
Step 2. Before loading a schema, we can change the default username/password in  openidm/db/mysql/conf/datasource.jdbc-default.json file.
Step 3. SQL Scripts are available in openidm/db/mysql/scripts/ folder
Step 4. Execute below 6 SQL scripts.
Step 5. Open the command prompt in folder openidm/db/mysql/scripts

```
> mysql -u root -p
mysql> source openidm.sql
mysql> source activiti.mysql.create.engine.sql
mysql> source activiti.mysql.create.history.sql
mysql> source activiti.mysql.create.identity.sql
mysql> show tables
```

# 2. Task: Switch your repository to MYSQL

Step 1. Locate openidm/conf/repo.orientdb.json and delete.
   
Step 2. Copy the MySQL configuration files
   Locate datasource.jdbc-default.json and repo.jdbc.json inside folder openidm/db/mysql/conf/.
   Copy both files and paste it inside openidm/conf

Step 3. Add the MySQL JDBC driver
   Download mysql-connector-java-8.0.16.jar and place it inside openidm/bundle/

Step 4. Locate file openidm/conf/boot/boot.properties and open it. Validate below lines.
   openidm.repo.host = localhost
   openidm.repo.port = 3306

Step 5. Start OpenIDM
   openidm > startup.bat
