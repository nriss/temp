# Eye color observation - IG Example v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Eye color observation**

## Resource Profile: Eye color observation 

| | |
| :--- | :--- |
| *Official URL*:https://example.org/ig/monig/StructureDefinition/eye-color-observation | *Version*:0.1.0 |
| Draft as of 2026-11-19 | *Computable Name*:EyeColorObservation |

 
Observation indicating the eye color of a patient. 

**Utilisations:**

* Exemples pour ce/t/te Profil: [Observation/EyeColorObservationExample](Observation-EyeColorObservationExample.md)

Vous pouvez également vérifier [les usages dans le FHIR IG Statistics](https://packages2.fhir.org/xig/resource/org.fhir.eu.monig|current/StructureDefinition/StructureDefinition-eye-color-observation.json)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-eye-color-observation.csv), [Excel](StructureDefinition-eye-color-observation.xlsx), [Schematron](StructureDefinition-eye-color-observation.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "eye-color-observation",
  "url" : "https://example.org/ig/monig/StructureDefinition/eye-color-observation",
  "version" : "0.1.0",
  "name" : "EyeColorObservation",
  "title" : "Eye color observation",
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
  "description" : "Observation indicating the eye color of a patient.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "FR",
      "display" : "France (la)"
    }]
  }],
  "fhirVersion" : "4.0.1",
  "mapping" : [{
    "identity" : "workflow",
    "uri" : "http://hl7.org/fhir/workflow",
    "name" : "Workflow Pattern"
  },
  {
    "identity" : "sct-concept",
    "uri" : "http://snomed.info/conceptdomain",
    "name" : "SNOMED CT Concept Domain Binding"
  },
  {
    "identity" : "v2",
    "uri" : "http://hl7.org/v2",
    "name" : "HL7 v2 Mapping"
  },
  {
    "identity" : "rim",
    "uri" : "http://hl7.org/v3",
    "name" : "RIM Mapping"
  },
  {
    "identity" : "w5",
    "uri" : "http://hl7.org/fhir/fivews",
    "name" : "FiveWs Pattern Mapping"
  },
  {
    "identity" : "sct-attr",
    "uri" : "http://snomed.org/attributebinding",
    "name" : "SNOMED CT Attribute Binding"
  }],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Observation",
  "baseDefinition" : "http://hl7.eu/fhir/base/StructureDefinition/medicalTestResult-eu-core|2.0.1",
  "derivation" : "constraint",
  "differential" : {
    "element" : [{
      "id" : "Observation",
      "path" : "Observation"
    },
    {
      "id" : "Observation.code.text",
      "path" : "Observation.code.text",
      "patternString" : "Eye color"
    },
    {
      "id" : "Observation.value[x]",
      "path" : "Observation.value[x]",
      "type" : [{
        "code" : "CodeableConcept"
      }]
    },
    {
      "id" : "Observation.value[x]:valueCodeableConcept",
      "path" : "Observation.value[x]",
      "sliceName" : "valueCodeableConcept",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "CodeableConcept"
      }],
      "binding" : {
        "strength" : "required",
        "valueSet" : "https://example.org/ig/monig/ValueSet/color-vs|0.1.0"
      }
    }]
  }
}

```
