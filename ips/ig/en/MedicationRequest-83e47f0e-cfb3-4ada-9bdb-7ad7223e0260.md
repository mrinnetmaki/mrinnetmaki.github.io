# MedicationRequestRosuvastatin10mg - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **MedicationRequestRosuvastatin10mg**

## Example MedicationRequest: MedicationRequestRosuvastatin10mg

Profiles: [IPA-MedicationRequest](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-medicationrequest.html) version: 1.1.0, [MedicationRequest (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-MedicationRequest-uv-ips.html), [MedicationRequest (EU core)](http://hl7.eu/fhir/base/2.0.0/StructureDefinition-medicationRequest-eu-core.html), [MedicationRequest - Obligations (EPS)](https://build.fhir.org/ig/hl7-eu/eps/StructureDefinition-medicationrequest-obl-eu-eps.html)

Security Labels: device reported (Details: ObservationValue code DEVRPT = 'device reported'), patient reported (Details: ObservationValue code PATRPT = 'patient reported'), syntactic transform (Details: ObservationValue code SYNTAC = 'syntactic transform'), mapped (Details: ObservationValue code MAPPED = 'mapped'), patient asserted (Details: ObservationValue code PATAST = 'patient asserted')

**status**: Active

**intent**: Instance Order

**category**: Active ambulatory use

**medication**: [Rosuvastatin 10 mg](Bundle-IpsBundle.md#urn-uuid-1af60d57-5a04-42d4-b63e-f509652c57f2)

**subject**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**reasonCode**: Hypercholesterolemia

**reasonReference**: [Diabetes related hypercholesterolemia](Bundle-IpsBundle.md#urn-uuid-c279fd61-c4da-406b-a14b-b6166b956f83)

**courseOfTherapyType**: Continuous long term therapy

> **dosageInstruction****text**: 1 tabletti iltaisin Kolesterolilääke**patientInstruction**: 1 tabletti iltaisin Kolesterolilääke

### DoseAndRates

| | |
| :--- | :--- |
| - | **Rate[x]** |
| * | 10 mg/day (Details: UCUM codemg/d = 'mg/d') |


### DispenseRequests

| | |
| :--- | :--- |
| - | **ValidityPeriod** |
| * | 2024-12-20 --> 2026-12-20 |



## Resource Content

```json
{
  "resourceType" : "MedicationRequest",
  "id" : "83e47f0e-cfb3-4ada-9bdb-7ad7223e0260",
  "meta" : {
    "profile" : ["http://hl7.org/fhir/uv/ipa/StructureDefinition/ipa-medicationrequest|1.1.0",
    "http://hl7.org/fhir/uv/ips/StructureDefinition/MedicationRequest-uv-ips",
    "http://hl7.eu/fhir/base/StructureDefinition/medicationRequest-eu-core",
    "http://hl7.eu/fhir/eps/StructureDefinition/medicationrequest-obl-eu-eps"],
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
  "status" : "active",
  "intent" : "instance-order",
  "category" : [{
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/medicationrequest-category",
      "code" : "community",
      "display" : "Community"
    },
    {
      "system" : "http://snomed.info/sct",
      "code" : "360270004",
      "display" : "Therapy - action"
    },
    {
      "system" : "http://terminology.hl7.org/CodeSystem/medicationrequest-admin-location",
      "code" : "community",
      "display" : "Community"
    }],
    "text" : "Active ambulatory use"
  }],
  "medicationReference" : {
    "reference" : "urn:uuid:1af60d57-5a04-42d4-b63e-f509652c57f2",
    "display" : "Rosuvastatin 10 mg"
  },
  "subject" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "reasonCode" : [{
    "coding" : [{
      "system" : "http://snomed.info/sct",
      "code" : "13644009",
      "display" : "Hypercholesterolemia (disorder)"
    },
    {
      "system" : "http://hl7.org/fhir/sid/icd-10",
      "code" : "E78.0",
      "display" : "Pure hypercholesterolaemia"
    }],
    "text" : "Hypercholesterolemia"
  }],
  "reasonReference" : [{
    "reference" : "urn:uuid:c279fd61-c4da-406b-a14b-b6166b956f83",
    "display" : "Diabetes related hypercholesterolemia"
  }],
  "courseOfTherapyType" : {
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/medicationrequest-course-of-therapy",
      "code" : "continuous",
      "display" : "Continuous long term therapy"
    }]
  },
  "dosageInstruction" : [{
    "text" : "1 tabletti iltaisin Kolesterolilääke",
    "patientInstruction" : "1 tabletti iltaisin Kolesterolilääke",
    "doseAndRate" : [{
      "rateQuantity" : {
        "value" : 10,
        "unit" : "mg/day",
        "system" : "http://unitsofmeasure.org",
        "code" : "mg/d"
      }
    }]
  }],
  "dispenseRequest" : {
    "validityPeriod" : {
      "start" : "2024-12-20",
      "end" : "2026-12-20"
    }
  }
}

```
