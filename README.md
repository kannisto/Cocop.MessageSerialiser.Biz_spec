
Cocop.MessageSerialiser.Biz API specification v.2.0
===================================================

---

<img src="logos.png" alt="COCOP and EU" style="display:block;margin-right:auto" />

COCOP - Coordinating Optimisation of Complex Industrial Processes  
https://cocop-spire.eu/

This project has received funding from the European Union's Horizon 2020 research and innovation programme under grant agreement No 723661. This piece of software reflects only the authors' views, and the Commission is not responsible for any use that may be made of the information contained therein.

---


Author
------

Petri Kannisto, Tampere University, Finland  
https://github.com/kannisto  
http://kannisto.org

**Please make sure to read and understand [LICENSE.txt](./LICENSE.txt)!**


## COCOP Toolkit

This application is a part of COCOP Toolkit, which was developed to enable a
decoupled and well-scalable architecture in industrial systems. Please see
https://kannisto.github.io/Cocop-Toolkit/


## Introduction

This is a specification for generic APIs that serialise and deserialise (or to
encode and decode) messages that contain production schedules for
industrial systems. Please familiarise yourself with this page:
https://kannisto.github.io/Cocop-Toolkit/messageserialiser.html

The specification consists of XML documents that specify a profile built upon 
standard-based XML schemata. This profile is a subset of what the schemata
specify. These XML documents shall be complied in any implementation of 
Cocop.MessageSerialiser.Biz. Although the XML files do not unambiguously specify
the possible content of the files, they provide guidelines of what features
shall be supported and how they are structured.

The underlying XML schemata have been published in B2MML-BatchML V0600
(Business to Manufacturing Markup Language) by Manufacturing Enterprise 
Solutions Association (MESA International).

Please see [LICENSE.txt](./LICENSE.txt) for legal conditions. You can find 
B2MML at http://www.mesa.org/en/B2MML.asp .

**Please note**:
* This application has not been certified for compliance with B2MML
* This application was not created by MESA International

See also:

* Github repo: https://github.com/kannisto/Cocop.MessageSerialiser.Biz_spec


## XML Files

### "Neg*.xml"

These files are meant for the negative testing of applications (i.e., error handling).

### "ProcessProductionSchedule*.xml"

These files specify how to represent production schedules in XML.
