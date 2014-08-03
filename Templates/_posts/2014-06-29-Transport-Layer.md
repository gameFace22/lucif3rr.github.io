<!---
TLS
-->

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
Providing proper transport layer protection can affect the site design. It’s easiest to require SSL for the entire site but due to performance reasons, some sites use SSL only on private pages. At a minimum, do all of the following:

- Require SSL for all sensitive pages. Non-SSL requests to these pages should be redirected to the SSL page.

- Set the ‘secure’ flag on all sensitive cookies.

- Configure your SSL provider to only support strong (e.g., FIPS 140-2 compliant) algorithms.

- Ensure your certificate is valid, not expired, not revoked, and matches all domains used by the site.

- Backend and other connections should also use SSL or other encryption technologies.

For more details: 

[OWASP Insufficient Transport Layer Protection](https://www.owasp.org/index.php/OWASP_Periodic_Table_of_Vulnerabilities_-_Insufficient_Transport_Layer_Protection) 

[OWASP Top 10 2010 A9 Insufficient Transport Layer Protection](https://www.owasp.org/index.php/Top_10_2010-A9-Insufficient_Transport_Layer_Protection) 

[SSL/TLS Deployment Practices](https://www.ssllabs.com/projects/best-practices/index.html)

CVSS Base Score:
----------------------------
For more details:- [7.8(AV:N/AC:L/AU:N/C:N/I:N/A:C)](http://nvd.nist.gov/cvss.cfm?vector=%28AV:N/AC:L/AU:N/C:N/I:N/A:C%29&version=2.0) 

