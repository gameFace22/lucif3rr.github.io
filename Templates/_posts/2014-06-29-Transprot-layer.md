---
layout: post
title: Transport Layer Protection
---

Synopsis:
------------------
Insufficient Transport Layer Protection is a security weakness caused by applications not taking any good security measures to protect network traffic.

Description:
----------------------
The lack of proper data encryption passes up the guarantees of confidentiality, integrity, and accountability that properly implemented encryption conveys. Not all traffic flowing between two endpoints is properly secured, which makes it possible for attackers to perform man-in-the-middle attacks.

For more details:- [Transport Layer Protection Cheat Sheet](https://www.owasp.org/index.php/Transport_Layer_Protection_Cheat_Sheet) 

Mitigation:
---------------
Providing proper transport layer protection can affect the site design. It’s easiest to require SSL for the entire site but due to performance reasons, some sites use SSL only on private pages. At a minimum, do all of the following:

1) Require SSL for all sensitive pages. Non-SSL requests to these pages should be redirected to the SSL page.

2) Set the ‘secure’ flag on all sensitive cookies.

3) Configure your SSL provider to only support strong (e.g., FIPS 140-2 compliant) algorithms.

4) Ensure your certificate is valid, not expired, not revoked, and matches all domains used by the site.

5) Backend and other connections should also use SSL or other encryption technologies.

For more details:- [Insufficient Transport Layer Protection](https://www.owasp.org/index.php/OWASP_Periodic_Table_of_Vulnerabilities_-_Insufficient_Transport_Layer_Protection) 

[OWASP Top 10 2010 A9 Insufficient Transport Layer Protection](https://www.owasp.org/index.php/Top_10_2010-A9-Insufficient_Transport_Layer_Protection) 

CVSS Base Score:
----------------------------
For more details:- [7.8(AV:N/AC:L/AU:N/C:N/I:N/A:C)](http://nvd.nist.gov/cvss.cfm?vector=%28AV:N/AC:L/AU:N/C:N/I:N/A:C%29&version=2.0) 

