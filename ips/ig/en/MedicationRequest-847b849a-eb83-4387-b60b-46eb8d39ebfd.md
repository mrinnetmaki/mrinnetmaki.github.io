# MedicationRequestInsulinNovorapid - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **MedicationRequestInsulinNovorapid**

## Example MedicationRequest: MedicationRequestInsulinNovorapid

Profiles: [IPA-MedicationRequest](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-medicationrequest.html) version: 1.1.0, [MedicationRequest (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-MedicationRequest-uv-ips.html), [MedicationRequest (EU core)](http://hl7.eu/fhir/base/2.0.0/StructureDefinition-medicationRequest-eu-core.html), [MedicationRequest - Obligations (EPS)](https://build.fhir.org/ig/hl7-eu/eps/StructureDefinition-medicationrequest-obl-eu-eps.html)

Security Labels: [device reported (Details: v3 Code System ObservationValue code DEVRPT = 'device reported')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html), [patient reported (Details: v3 Code System ObservationValue code PATRPT = 'patient reported')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html), [syntactic transform (Details: v3 Code System ObservationValue code SYNTAC = 'syntactic transform')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html), [mapped (Details: v3 Code System ObservationValue code MAPPED = 'mapped')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html), [patient asserted (Details: v3 Code System ObservationValue code PATAST = 'patient asserted')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html)

**status**: Active

**intent**: Instance Order

**category**: Active ambulatory use

**medication**: [Insulin NovoRapid 100 units/ml](Bundle-IpsBundle.md#urn-uuid-e6f153f4-6188-4dc4-9f19-f4179b9ee720)

**subject**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**reasonCode**: Type 1 diabetes mellitus

**reasonReference**: [Type 1 diabetes mellitus](Bundle-IpsBundle.md#urn-uuid-1558c456-efa1-4b3d-abe2-1522c6048bc7)

**courseOfTherapyType**: Continuous long term therapy

> **dosageInstruction****text**: 50-100 yksikköä vuorokaudessa, Pumpcart säiliöt insuliinipumppuun ihon alle DMI**patientInstruction**: 50-100 yksikköä vuorokaudessa, Pumpcart säiliöt insuliinipumppuun ihon alle DMI

### DoseAndRates

| | |
| :--- | :--- |
| - | **Rate[x]** |
| * | 50-100 units per day |




## Resource Content

```json
{
  "resourceType" : "MedicationRequest",
  "id" : "847b849a-eb83-4387-b60b-46eb8d39ebfd",
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
    "reference" : "urn:uuid:e6f153f4-6188-4dc4-9f19-f4179b9ee720",
    "display" : "Insulin NovoRapid 100 units/ml"
  },
  "subject" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "reasonCode" : [{
    "coding" : [{
      "system" : "http://snomed.info/sct",
      "code" : "46635009",
      "display" : "Type 1 diabetes mellitus"
    },
    {
      "system" : "http://hl7.org/fhir/sid/icd-10",
      "code" : "E10",
      "display" : "Type 1 diabetes mellitus"
    }],
    "text" : "Type 1 diabetes mellitus"
  }],
  "reasonReference" : [{
    "reference" : "urn:uuid:1558c456-efa1-4b3d-abe2-1522c6048bc7",
    "display" : "Type 1 diabetes mellitus"
  }],
  "courseOfTherapyType" : {
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/medicationrequest-course-of-therapy",
      "code" : "continuous",
      "display" : "Continuous long term therapy"
    }]
  },
  "dosageInstruction" : [{
    "text" : "50-100 yksikköä vuorokaudessa, Pumpcart säiliöt insuliinipumppuun ihon alle DMI",
    "patientInstruction" : "50-100 yksikköä vuorokaudessa, Pumpcart säiliöt insuliinipumppuun ihon alle DMI",
    "doseAndRate" : [{
      "rateRange" : {
        "low" : {
          "value" : 50,
          "unit" : "units per day",
          "system" : "http://unitsofmeasure.org",
          "code" : "[iU]/d"
        },
        "high" : {
          "value" : 100,
          "unit" : "units per day",
          "system" : "http://unitsofmeasure.org",
          "code" : "[iU]/d"
        }
      }
    }]
  }]
}

```
