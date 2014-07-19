---
Layout: POST
Title: Web Service Security
---

Synopsis:
---------------
Web services is a format that any application can use, regardless of the data being transported. 

Description:
-------------------
Web services let any application communicate with any other application without having to consider the language it was developed in or the format of the data.While the web applications are typically HTML-based and web services are XML-based.

For more details:- [OWASP Web Services](https://www.owasp.org/index.php/Web_Services)

Mitigation:
-------------
- Transport Confidentiality protects against from eavesdropping and Man-in-the-middle attacks against the server.So better to use TLS

- Client Cetificate Authentication using SSL is a strong form of Authentication required. Basic Authentication over SSL is not mandatory.

- SOAP encoding styles are meant to move data between software objects into XML format and back again. Enforce the same between the client and server.

- Message Confedentiality - Messages containing sensitive data must be encrypted using a strong cipher.

- Very important is Validation against malformed XML entities,XML Bomb attacks,external entity attacks.

- Ensure Virus Scanning technology is installed,updated and preferably  inline so that the files and attachments could be checked before being saved on disk.

For more details : [OWASP Web Service Security] https://www.owasp.org/index.php/Web_Service_Security_Cheat_Sheet

CVSS Base Score:
-------------------------- 

