# ImmunizationHepatitisB1 - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ImmunizationHepatitisB1**

## Example Immunization: ImmunizationHepatitisB1

Profiles: [IPA-Immunization](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-immunization.html) version: 1.1.0, [Immunization (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-Immunization-uv-ips.html), [Immunization (EU core)](http://hl7.eu/fhir/base/2.0.0/StructureDefinition-immunization-eu-core.html), [Immunization - Obligations (EPS)](https://build.fhir.org/ig/hl7-eu/eps/StructureDefinition-immunization-obl-eu-eps.html)

Security Labels: device reported (Details: ObservationValue code DEVRPT = 'device reported'), patient reported (Details: ObservationValue code PATRPT = 'patient reported'), syntactic transform (Details: ObservationValue code SYNTAC = 'syntactic transform'), mapped (Details: ObservationValue code MAPPED = 'mapped'), patient asserted (Details: ObservationValue code PATAST = 'patient asserted')

**status**: Completed

**vaccineCode**: Engerix-B for hepatitis B

**patient**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**occurrence**: 2010-10-25

**manufacturer**: GlaxoSmithKline Biologicals s.a. (GSK)

**lotNumber**: AHBVB649AG

**doseQuantity**: 1 ml (Details: UCUM codeml = 'ml')

**reasonCode**: Travel vaccinations, Elective immunization for international travel

### ProtocolApplieds

| | | | |
| :--- | :--- | :--- | :--- |
| - | **TargetDisease** | **DoseNumber[x]** | **SeriesDoses[x]** |
| * | Hepatitis B | 1 | 3 |



## Resource Content

```json
{
  "resourceType" : "Immunization",
  "id" : "a0ca2399-1f86-487b-ad6c-3e64081ae945",
  "meta" : {
    "profile" : ["http://hl7.org/fhir/uv/ipa/StructureDefinition/ipa-immunization|1.1.0",
    "http://hl7.org/fhir/uv/ips/StructureDefinition/Immunization-uv-ips",
    "http://hl7.eu/fhir/base/StructureDefinition/immunization-eu-core",
    "http://hl7.eu/fhir/eps/StructureDefinition/immunization-obl-eu-eps"],
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
  "status" : "completed",
  "vaccineCode" : {
    "coding" : [{
      "system" : "http://snomed.info/sct",
      "code" : "871822003",
      "display" : "Hepatitis B vaccine"
    },
    {
      "system" : "http://www.whocc.no/atc",
      "code" : "J07BC01",
      "display" : "hepatitis B, purified antigen"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.610",
      "code" : "49",
      "display" : "Hepatiitti B -rokote"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.611",
      "code" : "10",
      "display" : "Engerix-B"
    }],
    "text" : "Engerix-B for hepatitis B"
  },
  "patient" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "occurrenceDateTime" : "2010-10-25",
  "manufacturer" : {
    "display" : "GlaxoSmithKline Biologicals s.a. (GSK)"
  },
  "lotNumber" : "AHBVB649AG",
  "doseQuantity" : {
    "value" : 1,
    "unit" : "ml",
    "system" : "http://unitsofmeasure.org",
    "code" : "ml"
  },
  "reasonCode" : [{
    "coding" : [{
      "system" : "http://snomed.info/sct",
      "code" : "281657000",
      "display" : "Travel vaccinations"
    }]
  },
  {
    "coding" : [{
      "system" : "http://snomed.info/sct",
      "code" : "14747002",
      "display" : "Elective immunization for international travel"
    }]
  }],
  "protocolApplied" : [{
    "targetDisease" : [{
      "coding" : [{
        "system" : "http://snomed.info/sct",
        "code" : "66071002",
        "display" : "Type B viral hepatitis"
      },
      {
        "system" : "http://hl7.org/fhir/sid/icd-10",
        "code" : "B16",
        "display" : "Acute hepatitis B"
      },
      {
        "system" : "urn:oid:1.2.246.537.6.609",
        "code" : "14",
        "display" : "Hepatiitti B -viruksen aiheuttama maksatulehdus"
      }],
      "text" : "Hepatitis B"
    }],
    "doseNumberPositiveInt" : 1,
    "seriesDosesPositiveInt" : 3
  }]
}

```
