# ConditionSight - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ConditionSight**

## Example Condition: ConditionSight

Profiles: [IPA-Condition](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-condition.html) version: 1.1.0, [Condition (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-Condition-uv-ips.html), [Condition (EU core)](http://hl7.eu/fhir/base/2.0.0/StructureDefinition-condition-eu-core.html), [Condition - Obligations (EPS)](https://build.fhir.org/ig/hl7-eu/eps/StructureDefinition-condition-obl-eu-eps.html)

Security Labels: device reported (Details: ObservationValue code DEVRPT = 'device reported'), patient reported (Details: ObservationValue code PATRPT = 'patient reported'), syntactic transform (Details: ObservationValue code SYNTAC = 'syntactic transform'), mapped (Details: ObservationValue code MAPPED = 'mapped'), patient asserted (Details: ObservationValue code PATAST = 'patient asserted')

**clinicalStatus**: Active

**verificationStatus**: Confirmed

**category**: Encounter Diagnosis

**severity**: Mild

**code**: Myopia

**subject**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**onset**: 2016-05-13

**asserter**: Paakkala Liisa



## Resource Content

```json
{
  "resourceType" : "Condition",
  "id" : "af227524-ca64-46ed-8aad-c17f1a712af5",
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
      "code" : "encounter-diagnosis",
      "display" : "Encounter Diagnosis"
    }],
    "text" : "Encounter Diagnosis"
  }],
  "severity" : {
    "coding" : [{
      "system" : "http://snomed.info/sct",
      "code" : "255604002",
      "display" : "Mild"
    }],
    "text" : "Mild"
  },
  "code" : {
    "coding" : [{
      "system" : "http://snomed.info/sct",
      "code" : "232133000",
      "display" : "Simple myopia (disorder)"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.1",
      "code" : "H52.1",
      "display" : "Likitaittoisuus"
    },
    {
      "system" : "http://hl7.org/fhir/sid/icd-10",
      "code" : "H52.1",
      "display" : "Myopia"
    }],
    "text" : "Myopia"
  },
  "subject" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "onsetDateTime" : "2016-05-13",
  "asserter" : {
    "display" : "Paakkala Liisa"
  }
}

```
