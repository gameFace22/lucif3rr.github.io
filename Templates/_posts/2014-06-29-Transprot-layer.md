---
layout: post
title: Insufficient Transport Layer Protection
---

Synopsis:
------------------
Insufficient Transport Layer Protection is a security weakness caused by applications not taking any measures to protect network traffic.

Description:
----------------------
Not all traffic flowing between two endpoints is properly secured, which makes it possible for attackers to perform man-in-the-middle attacks.

For more details:- [Transport Layer Protection Cheat Sheet](https://www.owasp.org/index.php/Transport_Layer_Protection_Cheat_Sheet) 

Mitigation:
---------------
Implement HTTP Strict Transport Security in all browsers, which makes it possible to better enforce secure connections. Implement Certificate and Public Key pinning in browsers where applicable.

For more details:- [Insufficient Transport Layer Protection](https://www.owasp.org/index.php/OWASP_Periodic_Table_of_Vulnerabilities_-_Insufficient_Transport_Layer_Protection) 

[Top 10 2010 A9 Insufficient Transport Layer Protection](https://www.owasp.org/index.php/Top_10_2010-A9-Insufficient_Transport_Layer_Protection) 

CVSS Base Score:
----------------------------
For more details:- [7.8(AV:N/AC:L/AU:N/C:N/I:N/A:C)](http://nvd.nist.gov/cvss.cfm?vector=%28AV:N/AC:L/AU:N/C:N/I:N/A:C%29&version=2.0) 

