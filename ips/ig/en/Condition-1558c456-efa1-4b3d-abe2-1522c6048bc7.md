# ConditionDiabetesT1 - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ConditionDiabetesT1**

## Example Condition: ConditionDiabetesT1

Profiles: [IPA-Condition](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-condition.html) version: 1.1.0, [IPA-problem-list-item](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-problem-list-item.html) version: 1.1.0, [Condition (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-Condition-uv-ips.html), [Condition (EU core)](http://hl7.eu/fhir/base/2.0.0/StructureDefinition-condition-eu-core.html), [Condition - Obligations (EPS)](https://build.fhir.org/ig/hl7-eu/eps/StructureDefinition-condition-obl-eu-eps.html)

Security Labels: device reported (Details: ObservationValue code DEVRPT = 'device reported'), patient reported (Details: ObservationValue code PATRPT = 'patient reported'), syntactic transform (Details: ObservationValue code SYNTAC = 'syntactic transform'), mapped (Details: ObservationValue code MAPPED = 'mapped'), patient asserted (Details: ObservationValue code PATAST = 'patient asserted')

**clinicalStatus**: Active

**verificationStatus**: Confirmed

**category**: Problem List Item

**severity**: Severe

**code**: Type 1 diabetes mellitus

**subject**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**onset**: 1999-04

**note**: By urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f

> 

I wear an automated insulin delivery system.




## Resource Content

```json
{
  "resourceType" : "Condition",
  "id" : "1558c456-efa1-4b3d-abe2-1522c6048bc7",
  "meta" : {
    "profile" : ["http://hl7.org/fhir/uv/ipa/StructureDefinition/ipa-condition|1.1.0",
    "http://hl7.org/fhir/uv/ipa/StructureDefinition/ipa-problem-list-item|1.1.0",
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
      "code" : "active",
      "display" : "Active"
    }],
    "text" : "Active"
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
      "code" : "problem-list-item",
      "display" : "Problem List Item"
    },
    {
      "system" : "http://terminology.hl7.org/CodeSystem/condition-category",
      "code" : "encounter-diagnosis",
      "display" : "Encounter Diagnosis"
    }],
    "text" : "Problem List Item"
  }],
  "severity" : {
    "coding" : [{
      "system" : "http://snomed.info/sct",
      "code" : "24484000",
      "display" : "Severe"
    }],
    "text" : "Severe"
  },
  "code" : {
    "coding" : [{
      "system" : "http://snomed.info/sct",
      "code" : "46635009",
      "display" : "Type 1 diabetes mellitus"
    },
    {
      "system" : "http://hl7.org/fhir/sid/icd-10",
      "code" : "E10",
      "display" : "Type 1 diabetes mellitus"
    },
    {
      "system" : "http://id.who.int/icd/release/11/mms",
      "code" : "5A10",
      "display" : "Type 1 diabetes mellitus"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.1",
      "code" : "E10",
      "display" : "Nuoruustyypin diabetes"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.31",
      "code" : "T89",
      "display" : "Diabetes, tyyppi 1"
    },
    {
      "system" : "http://hl7.org/fhir/sid/icpc-2",
      "code" : "T89",
      "display" : "Diabetes insulin dependent"
    },
    {
      "system" : "http://terminology.hl7.org/CodeSystem/ICPC-3",
      "code" : "TD71",
      "display" : "Type 1 diabetes mellitus"
    },
    {
      "system" : "http://hl7.org/fhir/sid/icpc-1",
      "code" : "T90",
      "display" : "Diabetes Mellitus"
    }],
    "text" : "Type 1 diabetes mellitus"
  },
  "subject" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "onsetDateTime" : "1999-04",
  "note" : [{
    "authorReference" : {
      "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
      "display" : "Mikael Rinnetmäki, the patient"
    },
    "text" : "I wear an automated insulin delivery system."
  }]
}

```
