# Observation-vitals-bloodpressure-1 - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Observation-vitals-bloodpressure-1**

## Example Observation: Observation-vitals-bloodpressure-1

Profiles: [Observation Blood Pressure Profile](http://hl7.org/fhir/R4/bp.html), [IPA-Observation](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-observation.html) version: 1.1.0, [Vital Signs Profile](http://hl7.org/fhir/R4/vitalsigns.html)

**status**: Final

**category**: Vital Signs

**code**: Blood pressure systolic & diastolic

**subject**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**effective**: 2025-10-24

**performer**: Loukkaanhuhta, Heli Työterveyshoitaja

**interpretation**: Normal

**bodySite**: Left upper arm

> **component****code**: Systolic blood pressure**value**: 168 mmHg (Details: UCUM codemm[Hg] = 'mm[Hg]')

> **component****code**: Diastolic blood pressure**value**: 88 mmHg (Details: UCUM codemm[Hg] = 'mm[Hg]')



## Resource Content

```json
{
  "resourceType" : "Observation",
  "id" : "87fd93df-3a9e-433a-a824-97702a294dce",
  "meta" : {
    "profile" : ["http://hl7.org/fhir/StructureDefinition/bp",
    "http://hl7.org/fhir/uv/ipa/StructureDefinition/ipa-observation|1.1.0",
    "http://hl7.org/fhir/StructureDefinition/vitalsigns"]
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
  "effectiveDateTime" : "2025-10-24",
  "performer" : [{
    "display" : "Loukkaanhuhta, Heli Työterveyshoitaja"
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
      "value" : 168,
      "unit" : "mmHg",
      "system" : "http://unitsofmeasure.org",
      "code" : "mm[Hg]"
    }
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
      "value" : 88,
      "unit" : "mmHg",
      "system" : "http://unitsofmeasure.org",
      "code" : "mm[Hg]"
    }
  }]
}

```
