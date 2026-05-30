# Observation-lab-p-luakrvv-1 - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Observation-lab-p-luakrvv-1**

## Example Observation: Observation-lab-p-luakrvv-1

Profiles: [IPA-Observation](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-observation.html) version: 1.1.0, [Observation Results - Laboratory/Pathology (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-Observation-results-laboratory-pathology-uv-ips.html), [Observation: Medical Test Result (EU core)](http://hl7.eu/fhir/base/2.0.0/StructureDefinition-medicalTestResult-eu-core.html)

Security Labels: [device reported (Details: v3 Code System ObservationValue code DEVRPT = 'device reported')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html), [patient reported (Details: v3 Code System ObservationValue code PATRPT = 'patient reported')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html), [syntactic transform (Details: v3 Code System ObservationValue code SYNTAC = 'syntactic transform')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html), [mapped (Details: v3 Code System ObservationValue code MAPPED = 'mapped')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html), [patient asserted (Details: v3 Code System ObservationValue code PATAST = 'patient asserted')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html), [Artificial Intelligence asserted (Details: v3 Code System ObservationValue code AIAST = 'Artificial Intelligence asserted')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html)

**status**: Final

**category**: Laboratory

**code**: P -LuakRVV, lupusantikoagulantti, dRVVT

**subject**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**effective**: 2023-04-27 17:30:00+0300

**performer**: Fimlab

**value**: 0.94 suhde (Details: UCUM code1 = '1')

**interpretation**: Normal

### ReferenceRanges

| | | |
| :--- | :--- | :--- |
| - | **High** | **Text** |
| * | 1.16 | -1.16 Suhde |



## Resource Content

```json
{
  "resourceType" : "Observation",
  "id" : "a0b1c2d3-e4f5-6a7b-8c9d-e0f1a2b3c4d5",
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
    },
    {
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ObservationValue",
      "code" : "AIAST",
      "display" : "Artificial Intelligence asserted"
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
      "extension" : [{
        "url" : "http://hl7.org/fhir/uv/security-label-ds4p/StructureDefinition/extension-inline-sec-label",
        "valueCoding" : {
          "system" : "http://terminology.hl7.org/CodeSystem/v3-ObservationValue",
          "code" : "AIAST",
          "display" : "Artificial Intelligence asserted"
        }
      },
      {
        "url" : "http://hl7.org/fhir/uv/security-label-ds4p/StructureDefinition/extension-inline-sec-label",
        "valueCoding" : {
          "system" : "http://terminology.hl7.org/CodeSystem/v3-ObservationValue",
          "code" : "PATAST",
          "display" : "patient asserted"
        }
      }],
      "system" : "http://loinc.org",
      "code" : "50410-0",
      "display" : "dRVVT/dRVVT W excess phospholipid (screen to confirm ratio)"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.3",
      "code" : "4425",
      "display" : "P -LuakRVV"
    }],
    "text" : "P -LuakRVV, lupusantikoagulantti, dRVVT"
  },
  "subject" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "effectiveDateTime" : "2023-04-27T17:30:00+03:00",
  "performer" : [{
    "display" : "Fimlab"
  }],
  "valueQuantity" : {
    "value" : 0.94,
    "unit" : "suhde",
    "system" : "http://unitsofmeasure.org",
    "code" : "1"
  },
  "interpretation" : [{
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ObservationInterpretation",
      "code" : "N",
      "display" : "Normal"
    }]
  }],
  "referenceRange" : [{
    "high" : {
      "value" : 1.16
    },
    "text" : "-1.16 Suhde"
  }]
}

```
