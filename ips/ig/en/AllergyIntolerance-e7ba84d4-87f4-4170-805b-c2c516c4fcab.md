# AllergyIntoleranceMedicationNoKnown - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **AllergyIntoleranceMedicationNoKnown**

## Example AllergyIntolerance: AllergyIntoleranceMedicationNoKnown

Profiles: [IPA-AllergyIntolerance](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-allergyintolerance.html) version: 1.1.0, [AllergyIntolerance (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-AllergyIntolerance-uv-ips.html), [AllergyIntolerance (EU core)](http://hl7.eu/fhir/base/2.0.0/StructureDefinition-allergyIntolerance-eu-core.html), [AllergyIntolerance - Obligations (EPS)](https://build.fhir.org/ig/hl7-eu/eps/StructureDefinition-allergyintolerance-obl-eu-eps.html)

Security Labels: patient reported (Details: ObservationValue code PATRPT = 'patient reported'), patient asserted (Details: ObservationValue code PATAST = 'patient asserted')

**clinicalStatus**: Active

**verificationStatus**: Unconfirmed

**type**: Allergy

**category**: Medication

**code**: No known medication allergies

**patient**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)



## Resource Content

```json
{
  "resourceType" : "AllergyIntolerance",
  "id" : "e7ba84d4-87f4-4170-805b-c2c516c4fcab",
  "meta" : {
    "profile" : ["http://hl7.org/fhir/uv/ipa/StructureDefinition/ipa-allergyintolerance|1.1.0",
    "http://hl7.org/fhir/uv/ips/StructureDefinition/AllergyIntolerance-uv-ips",
    "http://hl7.eu/fhir/base/StructureDefinition/allergyIntolerance-eu-core",
    "http://hl7.eu/fhir/eps/StructureDefinition/allergyintolerance-obl-eu-eps"],
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
      "system" : "http://terminology.hl7.org/CodeSystem/allergyintolerance-clinical",
      "code" : "active",
      "display" : "Active"
    }],
    "text" : "Active"
  },
  "verificationStatus" : {
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/allergyintolerance-verification",
      "code" : "unconfirmed",
      "display" : "Unconfirmed"
    }],
    "text" : "Unconfirmed"
  },
  "type" : "allergy",
  "category" : ["medication"],
  "code" : {
    "coding" : [{
      "system" : "http://snomed.info/sct",
      "code" : "716186003",
      "display" : "No known allergy"
    }],
    "text" : "No known medication allergies"
  },
  "patient" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  }
}

```
