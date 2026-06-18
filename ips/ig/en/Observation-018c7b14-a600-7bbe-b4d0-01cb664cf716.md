# Observation-lab-u-krea-1 - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Observation-lab-u-krea-1**

## Example Observation: Observation-lab-u-krea-1

Profiles: [IPA-Observation](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-observation.html) version: 1.1.0, [Observation Results - Laboratory/Pathology (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-Observation-results-laboratory-pathology-uv-ips.html), [Observation: Medical Test Result (EU core)](http://hl7.eu/fhir/base/2.0.0/StructureDefinition-medicalTestResult-eu-core.html)

Security Labels: [device reported (Details: ObservationValue code DEVRPT = 'device reported')](http://terminology.hl7.org/7.2.0/CodeSystem-v3-ObservationValue.html), [patient reported (Details: ObservationValue code PATRPT = 'patient reported')](http://terminology.hl7.org/7.2.0/CodeSystem-v3-ObservationValue.html), [syntactic transform (Details: ObservationValue code SYNTAC = 'syntactic transform')](http://terminology.hl7.org/7.2.0/CodeSystem-v3-ObservationValue.html), [mapped (Details: ObservationValue code MAPPED = 'mapped')](http://terminology.hl7.org/7.2.0/CodeSystem-v3-ObservationValue.html), [patient asserted (Details: ObservationValue code PATAST = 'patient asserted')](http://terminology.hl7.org/7.2.0/CodeSystem-v3-ObservationValue.html)

**status**: Final

**category**: Laboratory

**code**: U -Krea (kreatiniini)

**subject**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**effective**: 2023-12-18 06:00:00+0200

**performer**: Fimlab

**value**: 12.4 mg/dl (Details: UCUM codemg/dl = 'mg/dl')



## Resource Content

```json
{
  "resourceType" : "Observation",
  "id" : "018c7b14-a600-7bbe-b4d0-01cb664cf716",
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
      "code" : "2161-8",
      "display" : "Creatinine [Mass/volume] in Urine"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.3",
      "code" : "2145",
      "display" : "U -Krea"
    }],
    "text" : "U -Krea (kreatiniini)"
  },
  "subject" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "effectiveDateTime" : "2023-12-18T06:00:00+02:00",
  "performer" : [{
    "display" : "Fimlab"
  }],
  "valueQuantity" : {
    "value" : 12.4,
    "unit" : "mg/dl",
    "system" : "http://unitsofmeasure.org",
    "code" : "mg/dl"
  }
}

```
