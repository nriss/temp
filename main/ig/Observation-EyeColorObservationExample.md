# Eye color observation example - IG Example v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Eye color observation example**

## Example Observation: Eye color observation example

-------

**French**

-------

Profil: [Eye color observation](StructureDefinition-eye-color-observation.md)

**status**: Final

**category**: Exam

**code**: Eye color

**subject**: Jane Doe

**effective**: 2026-11-19

**value**: Green

-------

**English**

-------

Profile: [Eye color observation](StructureDefinition-eye-color-observation.md)

**status**: Final

**category**: Exam

**code**: Eye color

**subject**: Jane Doe

**effective**: 2026-11-19

**value**: Green



## Resource Content

```json
{
  "resourceType" : "Observation",
  "id" : "EyeColorObservationExample",
  "meta" : {
    "profile" : ["https://example.org/ig/monig/StructureDefinition/eye-color-observation"]
  },
  "status" : "final",
  "category" : [{
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/observation-category",
      "code" : "exam"
    }]
  }],
  "code" : {
    "text" : "Eye color"
  },
  "subject" : {
    "display" : "Jane Doe"
  },
  "effectiveDateTime" : "2026-11-19",
  "valueCodeableConcept" : {
    "coding" : [{
      "system" : "https://example.org/ig/monig/CodeSystem/color-cs",
      "code" : "green",
      "display" : "Green"
    }]
  }
}

```
