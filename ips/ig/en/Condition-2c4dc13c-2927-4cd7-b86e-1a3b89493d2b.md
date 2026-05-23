# ConditionPulmonaryEmbolism - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ConditionPulmonaryEmbolism**

## Example Condition: ConditionPulmonaryEmbolism

Profiles: [IPA-Condition](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-condition.html) version: 1.1.0, [Condition (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-Condition-uv-ips.html), [Condition (EU core)](http://hl7.eu/fhir/base/2.0.0/StructureDefinition-condition-eu-core.html), [Condition - Obligations (EPS)](https://build.fhir.org/ig/hl7-eu/eps/StructureDefinition-condition-obl-eu-eps.html)

Security Labels: device reported (Details: ObservationValue code DEVRPT = 'device reported'), patient reported (Details: ObservationValue code PATRPT = 'patient reported'), syntactic transform (Details: ObservationValue code SYNTAC = 'syntactic transform'), mapped (Details: ObservationValue code MAPPED = 'mapped'), patient asserted (Details: ObservationValue code PATAST = 'patient asserted')

**clinicalStatus**: Resolved

**verificationStatus**: Confirmed

**category**: Encounter Diagnosis

**severity**: Moderate

**code**: Pulmonary embolism

**subject**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**onset**: 2022-10-23

**abatement**: 2023-03-01

**asserter**: Mattila, Topi Erkki Rikhard Erikoislääkäri



## Resource Content

```json
{
  "resourceType" : "Condition",
  "id" : "2c4dc13c-2927-4cd7-b86e-1a3b89493d2b",
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
      "code" : "59282003",
      "display" : "Pulmonary embolism"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.1",
      "code" : "I26.9",
      "display" : "Keuhkoveritulppa ilman akuuttia keuhkosydänsairautta"
    },
    {
      "system" : "http://hl7.org/fhir/sid/icd-10",
      "code" : "I26.9",
      "display" : "Pulmonary embolism without mention of acute cor pulmonale"
    }],
    "text" : "Pulmonary embolism"
  },
  "subject" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "onsetDateTime" : "2022-10-23",
  "abatementDateTime" : "2023-03-01",
  "asserter" : {
    "display" : "Mattila, Topi Erkki Rikhard Erikoislääkäri"
  }
}

```
