# ImmunizationHepatitisA1 - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ImmunizationHepatitisA1**

## Example Immunization: ImmunizationHepatitisA1

Profiles: [IPA-Immunization](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-immunization.html) version: 1.1.0, [Immunization (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-Immunization-uv-ips.html), [Immunization (EU core)](http://hl7.eu/fhir/base/2.0.0/StructureDefinition-immunization-eu-core.html), [Immunization - Obligations (EPS)](https://build.fhir.org/ig/hl7-eu/eps/StructureDefinition-immunization-obl-eu-eps.html)

Security Labels: device reported (Details: ObservationValue code DEVRPT = 'device reported'), patient reported (Details: ObservationValue code PATRPT = 'patient reported'), syntactic transform (Details: ObservationValue code SYNTAC = 'syntactic transform'), mapped (Details: ObservationValue code MAPPED = 'mapped'), patient asserted (Details: ObservationValue code PATAST = 'patient asserted')

**status**: Completed

**vaccineCode**: Havrix for hepatitis A

**patient**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**occurrence**: 2004-11-02

**manufacturer**: GlaxoSmithCline (GSK)

**doseQuantity**: 1 ml (Details: UCUM codeml = 'ml')

**reasonCode**: Travel vaccinations, Elective immunization for international travel

### ProtocolApplieds

| | | | |
| :--- | :--- | :--- | :--- |
| - | **TargetDisease** | **DoseNumber[x]** | **SeriesDoses[x]** |
| * | Hepatitis A | 1 | 2 |



## Resource Content

```json
{
  "resourceType" : "Immunization",
  "id" : "244fb199-b9b2-49ef-85cd-09e5cdbc83af",
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
      "code" : "871751006",
      "display" : "Hepatitis A vaccine"
    },
    {
      "system" : "http://www.whocc.no/atc",
      "code" : "J07BC02",
      "display" : "hepatitis A, inactivated, whole virus"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.610",
      "code" : "50",
      "display" : "Hepatiitti A -rokote"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.611",
      "code" : "13",
      "display" : "Havrix"
    }],
    "text" : "Havrix for hepatitis A"
  },
  "patient" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "occurrenceDateTime" : "2004-11-02",
  "manufacturer" : {
    "display" : "GlaxoSmithCline (GSK)"
  },
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
        "code" : "40468003",
        "display" : "Viral hepatitis, type A"
      },
      {
        "system" : "http://hl7.org/fhir/sid/icd-10",
        "code" : "B15",
        "display" : "Acute hepatitis A"
      },
      {
        "system" : "urn:oid:1.2.246.537.6.609",
        "code" : "13",
        "display" : "Hepatiitti A -viruksen aiheuttama maksatulehdus"
      }],
      "text" : "Hepatitis A"
    }],
    "doseNumberPositiveInt" : 1,
    "seriesDosesPositiveInt" : 2
  }]
}

```
