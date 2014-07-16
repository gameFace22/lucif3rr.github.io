---
Layout: POST
Title: Transport Layer Protection
---

Synopsis:
------------------
Insufficient Transport Layer Protection is a security weakness caused by applications not taking any measures to protect network traffic.

Description:
----------------------
All the traffic,flowing between two endpoints is not secured, which makes it possible for attackers to eavesdrop and to perform man-in-the-middle attacks.

For more details:- [Transport Layer Protection Cheat Sheet](https://www.owasp.org/index.php/Transport_Layer_Protection_Cheat_Sheet)
[MITM] - https://www.owasp.org/index.php/Man-in-the-middle_attack 

Mitigation:
---------------
- Implement HTTP Strict Transport Security in all browsers, which makes it possible to enforce HTTPS connections.Implement Certificate and Public Keys pinning in browsers whereever applicable.

- Use TLS for All Login and Aunthenticated pages and do not provide non-TLS pages for Secure Content.

- Do not perform redirects from Non-TLS to TLS Login Page.

- Use SSL connections whereever possible(IRC,browsers etc.)

- Strictly support strong protocols and Cryptographic Ciphers.

For more details: 

[OWASP Insufficient Transport Layer Protection](https://www.owasp.org/index.php/OWASP_Periodic_Table_of_Vulnerabilities_-_Insufficient_Transport_Layer_Protection) 

[OWASP Top 10 2010 A9 Insufficient Transport Layer Protection](https://www.owasp.org/index.php/Top_10_2010-A9-Insufficient_Transport_Layer_Protection) 

[SSL/TLS Deployment Practices](https://www.ssllabs.com/projects/best-practices/index.html)

CVSS Base Score:
----------------------------
For more details:- [7.8(AV:N/AC:L/AU:N/C:N/I:N/A:C)](http://nvd.nist.gov/cvss.cfm?vector=%28AV:N/AC:L/AU:N/C:N/I:N/A:C%29&version=2.0) 

