---
layout: post
title: XPath Injection
---

Synopsis:
----------------
XPath Injection attacks occur when a web site uses user-supplied information to construct an XPath query for XML data.

Description:
--------------------
By sending intentionally malformed information as input, an attacker can find out how the XML data is structured, or access data that cannot be normally accessed. The attacker’s privileges on the web site can be elevated if the XML data is being used for authentication (such as an XML based user file).

Read more:For more details:-[OWASP Guide on XPATH Injection](https://www.owasp.org/index.php/XPATH_Injection)  

Mitigation:
----------------
Use parameterized XPath queries (e.g. using XQuery). This will help ensure separation between data plane and control plane. Use an "accept known good" input validation strategy, i.e., use a whitelist of acceptable inputs that strictly conform to specifications.

Read more:For more details:-[mitre definitions](http://cwe.mitre.org/data/definitions/643.html)  


CVSS Base Score:
----------------------------
For more details:-[5.0 (AV:N/AC:L/AU:N/C:P/I:N/A:N)](http://nvd.nist.gov/cvss.cfm?vector=(AV:N/AC:L/AU:N/C:P/I:N/A:N)&version=2.0) 

