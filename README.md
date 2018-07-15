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

How to test: We will inject our script to inputed fields on systems.
If we can, we can follow the effections of scripts to analysis the security severity.

Example for XSS payload

```

```

## Broken Authentication
All requests to system should be required althentication.


```

```
## Broken Access Control

One of the general attack ways that hackers use is escalation to go pass the business rules of system.
We will folow the business rules points to inject your scripts.
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
## Insecure Deserialization


## Sensitive Data Explosure

There are applications graphic interface (API) do not properly provide the sensitive data as banking, financial, healcare, ...

Attacker can follow the response message from server to exploit, then they can steal more modify to weak points.


## CSRF - 


# Vulnerabilities

The impactful application security risk. From that hackers can detect and exploit to steal the sensitive data, make the broken system, even do unexpected actions ...


# References

=======
## Using Components with Known Vulnerabilities
We will have components
=======

One of the general attack ways that hackers use is escalation to go pass the business rules of system.
We will folow the business rules points to inject your scripts.
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
## Insecure Deserialization

## Using Components with Known Vulnerabilities
We will have components for system


## Insufficient Logging & Monitoring
