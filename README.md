# 1. Query

#### This will return all parameter as response in JSON body.
``` 
/users?_queryFilter=true
```

#### This will return entries that match the filter expression.
```
_queryFilter=filter-expression
```

#### This specifies a query by it's identifier
```
_queryId=Identifier
```



# 2. Response 

#### Format the body of the response
```
_prettyPrint=true
```

#### Return only the specified fields in the body of the response.
```
_fields=field[,field...]
```



# 3. URI Scheme

#### The URI scheme for accessing a managed object follows this convention, assuming the IDM web application was deployed at /openidm
```
/openidm/managed/type/id
```

#### The URI scheme for accessing a system object follows this convention
```
/openidm/system/resource-name/type/id
```

#### An example of system object in an LDAP directory might be
```
/openidm/system.ldap/account/3483438343984739
```

#### Return a list of configuration objects
```
/openidm/config
```

#### Single instance configuration objects are exposed under
````
/openidm/config/object-name
````

#### Workflow objects are exposed under
````
/openidm/workflow
````

#### Schedular services are exposed under
```
/openidm/schedular
```

#### Task scanning mechanism are exposed under
```
/openidm/taskscanner
```

#### Audit logs are exposed under
```
/openidm/audit
```

#### Interact with reconciliation engine
```
/openidm/recon.
```

#### Interact with synchronization engine
```
/openidm/sync
```


#### Interact with the script service
```
/openidm/script
```

#### Interact with the repository engine
```
/openidm/repo
```

#### Manage internal objects
```
/openidm/internal
```


