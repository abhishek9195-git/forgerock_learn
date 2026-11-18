# 1. Install VMWARE

# 2. INSTALL WINDOWS
- Install windows without network configuration
- Setup the network with NAT

# 3. Install java
- Install jdk inside c:/u01/java27
- update environmental variables JAVA_HOME
- Update hosts file

# 4. Mysql installation
- Install mysql 5.7.17
- Set path for bin in system variables

Connect to mysql
```
> mysql -u root -p
```

Change root password
```
> alter user 'root'@'localhost' identified by 'root';
```

Run this command
```
> install plugin validate_password soname 'validate_password.dll';
```

Run this command and check if installations are properly completed.
```
> select plugin_name, plugin_status from information_schema.plugins where plugin_name like 'validate%'
```

```
> show variables like 'validate_password%';
```

```
> set global validate_password_policy=LOW;
```

```
> set global validate_password_length=6;
```

```
> set global validate_password_number_count=0;
```

Shutdown
```
> mysqladmin -u root -p shutdown
```

# 5. OpenIDM Installation
1. Download the .zip file from github.com/OpenIdentityPlatform/OpenIDM/releases
2. Update file boot.properties

Start OpenIDM
```
startup.bat
```

Stop OpenIDM
```
shutdown
```





# WINRAR Installation
- Install winrar
