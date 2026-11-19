# Colors - IG Example v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Colors**

## CodeSystem: Colors 

| | |
| :--- | :--- |
| *Official URL*:https://example.org/ig/monig/CodeSystem/color-cs | *Version*:0.1.0 |
| Draft as of 2026-11-19 | *Computable Name*:ColorCS |

 
A few colors. 

 This Code system is referenced in the content logical definition of the following value sets: 

* [Colors](ValueSet-color-vs.md)



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "color-cs",
  "url" : "https://example.org/ig/monig/CodeSystem/color-cs",
  "version" : "0.1.0",
  "name" : "ColorCS",
  "title" : "Colors",
  "status" : "draft",
  "date" : "2026-11-19T09:17:54+00:00",
  "publisher" : "Work Group Meeting HL7 Europe Malaga",
  "contact" : [{
    "name" : "Work Group Meeting HL7 Europe Malaga",
    "telecom" : [{
      "system" : "url",
      "value" : "https://hl7europe.eu/hl7-europe-working-group-meeting-malaga-2026/"
    }]
  }],
  "description" : "A few colors.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "FR",
      "display" : "France (la)"
    }]
  }],
  "content" : "complete",
  "count" : 4,
  "concept" : [{
    "code" : "blue",
    "display" : "Blue"
  },
  {
    "code" : "brown",
    "display" : "Brown"
  },
  {
    "code" : "green",
    "display" : "Green"
  },
  {
    "code" : "grey",
    "display" : "Grey"
  }]
}

```
