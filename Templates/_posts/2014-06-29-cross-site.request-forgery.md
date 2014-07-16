---
Layout: post
Title: Cross Site Request Forgery(CSRF)
---

Synopsis
--------------
CSRF is an attack which forces an end user to execute unwanted actions on a web application in which he/she is currently authenticated.

Description
------------------
CSRF attack occurs when a malicious Web site, email, blog, instant message, or program causes a user’s Web browser to perform an unwanted action on a trusted site for which the user is currently authenticated. CSRF attacks generally target functions that cause a state change on the server but can also be used to access sensitive data.

To know more about CSRF visit: [ OWASP Guide on Cross-Site Request Forgery](https://www.owasp.org/index.php/Cross-Site_Request_Forgery_(CSRF))

Mitigation
---------------
*Only accepting POST Requests and using a secret cookie.

*URL Rewriting - This might be seen as a useful CSRF prevention technique as the attacker can not guess the victim's session ID. However, the user’s credential is exposed over the URL.

*Using Synchronizer Token Pattern which requires the genrating of random challenge tokens that are associated with the current session.
http://www.corej2eepatterns.com/Design/PresoDesign.htm

*Double Submit Cookies which is definedas sending a random value in both a cookie and as a request parameter.

*Encryped Token Pattern leverages an encryption rather than comparison,method of Token-validation.

*Without CSRF a Synchronizer Token,check the origin HTTP header and ensure no XSS Vulneribilities.
https://wiki.mozilla.org/Security/Origin 

Also see:[OWASP CSRF prevention without Synchronizer token](https://www.owasp.org/index.php/Cross-Site_Request_Forgery_(CSRF)_Prevention_Cheat_Sheet#CSRF_Prevention_without_a_Synchronizer_Token)
[OWASP Top 10:](https://www.owasp.org/index.php/Top_10_2013-A8-Cross-Site_Request_Forgery_(CSRF))
[TESTING FOR CSRF] https://www.owasp.org/index.php/Testing_for_CSRF_%28OWASP-SM-005%29

CVSS Base Score:
-----------------------------
[6.8(AV:N/AC:M/AU:N/C:P/I:P/A:P)](http://nvd.nist.gov/cvss.cfm?vector=%28AV:N/AC:M/AU:N/C:P/I:P/A:P%29&version=2.0)
