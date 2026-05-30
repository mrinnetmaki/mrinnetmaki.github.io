# Sensotrend IPS Client Capability Statement - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Sensotrend IPS Client Capability Statement**

## CapabilityStatement: Sensotrend IPS Client Capability Statement 

| | |
| :--- | :--- |
| *Official URL*:https://ips.sensotrend.com/ig/CapabilityStatement/ips-client-capability-statement-01 | *Version*:0.4.0 |
| Active as of 2026-03-12 | *Computable Name*:IpsClientCapabilityStatement |
| *Other Identifiers:*OID:1.2.246.537.6.990.18.5.777.13.1 | |

 [Raw OpenAPI-Swagger Definition file](../ips-client-capability-statement-01.openapi.json) | [Download](../ips-client-capability-statement-01.openapi.json) 



## Resource Content

```json
{
  "resourceType" : "CapabilityStatement",
  "id" : "ips-client-capability-statement-01",
  "url" : "https://ips.sensotrend.com/ig/CapabilityStatement/ips-client-capability-statement-01",
  "version" : "0.4.0",
  "name" : "IpsClientCapabilityStatement",
  "title" : "IPS Client Capability Statement",
  "status" : "active",
  "date" : "2026-03-12",
  "publisher" : "Mikael Rinnetmäki",
  "contact" : [{
    "name" : "Mikael Rinnetmäki",
    "telecom" : [{
      "system" : "url",
      "value" : "https://mikaelrinnetmaki.fi"
    },
    {
      "system" : "email",
      "value" : "mikael.rinnetmaki@gmail.com"
    }]
  }],
  "purpose" : "The metadata about Sensotrend's IPS Client implementation, including the supported resources and operations.",
  "kind" : "instance",
  "software" : {
    "name" : "Sensotrend IPS Client",
    "version" : "0.1.0",
    "releaseDate" : "2026-03-12"
  },
  "implementation" : {
    "description" : "Sensotrend's IPS Client implementation",
    "url" : "https://ips.sensotrend.com/view/"
  },
  "fhirVersion" : "4.0.1",
  "format" : ["json"],
  "implementationGuide" : ["http://hl7.org/fhir/uv/ipa/STU1.1",
  "http://hl7.org/fhir/uv/ips/STU2",
  "http://hl7.eu/fhir/base/2.0.0",
  "https://hl7.fi/fhir/finnish-base-profiles/2.0.0",
  "https://hl7.eu/fhir/eps/xtehr"],
  "rest" : [{
    "mode" : "client",
    "resource" : [{
      "type" : "Bundle",
      "profile" : "http://hl7.org/fhir/uv/ips/StructureDefinition/Bundle-uv-ips|2.0.0",
      "supportedProfile" : ["http://hl7.eu/fhir/eps/StructureDefinition/bundle-eu-eps|1.0.0-ci-build"],
      "interaction" : [{
        "code" : "read"
      }]
    },
    {
      "type" : "Composition",
      "profile" : "http://hl7.org/fhir/uv/ips/StructureDefinition/Composition-uv-ips|2.0.0",
      "supportedProfile" : ["http://hl7.eu/fhir/eps/StructureDefinition/composition-eu-eps|1.0.0-ci-build"]
    },
    {
      "type" : "Patient",
      "profile" : "http://hl7.org/fhir/uv/ips/StructureDefinition/Patient-uv-ips|2.0.0",
      "supportedProfile" : ["http://hl7.eu/fhir/eps/StructureDefinition/patient-eu-eps|1.0.0-ci-build",
      "https://hl7.fi/fhir/finnish-base-profiles/StructureDefinition/fi-base-patient|2.0.0"],
      "interaction" : [{
        "code" : "read"
      }],
      "operation" : [{
        "name" : "summary",
        "definition" : "http://hl7.org/fhir/uv/ips/OperationDefinition/summary|2.0.0",
        "documentation" : "The server supports the basic summary operation, but no search parameters. The returned IPS document is always in the universal IPS format, and for the default patient."
      }]
    },
    {
      "type" : "AllergyIntolerance",
      "profile" : "http://hl7.org/fhir/uv/ips/StructureDefinition/AllergyIntolerance-uv-ips|2.0.0",
      "supportedProfile" : ["http://hl7.eu/fhir/eps/StructureDefinition/allergyintolerance-obl-eu-eps|1.0.0-ci-build",
      "http://hl7.eu/fhir/base/StructureDefinition/allergyIntolerance-eu-core|2.0.0"]
    },
    {
      "type" : "Condition",
      "profile" : "http://hl7.org/fhir/uv/ips/StructureDefinition/Condition-uv-ips|2.0.0",
      "supportedProfile" : ["http://hl7.eu/fhir/eps/StructureDefinition/condition-obl-eu-eps|1.0.0-ci-build",
      "http://hl7.eu/fhir/base/StructureDefinition/condition-eu-core|2.0.0"]
    },
    {
      "type" : "Consent",
      "profile" : "http://hl7.eu/fhir/eps/StructureDefinition/consent-eu-eps|1.0.0-ci-build"
    },
    {
      "type" : "Device",
      "profile" : "http://hl7.org/fhir/uv/ips/StructureDefinition/Device-uv-ips|2.0.0",
      "supportedProfile" : ["http://hl7.eu/fhir/eps/StructureDefinition/device-eu-eps|1.0.0-ci-build"]
    },
    {
      "type" : "DeviceUseStatement",
      "profile" : "http://hl7.org/fhir/uv/ips/StructureDefinition/DeviceUseStatement-uv-ips|2.0.0",
      "supportedProfile" : ["http://hl7.eu/fhir/eps/StructureDefinition/deviceUseStatement-eu-eps|1.0.0-ci-build"]
    },
    {
      "type" : "DiagnosticReport",
      "profile" : "http://hl7.org/fhir/uv/ips/StructureDefinition/DiagnosticReport-uv-ips|2.0.0",
      "supportedProfile" : ["http://hl7.eu/fhir/eps/StructureDefinition/diagnosticReport-eu-eps|1.0.0-ci-build"]
    },
    {
      "type" : "Immunization",
      "profile" : "http://hl7.org/fhir/uv/ips/StructureDefinition/Immunization-uv-ips|2.0.0",
      "supportedProfile" : ["http://hl7.eu/fhir/base/StructureDefinition/immunization-eu-core|2.0.0",
      "http://hl7.eu/fhir/base/StructureDefinition/immunization-eu-core|2.0.0"]
    },
    {
      "type" : "Medication",
      "profile" : "http://hl7.org/fhir/uv/ips/StructureDefinition/Medication-uv-ips|2.0.0",
      "supportedProfile" : ["http://hl7.eu/fhir/eps/StructureDefinition/medication-obl-eu-eps|1.0.0-ci-build"]
    },
    {
      "type" : "MedicationRequest",
      "profile" : "http://hl7.org/fhir/uv/ips/StructureDefinition/MedicationRequest-uv-ips|2.0.0",
      "supportedProfile" : ["http://hl7.eu/fhir/eps/StructureDefinition/medicationrequest-obl-eu-eps|1.0.0-ci-build"]
    },
    {
      "type" : "MedicationStatement",
      "profile" : "http://hl7.org/fhir/uv/ips/StructureDefinition/MedicationStatement-uv-ips|2.0.0",
      "supportedProfile" : ["http://hl7.eu/fhir/eps/StructureDefinition/MedicationStatement-eu-eps|1.0.0-ci-build"]
    },
    {
      "type" : "Observation",
      "profile" : "http://hl7.eu/fhir/base/StructureDefinition/medicalTestResult-eu-core|2.0.0",
      "supportedProfile" : ["http://hl7.org/fhir/uv/ips/StructureDefinition/Observation-pregnancy-edd-uv-ips|2.0.0",
      "http://hl7.org/fhir/uv/ips/StructureDefinition/Observation-pregnancy-outcome-uv-ips|2.0.0",
      "http://hl7.org/fhir/uv/ips/StructureDefinition/Observation-pregnancy-status-uv-ips|2.0.0",
      "http://hl7.org/fhir/uv/ips/StructureDefinition/Observation-alcoholuse-uv-ips|2.0.0",
      "http://hl7.org/fhir/uv/ips/StructureDefinition/Observation-tobaccouse-uv-ips|2.0.0",
      "http://hl7.org/fhir/uv/ips/StructureDefinition/Observation-results-laboratory-pathology-uv-ips|2.0.0",
      "http://hl7.org/fhir/uv/ips/StructureDefinition/Observation-results-radiology-uv-ips|2.0.0",
      "http://hl7.org/fhir/StructureDefinition/resprate|4.0.1",
      "http://hl7.org/fhir/StructureDefinition/heartrate|4.0.1",
      "http://hl7.org/fhir/StructureDefinition/oxygensat|4.0.1",
      "http://hl7.org/fhir/StructureDefinition/bodytemp|4.0.1",
      "http://hl7.org/fhir/StructureDefinition/bodyheight|4.0.1",
      "http://hl7.org/fhir/StructureDefinition/headcircum|4.0.1",
      "http://hl7.org/fhir/StructureDefinition/bodyweight|4.0.1",
      "http://hl7.org/fhir/StructureDefinition/bmi|4.0.1",
      "http://hl7.org/fhir/StructureDefinition/bp|4.0.1",
      "http://hl7.eu/fhir/eps/StructureDefinition/observation-pregnancy-edd-eu-eps|1.0.0-ci-build",
      "http://hl7.eu/fhir/eps/StructureDefinition/observation-pregnancy-outcome-eu-eps|1.0.0-ci-build",
      "http://hl7.eu/fhir/eps/StructureDefinition/observation-pregnancy-status-eu-ips|1.0.0-ci-build"]
    },
    {
      "type" : "Procedure",
      "profile" : "http://hl7.org/fhir/uv/ips/StructureDefinition/Procedure-uv-ips|2.0.0",
      "supportedProfile" : ["http://hl7.eu/fhir/eps/StructureDefinition/procedure-eu-eps|1.0.0-ci-build"]
    }]
  }],
  "document" : [{
    "mode" : "producer",
    "profile" : "http://hl7.org/fhir/uv/ips/StructureDefinition/Composition-uv-ips|2.0.0"
  }]
}

```
