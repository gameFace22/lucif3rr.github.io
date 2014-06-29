---
layout: post
title: SQL Injection
---

Synopsis:
----------------
SQL injection attacks are a type of injection attack, in which SQL commands are injected into data-plane input in order to effect the execution of predefined SQL commands.

Description:
-------------------
A successful SQL injection exploit can read sensitive data from the database, modify database data (Insert/Update/Delete), execute administration operations on the database (such as shutdown the DBMS), recover the content of a given file present on the DBMS file system and in some cases issue commands to the operating system.

For more details:- [OWASP guide on SQL Injection](https://www.owasp.org/index.php/SQL_Injection) 
Also see:-[mitre definitions](http://cwe.mitre.org/data/definitions/89.html)

Mitigation:
----------------
Prevent user supplied input which contains malicious SQL from affecting the logic of the executed query.
Use persistence layers such as Hibernate or Enterprise Java Beans, which can provide significant protection against SQL injection if used properly.

For more details:-[Testing for SQL injection attacks](https://www.owasp.org/index.php/Testing_for_SQL_Injection_(OWASP-DV-005))

See SQL-Injection [Prevention cheat sheet](https://www.owasp.org/index.php/SQL_Injection_Prevention_Cheat_Sheet) 


CVSS Base Score:
----------------------------
[7.5 (AV:N/AC:L/AU:N/C:P/I:P/A:P)](http://nvd.nist.gov/cvss.cfm?vector=%28AV:N/AC:L/AU:N/C:P/I:P/A:P%29&version=2.0) 

