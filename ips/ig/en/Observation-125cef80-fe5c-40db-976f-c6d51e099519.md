# Observation-b-erybla-1 - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Observation-b-erybla-1**

## Example Observation: Observation-b-erybla-1

Profiles: [IPA-Observation](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-observation.html) version: 1.1.0, [Observation Results - Laboratory/Pathology (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-Observation-results-laboratory-pathology-uv-ips.html), [Observation: Medical Test Result (EU core)](http://hl7.eu/fhir/base/2.0.0/StructureDefinition-medicalTestResult-eu-core.html)

Security Labels: device reported (Details: ObservationValue code DEVRPT = 'device reported'), patient reported (Details: ObservationValue code PATRPT = 'patient reported'), syntactic transform (Details: ObservationValue code SYNTAC = 'syntactic transform'), mapped (Details: ObservationValue code MAPPED = 'mapped'), patient asserted (Details: ObservationValue code PATAST = 'patient asserted')

**status**: Final

**category**: Laboratory

**code**: B -EryBla (erytroblastit)

**subject**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**effective**: 2024-12-13 08:00:00+0200

**performer**: Fimlab

**value**: 0 /l (Details: UCUM code/L = '/L')

**interpretation**: Normal

### ReferenceRanges

| | | | |
| :--- | :--- | :--- | :--- |
| - | **Low** | **High** | **Text** |
| * | 0 | 200000000 | 0-0.02x10E9/l |



## Resource Content

```json
{
  "resourceType" : "Observation",
  "id" : "125cef80-fe5c-40db-976f-c6d51e099519",
  "meta" : {
    "profile" : ["http://hl7.org/fhir/uv/ipa/StructureDefinition/ipa-observation|1.1.0",
    "http://hl7.org/fhir/uv/ips/StructureDefinition/Observation-results-laboratory-pathology-uv-ips",
    "http://hl7.eu/fhir/base/StructureDefinition/medicalTestResult-eu-core"],
    "security" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ObservationValue",
      "code" : "DEVRPT",
      "display" : "device reported"
    },
    {
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ObservationValue",
      "code" : "PATRPT",
      "display" : "patient reported"
    },
    {
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ObservationValue",
      "code" : "SYNTAC",
      "display" : "syntactic transform"
    },
    {
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ObservationValue",
      "code" : "MAPPED",
      "display" : "mapped"
    },
    {
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ObservationValue",
      "code" : "PATAST",
      "display" : "patient asserted"
    }]
  },
  "status" : "final",
  "category" : [{
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/observation-category",
      "code" : "laboratory"
    }]
  }],
  "code" : {
    "coding" : [{
      "system" : "http://loinc.org",
      "code" : "715-3",
      "display" : "Normoblasts [#/volume] in Blood"
    },
    {
      "system" : "https://fimlab.fi/",
      "code" : "B%20-EryBla",
      "display" : "B -EryBla"
    }],
    "text" : "B -EryBla (erytroblastit)"
  },
  "subject" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "effectiveDateTime" : "2024-12-13T08:00:00+02:00",
  "performer" : [{
    "display" : "Fimlab"
  }],
  "valueQuantity" : {
    "value" : 0,
    "unit" : "/l",
    "system" : "http://unitsofmeasure.org",
    "code" : "/L"
  },
  "interpretation" : [{
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ObservationInterpretation",
      "code" : "N",
      "display" : "Normal"
    }]
  }],
  "referenceRange" : [{
    "low" : {
      "value" : 0
    },
    "high" : {
      "value" : 200000000
    },
    "text" : "0-0.02x10E9/l"
  }]
}

```
