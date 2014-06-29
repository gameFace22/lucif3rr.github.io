---
layout: post
title: Insecure Cryptographic Storage
---

Synopsis:
----------------
Insecure Cryptographic Storage is a vulnerability that occurs when sensitive data is not stored securely.


Description:
-------------------
Insecure Cryptographic Storage is a collection of vulnerabilities which has to do with making sure the most important data is encrypted when it needs to be.
The most common flaw in this area is not encrypting data that deserves encryption. When encryption is employed, unsafe key generation and storage, not rotating keys, and weak algorithm usage is common.


Mitigation:
----------------
Start with manual approach. Scanners and tools cannot verify cryptographic weakness. Best way is the review of code, review of used cryptographic algorithm and key management.  
For more details-:-
[Cryptographic_Storage_Cheat_Sheet](https://www.owasp.org/index.php/Cryptographic_Storage_Cheat_Sheet)

[Owasp top 10](https://www.owasp.org/index.php/Top_10_2010-A7-Insecure_Cryptographic_Storage)

CVSS Base Score:
-------------------------

