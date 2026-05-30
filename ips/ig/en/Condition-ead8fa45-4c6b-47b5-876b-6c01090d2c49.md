# ConditionFinger - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ConditionFinger**

## Example Condition: ConditionFinger

Profiles: [IPA-Condition](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-condition.html) version: 1.1.0, [Condition (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-Condition-uv-ips.html), [Condition (EU core)](http://hl7.eu/fhir/base/2.0.0/StructureDefinition-condition-eu-core.html), [Condition - Obligations (EPS)](https://build.fhir.org/ig/hl7-eu/eps/StructureDefinition-condition-obl-eu-eps.html)

Security Labels: [device reported (Details: v3 Code System ObservationValue code DEVRPT = 'device reported')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html), [patient reported (Details: v3 Code System ObservationValue code PATRPT = 'patient reported')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html), [syntactic transform (Details: v3 Code System ObservationValue code SYNTAC = 'syntactic transform')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html), [mapped (Details: v3 Code System ObservationValue code MAPPED = 'mapped')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html), [patient asserted (Details: v3 Code System ObservationValue code PATAST = 'patient asserted')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html)

**clinicalStatus**: Resolved

**verificationStatus**: Confirmed

**category**: Encounter Diagnosis

**severity**: Moderate

**code**: Fracture of left ring finger

**subject**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**onset**: 2017-11-20

**asserter**: Partio, E Nikke Nestor Erikoistuva lääkäri



## Resource Content

```json
{
  "resourceType" : "Condition",
  "id" : "ead8fa45-4c6b-47b5-876b-6c01090d2c49",
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
      "code" : "704094001",
      "display" : "Closed fracture of proximal phalanx of ring finger (disorder)"
    },
    {
      "system" : "http://hl7.org/fhir/sid/icd-10",
      "code" : "S62.6",
      "display" : "Fracture of other finger"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.1",
      "code" : "S62.6",
      "display" : "Muun sormen murtuma"
    },
    {
      "system" : "http://hl7.org/fhir/sid/icd-10",
      "code" : "W09",
      "display" : "Fall involving playground equipment"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.1",
      "code" : "W09",
      "display" : "Kaatuminen tai putoaminen leikkikenttävälineeltä"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.1",
      "code" : "Y94.8",
      "display" : "Muu vapaa-ajan tapaturma"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.31",
      "code" : "L08",
      "display" : "Olkapään oire/vaiva"
    }],
    "text" : "Fracture of left ring finger"
  },
  "subject" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "onsetDateTime" : "2017-11-20",
  "asserter" : {
    "display" : "Partio, E Nikke Nestor Erikoistuva lääkäri"
  }
}

```
