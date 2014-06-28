---
layout: post
title: Authentication and Session Management
---

Synopsis
---------------
Authentication is the act of establishing something (or someone) as authentic, to check that claims made by or about the thing are true. Session Management is a process by which a server maintains the state of an entity interacting with it.

Description
-----------------
Authentication is commonly performed by submitting a username or ID and one or more items of private information that only the user should know. 
To know more about authentication guidelines, see:- [ OWASP Guide](https://www.owasp.org/index.php/Guide_to_Authentication).
Sessions are maintained on the server by a session identifier which can be passed back and forward between the client and server when transmitting and receiving requests. 
Mitigation
---------------
Use an authentication framework or library such as the OWASP ESAPI Authentication feature.
[ OWASP Top Ten](https://www.owasp.org/index.php/Top_10_2013-A2-Broken_Authentication_and_Session_Management)
For authentication some guidelines are to be followed like giving proper usernames and passwords. [ Authenticatio General Guidelines](https://www.owasp.org/index.php/Authentication_Cheat_Sheet#Authentication_General_Guidelines)
Session management is directly related to authentication. For more guidelines on session management, see:-[ Session Management cheatsheet](https://www.owasp.org/index.php/Session_Management_Cheat_Sheet) 
CVSS Base Score:
---------------------------- 
[5.8(AV:N/AC:M/AU:N/C:P/I:P/A:N)](http://nvd.nist.gov/cvss.cfm?vector=(AV:N/AC:M/AU:N/C:P/I:P/A:N)&version=2.0) 
