---
layout: post
title: Input validation
---
Synopsis:
---------------
Input validation refers to the process of validating all the input to an application before using it. 

Description:
------------------
Many applications do not plan input validation, and leave it up to the individual developers. This is a recipe for disaster, as different developers will certainly all choose a different approach, and many will simply leave it out in the pursuit of more interesting development.

Mitigation:
---------------
Use an input validation framework such as Struts or the OWASP ESAPI Validation API.
Use an "accept known good" input validation strategy.
For more details:- [mitre definition](http://cwe.mitre.org/data/definitions/20.html)

For guidance for providing Input Validation security functionality in applications:- [Input Validation Cheat Sheet
](https://www.owasp.org/index.php/Input_Validation_Cheat_Sheet)

CVSS Base Score:
----------------------------

