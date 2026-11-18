# 1. Query

#### This will return all parameter as response in JSON body.
``` 
/users?_queryFilter=true
```

```
_queryFilter=filter-expression
```
- This will return entries that match the filter expression.


```
_queryId=Identifier
```
- This specifies a query by it's identifier



# 2. Response Formats
```
_prettyPrint=true
```
- Format the body of the response


```
_fields=field[,field...]
```
- Return only the specified fields in the body of the response.


# 3. URI Scheme
```
/openidm/managed/type/id
```
- The URI scheme for accessing a managed object follows this convention, assuming the IDM web application was deployed at /openidm

```
/openidm/system/resource-name/type/id
```
- The URI scheme for accessing a system object follows this convention

```
/openidm/system.ldap/account/3483438343984739
```
- An example of system object in an LDAP directory might be

