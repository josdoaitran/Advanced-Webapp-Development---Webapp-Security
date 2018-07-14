# Advanced-Webapp-Development---Webapp-Security
Advanced Webapp Development - Webapp Security

## SQL Injection


A malicious attacker could supply:
```
username = ' OR '1'='1
sqlStr = "SELECT username FROM users WHERE username='' OR '1'='1' AND password='xxx';"
      -- Returns true
```
``` 
username = ' OR '1'='1' --
sqlStr = "SELECT username FROM users WHERE username='' OR '1'='1' -- ...'"
      -- Forcing the rest of statement, if any, as comment
```
```
username = x';DROP TABLE users;
sqlStr = "SELECT username FROM users WHERE username ='a';DROP TABLE users;'..."
      -- Piggyback another malicious SQL statement.
      -- But most SQL implementations do not permit multiple statements in one query
```

Payload examples:
```

```

## XSS - Cross Site Scripting


Types of XSS:

How to test: We will inject our script to inputed fields on systems.
If we can, we can follow the effections of scripts to analysis the security severity.

Example for XSS payload

```

```


## Broken Authentication

```

```
## Broken Access Control

```

```

## Sensitive Data Exposure
Sensitive data are the information of Web Server, internal data of server.
```
password
password-salt

user-id
card-id
```
