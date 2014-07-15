---
Layout: POST
Title: Authentication & Sessions
---

Synopsis
---------------
Authentication is the act of establishing something (or someone) as authentic, to check that claims made by or about the thing are true. Session Management is a process by which a server maintains the state of an entity interacting with it.

Description
-----------------
Authentication is commonly performed by submitting a username or ID and one or more items of private information that only the user should know. 
Sessions are maintained on the server by a session identifier which can be passed back and forward between the client and server when transmitting and receiving requests. 

To know more about authentication guidelines, see [OWASP Guide](https://www.owasp.org/index.php/Guide_to_Authentication).

Mitigation
---------------
*Make sure userid are case insensitive and ensure a very strong password which is a combination of numbers,alpahbets,symbols and fix the length near to 10 characters.
*Ensure Secure Password Recovery Mechanism
[PASSWORD_FORGOT_SHEET] https://www.owasp.org/index.php/Forgot_Password_Cheat_Sheet
*Use Multi Factor authentication and transmit only over TLS.
*Use proper Authentication Response
BAD PRACTICE:     "Login for User foo: invalid password"
                  "Login failed, invalid user ID"
                  "Login failed; account disabled"
                  "Login failed; this user is not active"
GOOD PRACTICE:    "Login failed; Invalid userID or password"  
*Usage of authentication protocols that require no password. Like OAuth,SAML and OpenID.
*Usgae of secure Password Managers

To know more, see
[OWASP SESSION MANAGEMENT] https://www.owasp.org/index.php/Session_Management_Cheat_Sheet

CVSS Base Score:
----------------------------
[5.8(AV:N/AC:M/AU:N/C:P/I:P/A:N)](http://nvd.nist.gov/cvss.cfm?vector=(AV:N/AC:M/AU:N/C:P/I:P/A:N&version=2.0) 

