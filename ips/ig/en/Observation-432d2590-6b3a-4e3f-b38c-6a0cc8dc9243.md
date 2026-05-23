# Observation-alcohol-use - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Observation-alcohol-use**

## Example Observation: Observation-alcohol-use

Profiles: [IPA-Observation](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-observation.html) version: 1.1.0, [Observation Social History - Alcohol Use (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-Observation-alcoholuse-uv-ips.html) version: 2.0.0

Security Label: patient reported (Details: ObservationValue code PATRPT = 'patient reported')

**status**: Final

**category**: Social History

**code**: Alcoholic drinks per day

**subject**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**effective**: 2026-01-11 20:41:00+0200

**performer**: [Mikael Rinnetmäki, the patient](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**value**: 0.05 alcoholic drinks per day (Details: UCUM code/d = '/d')



## Resource Content

```json
{
  "resourceType" : "Observation",
  "id" : "432d2590-6b3a-4e3f-b38c-6a0cc8dc9243",
  "meta" : {
    "profile" : ["http://hl7.org/fhir/uv/ipa/StructureDefinition/ipa-observation|1.1.0",
    "http://hl7.org/fhir/uv/ips/StructureDefinition/Observation-alcoholuse-uv-ips|2.0.0"],
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
      "code" : "social-history"
    }]
  }],
  "code" : {
    "coding" : [{
      "system" : "http://loinc.org",
      "code" : "74013-4",
      "display" : "Alcoholic drinks per day"
    }],
    "text" : "Alcoholic drinks per day"
  },
  "subject" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "effectiveDateTime" : "2026-01-11T20:41:00+02:00",
  "performer" : [{
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki, the patient"
  }],
  "valueQuantity" : {
    "value" : 0.05,
    "unit" : "alcoholic drinks per day",
    "system" : "http://unitsofmeasure.org",
    "code" : "/d"
  }
}

```
