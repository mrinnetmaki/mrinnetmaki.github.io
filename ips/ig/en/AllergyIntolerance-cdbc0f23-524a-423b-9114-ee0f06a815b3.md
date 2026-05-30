# AllergyIntoleranceBirch - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **AllergyIntoleranceBirch**

## Example AllergyIntolerance: AllergyIntoleranceBirch

Profiles: [IPA-AllergyIntolerance](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-allergyintolerance.html) version: 1.1.0, [AllergyIntolerance (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-AllergyIntolerance-uv-ips.html), [AllergyIntolerance (EU core)](http://hl7.eu/fhir/base/2.0.0/StructureDefinition-allergyIntolerance-eu-core.html), [AllergyIntolerance - Obligations (EPS)](https://build.fhir.org/ig/hl7-eu/eps/StructureDefinition-allergyintolerance-obl-eu-eps.html)

Security Labels: [patient reported (Details: v3 Code System ObservationValue code PATRPT = 'patient reported')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html), [patient asserted (Details: v3 Code System ObservationValue code PATAST = 'patient asserted')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html)

**clinicalStatus**: Active

**verificationStatus**: Unconfirmed

**type**: Allergy

**category**: Environment

**criticality**: Low Risk

**code**: Allergy to pollen, birch at least.

**patient**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**onset**: 1999

**note**: 

> 

Symptoms amplified by apple and nut allergies.


### Reactions

| | | | |
| :--- | :--- | :--- | :--- |
| - | **Substance** | **Manifestation** | **Severity** |
| * | Pollen, at least birch pollen | Dry eyes | Mild |



## Resource Content

```json
{
  "resourceType" : "AllergyIntolerance",
  "id" : "cdbc0f23-524a-423b-9114-ee0f06a815b3",
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
  "category" : ["environment"],
  "criticality" : "low",
  "code" : {
    "coding" : [{
      "system" : "http://snomed.info/sct",
      "code" : "256259004",
      "display" : "Pollen"
    },
    {
      "system" : "http://snomed.info/sct",
      "code" : "256262001",
      "display" : "European white birch pollen"
    }],
    "text" : "Allergy to pollen, birch at least."
  },
  "patient" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "onsetDateTime" : "1999",
  "note" : [{
    "text" : "Symptoms amplified by apple and nut allergies."
  }],
  "reaction" : [{
    "substance" : {
      "coding" : [{
        "system" : "http://snomed.info/sct",
        "code" : "256259004",
        "display" : "Pollen"
      },
      {
        "system" : "http://snomed.info/sct",
        "code" : "782576004",
        "display" : "Tree pollen"
      },
      {
        "system" : "http://snomed.info/sct",
        "code" : "256262001",
        "display" : "European white birch pollen"
      }],
      "text" : "Pollen, at least birch pollen"
    },
    "manifestation" : [{
      "coding" : [{
        "system" : "http://snomed.info/sct",
        "code" : "162290004",
        "display" : "Dry eyes"
      }],
      "text" : "Dry eyes"
    }],
    "severity" : "mild"
  }]
}

```
