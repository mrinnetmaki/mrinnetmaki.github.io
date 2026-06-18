# Observation-lab-s-ttgaba-1 - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Observation-lab-s-ttgaba-1**

## Example Observation: Observation-lab-s-ttgaba-1

Profiles: [IPA-Observation](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-observation.html) version: 1.1.0, [Observation Results - Laboratory/Pathology (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-Observation-results-laboratory-pathology-uv-ips.html), [Observation: Medical Test Result (EU core)](http://hl7.eu/fhir/base/2.0.0/StructureDefinition-medicalTestResult-eu-core.html)

Security Labels: [device reported (Details: ObservationValue code DEVRPT = 'device reported')](http://terminology.hl7.org/7.2.0/CodeSystem-v3-ObservationValue.html), [patient reported (Details: ObservationValue code PATRPT = 'patient reported')](http://terminology.hl7.org/7.2.0/CodeSystem-v3-ObservationValue.html), [syntactic transform (Details: ObservationValue code SYNTAC = 'syntactic transform')](http://terminology.hl7.org/7.2.0/CodeSystem-v3-ObservationValue.html), [mapped (Details: ObservationValue code MAPPED = 'mapped')](http://terminology.hl7.org/7.2.0/CodeSystem-v3-ObservationValue.html), [patient asserted (Details: ObservationValue code PATAST = 'patient asserted')](http://terminology.hl7.org/7.2.0/CodeSystem-v3-ObservationValue.html)

**status**: Final

**category**: Laboratory

**code**: S -tTGAbA (kudostransglutaminaasi, IgA-vasta-aineet)

**subject**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**effective**: 2026-05-22 14:40:00+0300

**performer**: Fimlab

**value**: 0.9 kU/l (Details: UCUM codekU/l = 'kU/l')

**interpretation**: Normal

### ReferenceRanges

| | | | |
| :--- | :--- | :--- | :--- |
| - | **Low** | **High** | **Text** |
| * | 0 | 7 | 0.0-7.0 kU/l |



## Resource Content

```json
{
  "resourceType" : "Observation",
  "id" : "019e4fb3-2100-7add-bf63-941525b5e5bb",
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
          "code" : "PATAST",
          "display" : "patient asserted"
        }
      }],
      "system" : "http://loinc.org",
      "code" : "31017-7",
      "display" : "Tissue transglutaminase IgA Ab [Units/volume] in Serum"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.3",
      "code" : "1885",
      "display" : "S -tTGAbA"
    }],
    "text" : "S -tTGAbA (kudostransglutaminaasi, IgA-vasta-aineet)"
  },
  "subject" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "effectiveDateTime" : "2026-05-22T14:40:00+03:00",
  "performer" : [{
    "display" : "Fimlab"
  }],
  "valueQuantity" : {
    "value" : 0.9,
    "unit" : "kU/l",
    "system" : "http://unitsofmeasure.org",
    "code" : "kU/l"
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
      "value" : 0
    },
    "high" : {
      "value" : 7
    },
    "text" : "0.0-7.0 kU/l"
  }]
}

```
