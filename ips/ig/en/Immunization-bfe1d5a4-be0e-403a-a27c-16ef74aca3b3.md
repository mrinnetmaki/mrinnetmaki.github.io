# ImmunizationInfluenza5 - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ImmunizationInfluenza5**

## Example Immunization: ImmunizationInfluenza5

Profiles: [IPA-Immunization](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-immunization.html) version: 1.1.0, [Immunization (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-Immunization-uv-ips.html), [Immunization (EU core)](http://hl7.eu/fhir/base/2.0.0/StructureDefinition-immunization-eu-core.html), [Immunization - Obligations (EPS)](https://build.fhir.org/ig/hl7-eu/eps/StructureDefinition-immunization-obl-eu-eps.html)

Security Labels: [device reported (Details: v3 Code System ObservationValue code DEVRPT = 'device reported')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html), [patient reported (Details: v3 Code System ObservationValue code PATRPT = 'patient reported')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html), [syntactic transform (Details: v3 Code System ObservationValue code SYNTAC = 'syntactic transform')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html), [mapped (Details: v3 Code System ObservationValue code MAPPED = 'mapped')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html), [patient asserted (Details: v3 Code System ObservationValue code PATAST = 'patient asserted')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html)

**status**: Completed

**vaccineCode**: VaxigripTetra vaccine for influenza

**patient**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**occurrence**: 2023-12-20

**manufacturer**: Sanofi Pasteur

**doseQuantity**: 0.5 ml (Details: UCUM codeml = 'ml')

### ProtocolApplieds

| | | |
| :--- | :--- | :--- |
| - | **TargetDisease** | **DoseNumber[x]** |
| * | Influenza | 1 |



## Resource Content

```json
{
  "resourceType" : "Immunization",
  "id" : "bfe1d5a4-be0e-403a-a27c-16ef74aca3b3",
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
      "code" : "1181000221105",
      "display" : "Influenza vaccine"
    },
    {
      "system" : "http://www.whocc.no/atc",
      "code" : "J07BB02",
      "display" : "influenza, inactivated, split virus or surface antigen"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.610",
      "code" : "48",
      "display" : "Influenssarokote"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.611",
      "code" : "122",
      "display" : "VaxigripTetra"
    }],
    "text" : "VaxigripTetra vaccine for influenza"
  },
  "patient" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "occurrenceDateTime" : "2023-12-20",
  "manufacturer" : {
    "display" : "Sanofi Pasteur"
  },
  "doseQuantity" : {
    "value" : 0.5,
    "unit" : "ml",
    "system" : "http://unitsofmeasure.org",
    "code" : "ml"
  },
  "protocolApplied" : [{
    "targetDisease" : [{
      "coding" : [{
        "system" : "http://snomed.info/sct",
        "code" : "6142004",
        "display" : "Influenza"
      },
      {
        "system" : "http://hl7.org/fhir/sid/icd-10",
        "code" : "J11",
        "display" : "Influenza, virus not identified"
      },
      {
        "system" : "urn:oid:1.2.246.537.6.609",
        "code" : "12",
        "display" : "Influenssa"
      }],
      "text" : "Influenza"
    }],
    "doseNumberPositiveInt" : 1
  }]
}

```
