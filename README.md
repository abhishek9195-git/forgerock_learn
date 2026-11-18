# 1. Install VMWARE


# 2. INSTALL WINDOWS
- Install windows without network configuration
- Setup the network with NAT
- ipconfig and Update hosts file


# 3. JAVA INSTALLATION 
- Install jdk inside c:/u01/java27

Set User Variable
```
JAVA_HOME: C:\U01\app\JAVA27 
```

Set System Variable
```
C:\u01\app\JAVA27
```

# 4. MAVEN INSTALLATION

Set User Variable
```
MAVEN_HOME: c:\u01\app\apache-maven-3.10.1-bin\apache-maven-3.10.1\bin
```

Set System Variable
```
%MAVEN_HOME%\bin
```

# 5. MYSQL INSTALLATION

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


# 6. OPENIDM INSTALLATION
1. Download the .zip file from github.com/OpenIdentityPlatform/OpenIDM/releases
2. Download file: openidm:7.1.2.zip. (DON'T DOWNLOAD Source code option).
3. Update file boot.properties

Set User Variable
```
OPENIDM_HOME: C:\U01\app\openidm 
```

Set System Variable
```
C:\u01\app\openidm
```

Start OpenIDM
```
> startup.bat
```
USERNAME: openidm-admin
PASSWORD: openidm-admin

Stop OpenIDM (done from felix console)
```
> shutdown
```





# WINRAR Installation
- Install winrar
