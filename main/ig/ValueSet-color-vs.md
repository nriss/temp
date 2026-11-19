# Colors - IG Example v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Colors**

## ValueSet: Colors 

| | |
| :--- | :--- |
| *Official URL*:https://example.org/ig/monig/ValueSet/color-vs | *Version*:0.1.0 |
| Draft as of 2026-11-19 | *Computable Name*:ColorVS |

 
A few colors. 

 **References** 

* [Eye color observation](StructureDefinition-eye-color-observation.md)

### Définition logique (CLD)

 

### Expansion

-------

 Explanation of the columns that may appear on this page: 

| | |
| :--- | :--- |
| Level | A few code lists that FHIR defines are hierarchical - each code is assigned a level. In this scheme, some codes are under other codes, and imply that the code they are under also applies |
| System | The source of the definition of the code (when the value set draws in codes defined elsewhere) |
| Code | The code (used as the code in the resource instance) |
| Display | The display (used in the*display*element of a[Coding](http://hl7.org/fhir/R4/datatypes.html#Coding)). If there is no display, implementers should not simply display the code, but map the concept into their application |
| Definition | An explanation of the meaning of the concept |
| Comments | Additional notes about how to use the code |



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "color-vs",
  "url" : "https://example.org/ig/monig/ValueSet/color-vs",
  "version" : "0.1.0",
  "name" : "ColorVS",
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
  "compose" : {
    "include" : [{
      "system" : "https://example.org/ig/monig/CodeSystem/color-cs",
      "version" : "0.1.0"
    }]
  }
}

```
