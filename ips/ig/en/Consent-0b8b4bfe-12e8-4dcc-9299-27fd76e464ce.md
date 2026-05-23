# Consent-data-use-healthcare - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Consent-data-use-healthcare**

## Example Consent: Consent-data-use-healthcare

I want my data to be used for my treatment. Please use it! I'm fine with AI and decision support systems having access to my data for this purpose



## Resource Content

```json
{
  "resourceType" : "Consent",
  "id" : "0b8b4bfe-12e8-4dcc-9299-27fd76e464ce",
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
    "text" : "Patient Privacy"
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
  "policy" : [{
    "uri" : "https://eur-lex.europa.eu/eli/reg/2016/679/oj"
  }],
  "provision" : {
    "type" : "permit",
    "action" : [{
      "coding" : [{
        "system" : "http://terminology.hl7.org/CodeSystem/consentaction",
        "code" : "collect"
      }]
    },
    {
      "coding" : [{
        "system" : "http://terminology.hl7.org/CodeSystem/consentaction",
        "code" : "access"
      }]
    },
    {
      "coding" : [{
        "system" : "http://terminology.hl7.org/CodeSystem/consentaction",
        "code" : "use"
      }]
    },
    {
      "coding" : [{
        "system" : "http://terminology.hl7.org/CodeSystem/consentaction",
        "code" : "disclose"
      }]
    },
    {
      "coding" : [{
        "system" : "http://terminology.hl7.org/CodeSystem/consentaction",
        "code" : "correct"
      }]
    }],
    "purpose" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ActReason",
      "code" : "TREAT",
      "display" : "treatment"
    },
    {
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ActReason",
      "code" : "COC",
      "display" : "coordination of care"
    },
    {
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ActReason",
      "code" : "ETREAT",
      "display" : "Emergency Treatment"
    },
    {
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ActReason",
      "code" : "BTG",
      "display" : "break the glass"
    },
    {
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ActReason",
      "code" : "ERTREAT",
      "display" : "emergency room treatment"
    },
    {
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ActReason",
      "code" : "HOPERAT",
      "display" : "healthcare operations"
    },
    {
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ActReason",
      "code" : "TREATDS",
      "display" : "decision support assisted treatment decision"
    },
    {
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ActReason",
      "code" : "HTEST",
      "display" : "test health data"
    },
    {
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ActReason",
      "code" : "PATRQT",
      "display" : "patient requested"
    }]
  }
}

```
