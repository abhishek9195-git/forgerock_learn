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



# 2. Response Formats

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

