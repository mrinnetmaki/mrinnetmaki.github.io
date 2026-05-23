# ConditionShoulder - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ConditionShoulder**

## Example Condition: ConditionShoulder

Profiles: [IPA-Condition](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-condition.html) version: 1.1.0, [Condition (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-Condition-uv-ips.html), [Condition (EU core)](http://hl7.eu/fhir/base/2.0.0/StructureDefinition-condition-eu-core.html), [Condition - Obligations (EPS)](https://build.fhir.org/ig/hl7-eu/eps/StructureDefinition-condition-obl-eu-eps.html)

Security Labels: device reported (Details: ObservationValue code DEVRPT = 'device reported'), patient reported (Details: ObservationValue code PATRPT = 'patient reported'), syntactic transform (Details: ObservationValue code SYNTAC = 'syntactic transform'), mapped (Details: ObservationValue code MAPPED = 'mapped'), patient asserted (Details: ObservationValue code PATAST = 'patient asserted')

**clinicalStatus**: Resolved

**verificationStatus**: Confirmed

**category**: Encounter Diagnosis

**severity**: Moderate

**code**: Shoulder problem

**subject**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**onset**: 2020-08-20

**asserter**: Pitkänen, Riikka fysioterapeutti

**note**: By urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f

> 

This problem was alleviated with some physiotherapy and well-selected exercises. However, late 2025 the problem started to come back, and the same exercises don't seem to help as much as they did before.




## Resource Content

```json
{
  "resourceType" : "Condition",
  "id" : "22e07a7b-4d9b-406d-93bc-dc60de933f1f",
  "meta" : {
    "profile" : ["http://hl7.org/fhir/uv/ipa/StructureDefinition/ipa-condition|1.1.0",
    "http://hl7.org/fhir/uv/ips/StructureDefinition/Condition-uv-ips",
    "http://hl7.eu/fhir/base/StructureDefinition/condition-eu-core",
    "http://hl7.eu/fhir/eps/StructureDefinition/condition-obl-eu-eps"],
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
  "clinicalStatus" : {
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/condition-clinical",
      "code" : "resolved",
      "display" : "Resolved"
    }],
    "text" : "Resolved"
  },
  "verificationStatus" : {
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/condition-ver-status",
      "code" : "confirmed",
      "display" : "Confirmed"
    }],
    "text" : "Confirmed"
  },
  "category" : [{
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/condition-category",
      "code" : "encounter-diagnosis",
      "display" : "Encounter Diagnosis"
    }],
    "text" : "Encounter Diagnosis"
  }],
  "severity" : {
    "coding" : [{
      "system" : "http://snomed.info/sct",
      "code" : "6736007",
      "display" : "Midgrade"
    }],
    "text" : "Moderate"
  },
  "code" : {
    "coding" : [{
      "system" : "http://snomed.info/sct",
      "code" : "249918006",
      "display" : "Shoulder stiff"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.1",
      "code" : "M24.5",
      "display" : "Nivelen kontraktuura"
    },
    {
      "system" : "http://hl7.org/fhir/sid/icd-10",
      "code" : "M24.5",
      "display" : "Contracture of joint"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.31",
      "code" : "L08",
      "display" : "Olkapään oire/vaiva"
    }],
    "text" : "Shoulder problem"
  },
  "subject" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "onsetDateTime" : "2020-08-20",
  "asserter" : {
    "display" : "Pitkänen, Riikka fysioterapeutti"
  },
  "note" : [{
    "authorReference" : {
      "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
      "display" : "Mikael Rinnetmäki, the patient"
    },
    "text" : "This problem was alleviated with some physiotherapy and well-selected exercises. However, late 2025 the problem started to come back, and the same exercises don't seem to help as much as they did before."
  }]
}

```
