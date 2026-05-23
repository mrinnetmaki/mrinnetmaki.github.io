# MedicationStatementInsulinNovorapid - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **MedicationStatementInsulinNovorapid**

## Example MedicationStatement: MedicationStatementInsulinNovorapid

Profiles: [IPA-MedicationStatement](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-medicationstatement.html) version: 1.1.0, [MedicationStatement (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-MedicationStatement-uv-ips.html), [MedicationStatement (EU core)](http://hl7.eu/fhir/base/2.0.0/StructureDefinition-medicationStatement-eu-core.html), [MedicationStatement (EPS)](https://build.fhir.org/ig/hl7-eu/eps/StructureDefinition-MedicationStatement-eu-eps.html)

Security Labels: device reported (Details: ObservationValue code DEVRPT = 'device reported'), patient reported (Details: ObservationValue code PATRPT = 'patient reported'), syntactic transform (Details: ObservationValue code SYNTAC = 'syntactic transform'), mapped (Details: ObservationValue code MAPPED = 'mapped'), patient asserted (Details: ObservationValue code PATAST = 'patient asserted')

**basedOn**: [Prescription for Insulin Novorapid](Bundle-IpsBundle.md#urn-uuid-847b849a-eb83-4387-b60b-46eb8d39ebfd)

**status**: active

**category**: Active ambulatory use

**medication**: [Insulin NovoRapid 100 units/ml](Bundle-IpsBundle.md#urn-uuid-e6f153f4-6188-4dc4-9f19-f4179b9ee720)

**subject**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**effective**: 2023-10-06 --> (ongoing)

**informationSource**: [Mikael Rinnetmäki, the patient](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**reasonCode**: Type 1 diabetes mellitus

**reasonReference**: [Type 1 diabetes mellitus](Bundle-IpsBundle.md#urn-uuid-1558c456-efa1-4b3d-abe2-1522c6048bc7)

**note**: By urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f

> 

My prescription is for 50 - 100 iU/d. I usually consume 40 to 70 iU per day.


> **dosage****text**: 40-70 iU/d

### DoseAndRates

| | |
| :--- | :--- |
| - | **Rate[x]** |
| * | 40-70 units per day |




## Resource Content

```json
{
  "resourceType" : "MedicationStatement",
  "id" : "bb2d0be6-24fd-4e1f-8fa4-10e058ed2775",
  "meta" : {
    "profile" : ["http://hl7.org/fhir/uv/ipa/StructureDefinition/ipa-medicationstatement|1.1.0",
    "http://hl7.org/fhir/uv/ips/StructureDefinition/MedicationStatement-uv-ips",
    "http://hl7.eu/fhir/base/StructureDefinition/medicationStatement-eu-core",
    "http://hl7.eu/fhir/eps/StructureDefinition/MedicationStatement-eu-eps"],
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
  "basedOn" : [{
    "reference" : "urn:uuid:847b849a-eb83-4387-b60b-46eb8d39ebfd",
    "display" : "Prescription for Insulin Novorapid"
  }],
  "status" : "active",
  "category" : {
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/medication-statement-category",
      "code" : "community",
      "display" : "Community"
    },
    {
      "system" : "http://snomed.info/sct",
      "code" : "360270004",
      "display" : "Therapy - action"
    }],
    "text" : "Active ambulatory use"
  },
  "medicationReference" : {
    "reference" : "urn:uuid:e6f153f4-6188-4dc4-9f19-f4179b9ee720",
    "display" : "Insulin NovoRapid 100 units/ml"
  },
  "subject" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "effectivePeriod" : {
    "start" : "2023-10-06"
  },
  "informationSource" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki, the patient"
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
  "note" : [{
    "authorReference" : {
      "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
      "display" : "Mikael Rinnetmäki, the patient"
    },
    "text" : "My prescription is for 50 - 100 iU/d. I usually consume 40 to 70 iU per day."
  }],
  "dosage" : [{
    "text" : "40-70 iU/d",
    "doseAndRate" : [{
      "rateRange" : {
        "low" : {
          "value" : 40,
          "unit" : "units per day",
          "system" : "http://unitsofmeasure.org",
          "code" : "[iU]/d"
        },
        "high" : {
          "value" : 70,
          "unit" : "units per day",
          "system" : "http://unitsofmeasure.org",
          "code" : "[iU]/d"
        }
      }
    }]
  }]
}

```
