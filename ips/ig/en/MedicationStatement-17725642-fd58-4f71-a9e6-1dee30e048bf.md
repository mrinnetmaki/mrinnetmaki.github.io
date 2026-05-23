# MedicationStatementEzetimibe - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **MedicationStatementEzetimibe**

## Example MedicationStatement: MedicationStatementEzetimibe

Profiles: [IPA-MedicationStatement](http://hl7.org/fhir/uv/ipa/STU1.1/StructureDefinition-ipa-medicationstatement.html) version: 1.1.0, [MedicationStatement (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-MedicationStatement-uv-ips.html), [MedicationStatement (EU core)](http://hl7.eu/fhir/base/2.0.0/StructureDefinition-medicationStatement-eu-core.html), [MedicationStatement (EPS)](https://build.fhir.org/ig/hl7-eu/eps/StructureDefinition-MedicationStatement-eu-eps.html)

Security Labels: device reported (Details: ObservationValue code DEVRPT = 'device reported'), patient reported (Details: ObservationValue code PATRPT = 'patient reported'), syntactic transform (Details: ObservationValue code SYNTAC = 'syntactic transform'), mapped (Details: ObservationValue code MAPPED = 'mapped'), patient asserted (Details: ObservationValue code PATAST = 'patient asserted')

**basedOn**: [Prescription for Ezetimibe](Bundle-IpsBundle.md#urn-uuid-58b57392-03fb-4a5f-90b9-117f82754431)

**status**: active

**category**: Active ambulatory use

**medication**: [Ezetimibe 10 mg](Bundle-IpsBundle.md#urn-uuid-9a241a9a-d6ee-4361-af90-9aa702499329)

**subject**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**effective**: 2023-12-20 --> (ongoing)

**reasonCode**: Hypercholesterolemia

**reasonReference**: [Diabetes related hypercholesterolemia](Bundle-IpsBundle.md#urn-uuid-c279fd61-c4da-406b-a14b-b6166b956f83)

**note**: By urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f

> 

I know I should be taking both rosuvastatin and ezetimibe in the evening, but I take them in the morning, because that's when I remember to take them. My doctor knows this, and approves.


> **dosage****text**: 1 tabletti 1 kerran vuorokaudessa suun kautta Kolesterolilääke, ldl-tavoite <1,4, yhdessä statiinin kanssa.**patientInstruction**: 1 tabletti 1 kerran vuorokaudessa suun kautta Kolesterolilääke, ldl-tavoite <1,4, yhdessä statiinin kanssa.

### DoseAndRates

| | |
| :--- | :--- |
| - | **Rate[x]** |
| * | 10 mg/day (Details: UCUM codemg/d = 'mg/d') |




## Resource Content

```json
{
  "resourceType" : "MedicationStatement",
  "id" : "17725642-fd58-4f71-a9e6-1dee30e048bf",
  "meta" : {
    "profile" : ["http://hl7.org/fhir/uv/ipa/StructureDefinition/ipa-medicationstatement|1.1.0",
    "http://hl7.org/fhir/uv/ips/StructureDefinition/MedicationStatement-uv-ips",
    "http://hl7.eu/fhir/base/StructureDefinition/medicationStatement-eu-core",
    "http://hl7.eu/fhir/eps/StructureDefinition/MedicationStatement-eu-eps"],
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
  "basedOn" : [{
    "reference" : "urn:uuid:58b57392-03fb-4a5f-90b9-117f82754431",
    "display" : "Prescription for Ezetimibe"
  }],
  "status" : "active",
  "category" : {
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/medication-statement-category",
      "code" : "community",
      "display" : "Community"
    },
    {
      "system" : "http://snomed.info/sct",
      "code" : "360270004",
      "display" : "Therapy - action"
    }],
    "text" : "Active ambulatory use"
  },
  "medicationReference" : {
    "reference" : "urn:uuid:9a241a9a-d6ee-4361-af90-9aa702499329",
    "display" : "Ezetimibe 10 mg"
  },
  "subject" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "effectivePeriod" : {
    "start" : "2023-12-20"
  },
  "reasonCode" : [{
    "coding" : [{
      "system" : "http://snomed.info/sct",
      "code" : "13644009",
      "display" : "Hypercholesterolemia (disorder)"
    },
    {
      "system" : "http://hl7.org/fhir/sid/icd-10",
      "code" : "E78.0",
      "display" : "Pure hypercholesterolaemia"
    }],
    "text" : "Hypercholesterolemia"
  }],
  "reasonReference" : [{
    "reference" : "urn:uuid:c279fd61-c4da-406b-a14b-b6166b956f83",
    "display" : "Diabetes related hypercholesterolemia"
  }],
  "note" : [{
    "authorReference" : {
      "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
      "display" : "Mikael Rinnetmäki, the patient"
    },
    "text" : "I know I should be taking both rosuvastatin and ezetimibe in the evening, but I take them in the morning, because that's when I remember to take them. My doctor knows this, and approves."
  }],
  "dosage" : [{
    "text" : "1 tabletti 1 kerran vuorokaudessa suun kautta Kolesterolilääke, ldl-tavoite <1,4, yhdessä statiinin kanssa.",
    "patientInstruction" : "1 tabletti 1 kerran vuorokaudessa suun kautta Kolesterolilääke, ldl-tavoite <1,4, yhdessä statiinin kanssa.",
    "doseAndRate" : [{
      "rateQuantity" : {
        "value" : 10,
        "unit" : "mg/day",
        "system" : "http://unitsofmeasure.org",
        "code" : "mg/d"
      }
    }]
  }]
}

```
