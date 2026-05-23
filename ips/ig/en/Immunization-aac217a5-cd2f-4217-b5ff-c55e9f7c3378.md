# ImmunizationCovid3 - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ImmunizationCovid3**

## Example Immunization: ImmunizationCovid3

Profiles: [IPA-Immunization](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-immunization.html) version: 1.1.0, [Immunization (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-Immunization-uv-ips.html), [Immunization (EU core)](http://hl7.eu/fhir/base/2.0.0/StructureDefinition-immunization-eu-core.html), [Immunization - Obligations (EPS)](https://build.fhir.org/ig/hl7-eu/eps/StructureDefinition-immunization-obl-eu-eps.html)

Security Labels: device reported (Details: ObservationValue code DEVRPT = 'device reported'), patient reported (Details: ObservationValue code PATRPT = 'patient reported'), syntactic transform (Details: ObservationValue code SYNTAC = 'syntactic transform'), mapped (Details: ObservationValue code MAPPED = 'mapped'), patient asserted (Details: ObservationValue code PATAST = 'patient asserted')

**status**: Completed

**vaccineCode**: Moderna Spikevax covid-19 mRNA vaccine

**patient**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**occurrence**: 2022-01-17

**manufacturer**: Moderna

**doseQuantity**: 0.25 ml (Details: UCUM codeml = 'ml')

### ProtocolApplieds

| | | |
| :--- | :--- | :--- |
| - | **TargetDisease** | **DoseNumber[x]** |
| * | Covid-19 | 1 |



## Resource Content

```json
{
  "resourceType" : "Immunization",
  "id" : "aac217a5-cd2f-4217-b5ff-c55e9f7c3378",
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
      "code" : "1119349007",
      "display" : "COVID-19 mRNA vaccine"
    },
    {
      "system" : "http://www.whocc.no/atc",
      "code" : "J07BN01",
      "display" : "covid-19, RNA-based vaccine"
    },
    {
      "system" : "http://hl7.org/fhir/sid/cvx",
      "code" : "519",
      "display" : "COVID-19 mRNA, bivalent, original/Omicron BA.1, Non-US Vaccine (Spikevax Bivalent), Moderna"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.610",
      "code" : "59",
      "display" : "COVID-19-rokote"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.611",
      "code" : "142",
      "display" : "Spikevax"
    }],
    "text" : "Moderna Spikevax covid-19 mRNA vaccine"
  },
  "patient" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "occurrenceDateTime" : "2022-01-17",
  "manufacturer" : {
    "display" : "Moderna"
  },
  "doseQuantity" : {
    "value" : 0.25,
    "unit" : "ml",
    "system" : "http://unitsofmeasure.org",
    "code" : "ml"
  },
  "protocolApplied" : [{
    "targetDisease" : [{
      "coding" : [{
        "system" : "http://snomed.info/sct",
        "code" : "840539006",
        "display" : "Disease caused by severe acute respiratory syndrome coronavirus 2"
      },
      {
        "system" : "http://hl7.org/fhir/sid/icd-10",
        "code" : "U07.2",
        "display" : "COVID-19, virus not identified"
      },
      {
        "system" : "urn:oid:1.2.246.537.6.609",
        "code" : "29",
        "display" : "COVID-19-tauti"
      }],
      "text" : "Covid-19"
    }],
    "doseNumberPositiveInt" : 1
  }]
}

```
