# ImmunizationPolio - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ImmunizationPolio**

## Example Immunization: ImmunizationPolio

Profiles: [IPA-Immunization](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-immunization.html) version: 1.1.0, [Immunization (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-Immunization-uv-ips.html), [Immunization (EU core)](http://hl7.eu/fhir/base/2.0.0/StructureDefinition-immunization-eu-core.html), [Immunization - Obligations (EPS)](https://build.fhir.org/ig/hl7-eu/eps/StructureDefinition-immunization-obl-eu-eps.html)

Security Labels: device reported (Details: ObservationValue code DEVRPT = 'device reported'), patient reported (Details: ObservationValue code PATRPT = 'patient reported'), syntactic transform (Details: ObservationValue code SYNTAC = 'syntactic transform'), mapped (Details: ObservationValue code MAPPED = 'mapped'), patient asserted (Details: ObservationValue code PATAST = 'patient asserted')

**status**: Completed

**vaccineCode**: Imovax Polio vaccine

**patient**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**occurrence**: 2011-05-12

**manufacturer**: Sanofi Pasteur

**doseQuantity**: 0.5 ml (Details: UCUM codeml = 'ml')

### ProtocolApplieds

| | | |
| :--- | :--- | :--- |
| - | **TargetDisease** | **DoseNumber[x]** |
| * | Polio | 1 |



## Resource Content

```json
{
  "resourceType" : "Immunization",
  "id" : "f1649cba-fde7-4d54-8fcd-37b6240017ac",
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
      "code" : "871740006",
      "display" : "Inactivated polio vaccine"
    },
    {
      "system" : "http://www.whocc.no/atc",
      "code" : "J07BF03",
      "display" : "poliomyelitis, trivalent, inactivated, whole virus"
    },
    {
      "system" : "http://hl7.org/fhir/sid/cvx",
      "code" : "10",
      "display" : "poliovirus vaccine, inactivated"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.610",
      "code" : "53",
      "display" : "Poliorokote"
    },
    {
      "system" : "urn:oid:1.2.246.537.6.611",
      "code" : "19",
      "display" : "Imovax Polio"
    }],
    "text" : "Imovax Polio vaccine"
  },
  "patient" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "occurrenceDateTime" : "2011-05-12",
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
        "code" : "398102009",
        "display" : "Poliomyelitis"
      },
      {
        "system" : "http://hl7.org/fhir/sid/icd-10",
        "code" : "A80",
        "display" : "Acute poliomyelitis"
      },
      {
        "system" : "urn:oid:1.2.246.537.6.609",
        "code" : "17",
        "display" : "Polio"
      }],
      "text" : "Polio"
    }],
    "doseNumberPositiveInt" : 1
  }]
}

```
