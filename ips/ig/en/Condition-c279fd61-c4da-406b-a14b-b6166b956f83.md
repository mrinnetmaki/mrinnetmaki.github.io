# ConditionHypercholesterolemia - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ConditionHypercholesterolemia**

## Example Condition: ConditionHypercholesterolemia

Profiles: [IPA-Condition](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-condition.html) version: 1.1.0, [IPA-problem-list-item](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-problem-list-item.html) version: 1.1.0, [Condition (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-Condition-uv-ips.html), [Condition - Obligations (EPS)](https://build.fhir.org/ig/hl7-eu/eps/StructureDefinition-condition-obl-eu-eps.html)

Security Labels: patient reported (Details: ObservationValue code PATRPT = 'patient reported'), patient asserted (Details: ObservationValue code PATAST = 'patient asserted')

**clinicalStatus**: Active

**verificationStatus**: Confirmed

**category**: Problem List Item

**severity**: Mild

**code**: Hypercholesterolemia

**subject**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**onset**: 2023-12-18

**note**: By urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f

> 

The guidelines for dyslipidemia categorize people who have lived with type 1 diabetes for more than 10 years into 'high risk' class where the LDL target is < 1.8 mmol/l. For those with additional risk factors (I have mild retinopathy and a past event of pulmonary embolism) the LDL target is < 1.4 mmol/l.




## Resource Content

```json
{
  "resourceType" : "Condition",
  "id" : "c279fd61-c4da-406b-a14b-b6166b956f83",
  "meta" : {
    "profile" : ["http://hl7.org/fhir/uv/ipa/StructureDefinition/ipa-condition|1.1.0",
    "http://hl7.org/fhir/uv/ipa/StructureDefinition/ipa-problem-list-item|1.1.0",
    "http://hl7.org/fhir/uv/ips/StructureDefinition/Condition-uv-ips",
    "http://hl7.eu/fhir/eps/StructureDefinition/condition-obl-eu-eps"],
    "security" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ObservationValue",
      "code" : "PATRPT",
      "display" : "patient reported"
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
      "code" : "255604002",
      "display" : "Mild"
    }],
    "text" : "Mild"
  },
  "code" : {
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
  },
  "subject" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "onsetDateTime" : "2023-12-18",
  "note" : [{
    "authorReference" : {
      "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
      "display" : "Mikael Rinnetmäki, the patient"
    },
    "text" : "The guidelines for dyslipidemia categorize people who have lived with type 1 diabetes for more than 10 years into 'high risk' class where the LDL target is < 1.8 mmol/l. For those with additional risk factors (I have mild retinopathy and a past event of pulmonary embolism) the LDL target is < 1.4 mmol/l."
  }]
}

```
