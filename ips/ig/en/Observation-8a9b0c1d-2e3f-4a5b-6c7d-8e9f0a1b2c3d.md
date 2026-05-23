# Observation-lab-fp-fe-1 - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Observation-lab-fp-fe-1**

## Example Observation: Observation-lab-fp-fe-1

Profiles: [IPA-Observation](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-observation.html) version: 1.1.0, [Observation Results - Laboratory/Pathology (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-Observation-results-laboratory-pathology-uv-ips.html), [Observation: Medical Test Result (EU core)](http://hl7.eu/fhir/base/2.0.0/StructureDefinition-medicalTestResult-eu-core.html)

Security Labels: device reported (Details: ObservationValue code DEVRPT = 'device reported'), patient reported (Details: ObservationValue code PATRPT = 'patient reported'), syntactic transform (Details: ObservationValue code SYNTAC = 'syntactic transform'), mapped (Details: ObservationValue code MAPPED = 'mapped'), patient asserted (Details: ObservationValue code PATAST = 'patient asserted'), Artificial Intelligence asserted (Details: ObservationValue code AIAST = 'Artificial Intelligence asserted')

**status**: Final

**category**: Laboratory

**code**: fP-Fe, rauta

**subject**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**effective**: 2024-03-22 10:35:00+0200

**performer**: Fimlab

**value**: 12.1 umol/l (Details: UCUM codeumol/L = 'umol/L')

**interpretation**: Normal

### ReferenceRanges

| | | | |
| :--- | :--- | :--- | :--- |
| - | **Low** | **High** | **Text** |
| * | 9 | 34 | 9-34 umol/l |



## Resource Content

```json
{
  "resourceType" : "Observation",
  "id" : "8a9b0c1d-2e3f-4a5b-6c7d-8e9f0a1b2c3d",
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
      "code" : "14798-3",
      "display" : "Iron [Moles/volume] in Serum or Plasma"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.3",
      "code" : "4529",
      "display" : "fP-Fe"
    }],
    "text" : "fP-Fe, rauta"
  },
  "subject" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "effectiveDateTime" : "2024-03-22T10:35:00+02:00",
  "performer" : [{
    "display" : "Fimlab"
  }],
  "valueQuantity" : {
    "value" : 12.1,
    "unit" : "umol/l",
    "system" : "http://unitsofmeasure.org",
    "code" : "umol/L"
  },
  "interpretation" : [{
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ObservationInterpretation",
      "code" : "N",
      "display" : "Normal"
    }]
  }],
  "referenceRange" : [{
    "low" : {
      "value" : 9
    },
    "high" : {
      "value" : 34
    },
    "text" : "9-34 umol/l"
  }]
}

```
