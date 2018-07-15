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

Cross-Site Scripting (XSS) is a special form of "Code Injection Attack", whereas the attackers inject malicious client-side script (e.g., JavaScript) into your web pages (e.g., through the comment field) that would be saved in database.

Types of XSS:

Example for XSS payload

```

```


## Broken Authentication


## Sensitive Data Explosure

There are applications graphic interface (API) do not properly provide the sensitive data as banking, financial, healcare, ...

Attacker can follow the response message from server to exploit, then they can steal more modify to weak points.


## CSRF - 


# Vulnerabilities

The impactful application security risk. From that hackers can detect and exploit to steal the sensitive data, make the broken system, even do unexpected actions ...


# References


