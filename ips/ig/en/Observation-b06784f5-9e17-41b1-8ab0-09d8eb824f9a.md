# Observation-vitals-bloodpressure-4 - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Observation-vitals-bloodpressure-4**

## Example Observation: Observation-vitals-bloodpressure-4

Profiles: [Observation Blood Pressure Profile](http://hl7.org/fhir/R4/bp.html), [IPA-Observation](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-observation.html) version: 1.1.0, [Vital Signs Profile](http://hl7.org/fhir/R4/vitalsigns.html)

Security Label: [patient reported (Details: v3 Code System ObservationValue code PATRPT = 'patient reported')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html)

**status**: Final

**category**: Vital Signs

**code**: Blood pressure systolic & diastolic

**subject**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**effective**: 2026-01-04 15:49:06+0200

**performer**: [Mikael Rinnetmäki, the patient](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**interpretation**: Normal

**bodySite**: Left upper arm

> **component****code**: Systolic blood pressure**value**: 114 mmHg (Details: UCUM codemm[Hg] = 'mm[Hg]')**interpretation**: Normal

### ReferenceRanges

| | |
| :--- | :--- |
| - | **High** |
| * | 130 mmHg (Details: UCUM codemm[Hg] = 'mm[Hg]') |


> **component****code**: Diastolic blood pressure**value**: 61 mmHg (Details: UCUM codemm[Hg] = 'mm[Hg]')**interpretation**: Normal

### ReferenceRanges

| | |
| :--- | :--- |
| - | **High** |
| * | 85 mmHg (Details: UCUM codemm[Hg] = 'mm[Hg]') |




## Resource Content

```json
{
  "resourceType" : "Observation",
  "id" : "b06784f5-9e17-41b1-8ab0-09d8eb824f9a",
  "meta" : {
    "profile" : ["http://hl7.org/fhir/StructureDefinition/bp",
    "http://hl7.org/fhir/uv/ipa/StructureDefinition/ipa-observation|1.1.0",
    "http://hl7.org/fhir/StructureDefinition/vitalsigns"],
    "security" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ObservationValue",
      "code" : "PATRPT",
      "display" : "patient reported"
    }]
  },
  "status" : "final",
  "category" : [{
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/observation-category",
      "code" : "vital-signs",
      "display" : "Vital Signs"
    }]
  }],
  "code" : {
    "coding" : [{
      "system" : "http://loinc.org",
      "code" : "85354-9",
      "display" : "Blood pressure panel with all children optional"
    }],
    "text" : "Blood pressure systolic & diastolic"
  },
  "subject" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "effectiveDateTime" : "2026-01-04T15:49:06+02:00",
  "performer" : [{
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki, the patient"
  }],
  "interpretation" : [{
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ObservationInterpretation",
      "code" : "N",
      "display" : "Normal"
    }]
  }],
  "bodySite" : {
    "coding" : [{
      "system" : "http://snomed.info/sct",
      "code" : "368208006",
      "display" : "Left upper arm"
    }]
  },
  "component" : [{
    "code" : {
      "coding" : [{
        "system" : "http://loinc.org",
        "code" : "8480-6",
        "display" : "Systolic blood pressure"
      }],
      "text" : "Systolic blood pressure"
    },
    "valueQuantity" : {
      "value" : 114,
      "unit" : "mmHg",
      "system" : "http://unitsofmeasure.org",
      "code" : "mm[Hg]"
    },
    "interpretation" : [{
      "coding" : [{
        "system" : "http://terminology.hl7.org/CodeSystem/v3-ObservationInterpretation",
        "code" : "N",
        "display" : "Normal"
      }]
    }],
    "referenceRange" : [{
      "high" : {
        "value" : 130,
        "unit" : "mmHg",
        "system" : "http://unitsofmeasure.org",
        "code" : "mm[Hg]"
      }
    }]
  },
  {
    "code" : {
      "coding" : [{
        "system" : "http://loinc.org",
        "code" : "8462-4",
        "display" : "Diastolic blood pressure"
      }],
      "text" : "Diastolic blood pressure"
    },
    "valueQuantity" : {
      "value" : 61,
      "unit" : "mmHg",
      "system" : "http://unitsofmeasure.org",
      "code" : "mm[Hg]"
    },
    "interpretation" : [{
      "coding" : [{
        "system" : "http://terminology.hl7.org/CodeSystem/v3-ObservationInterpretation",
        "code" : "N",
        "display" : "Normal"
      }]
    }],
    "referenceRange" : [{
      "high" : {
        "value" : 85,
        "unit" : "mmHg",
        "system" : "http://unitsofmeasure.org",
        "code" : "mm[Hg]"
      }
    }]
  }]
}

```
