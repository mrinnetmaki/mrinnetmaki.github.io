# Deny-data-use-for-marketing - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Deny-data-use-for-marketing**

## Example Consent: Deny-data-use-for-marketing

I don't want my data to be used for marketing purposes.



## Resource Content

```json
{
  "resourceType" : "Consent",
  "id" : "fc6ca80d-ce07-47d9-a1c0-49e955ae166b",
  "meta" : {
    "profile" : ["http://hl7.eu/fhir/eps/StructureDefinition/consent-eu-eps"],
    "security" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ObservationValue",
      "code" : "PATRPT",
      "display" : "patient reported"
    }]
  },
  "status" : "active",
  "scope" : {
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/consentscope",
      "code" : "adr",
      "display" : "Advanced Care Directive"
    },
    {
      "system" : "http://terminology.hl7.org/CodeSystem/consentscope",
      "code" : "patient-privacy",
      "display" : "Privacy Consent"
    }],
    "text" : "Patient Privacy Consent"
  },
  "category" : [{
    "coding" : [{
      "system" : "http://loinc.org",
      "code" : "64292-6",
      "display" : "Release of information consent Document"
    }],
    "text" : "Release of information consent Document"
  },
  {
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/consentcategorycodes",
      "code" : "acd",
      "display" : "Advance Directive"
    }],
    "text" : "Advance Directive"
  },
  {
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/consentcategorycodes",
      "code" : "rsdid",
      "display" : "De-identified Information Access"
    }],
    "text" : "De-identified information"
  },
  {
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/consentcategorycodes",
      "code" : "rsreid",
      "display" : "Re-identifiable Information Access"
    }],
    "text" : "Re-identifiable information"
  }],
  "patient" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "dateTime" : "2026-02-13T17:59:00+02:00",
  "performer" : [{
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki, the patient"
  }],
  "policyRule" : {
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ActCode",
      "code" : "GDPRCD",
      "display" : "GDPR Consent Directive"
    }],
    "text" : "GDPR consent"
  },
  "provision" : {
    "type" : "deny",
    "purpose" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ActReason",
      "code" : "HMARKT",
      "display" : "healthcare marketing"
    }],
    "data" : [{
      "meaning" : "related",
      "reference" : {
        "type" : "Bundle",
        "identifier" : {
          "value" : "ips-for-mikko"
        },
        "display" : "This patient summary"
      }
    }]
  }
}

```
