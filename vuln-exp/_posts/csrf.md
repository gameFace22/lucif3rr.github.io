---
layout: post
title: Cross Site Request Forgery (CSRF)
---

Synopsis
--------------
CSRF is an attack which forces an end user to execute unwanted actions on a web application in which he/she is currently authenticated.

Description:
------------------
CSRF attack occurs when a malicious Web site, email, blog, instant message, or program causes a user’s Web browser to perform an unwanted action on a trusted site for which the user is currently authenticated. CSRF attacks generally target functions that cause a state change on the server but can also be used to access sensitive data.
To know more about CSRF visit:- [ OWASP Guide on Cross-Site Request Forgery](https://www.owasp.org/index.php/Cross-Site_Request_Forgery_(CSRF))

Mitigation
---------------
Using a Synchronizer Token is one way that an application can rely upon the Same-Origin Policy to prevent CSRF by maintaining a secret token to authenticate requests. To know more:- [Cross-Site Request Forgery Prevention Cheatsheet](https://www.owasp.org/index.php/Cross-Site_Request_Forgery_(CSRF)_Prevention_Cheat_Sheet#General_Recommendation:_Synchronizer_Token_Pattern).

For see:- [ CSRF prevention without Synchronizer token](https://www.owasp.org/index.php/Cross-Site_Request_Forgery_(CSRF)_Prevention_Cheat_Sheet#CSRF_Prevention_without_a_Synchronizer_Token)

[OWASP Top 10:](https://www.owasp.org/index.php/Top_10_2013-A8-Cross-Site_Request_Forgery_(CSRF))

CVSS Base Score:
----------------

[6.8(AV:N/AC:M/AU:N/C:P/I:P/A:P)](http://nvd.nist.gov/cvss.cfm?vector=%28AV:N/AC:M/AU:N/C:P/I:P/A:P%29&version=2.0)
