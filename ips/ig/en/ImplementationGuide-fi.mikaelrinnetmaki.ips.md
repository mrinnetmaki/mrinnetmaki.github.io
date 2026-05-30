# Resource International Patient Summary for Mikael Rinnetmäki



## Resource Content

```json
{
  "resourceType" : "ImplementationGuide",
  "id" : "fi.mikaelrinnetmaki.ips",
  "language" : "en",
  "url" : "https://mikaelrinnetmaki.fi/ips/ig/ImplementationGuide/fi.mikaelrinnetmaki.ips",
  "version" : "0.4.0",
  "name" : "MikaelsIPS",
  "title" : "International Patient Summary for Mikael Rinnetmäki",
  "status" : "active",
  "date" : "2026-05-30T12:56:35+02:00",
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
  "description" : "This document describes Sensotrend's implementation of the [HL7 FHIR IPS](https://hl7.org/fhir/uv/ips/) format of the [International Patient Summary (IPS)](https://international-patient-summary.net/) specification both as a client app and as a FHIR server. It also includes and extensive example patient summary for Mikael Rinnetmäki, the author and the patient.",
  "packageId" : "fi.mikaelrinnetmaki.ips",
  "license" : "CC0-1.0",
  "fhirVersion" : ["4.0.1"],
  "dependsOn" : [{
    "id" : "hl7tx",
    "extension" : [{
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/implementationguide-dependency-comment",
      "valueMarkdown" : "Automatically added as a dependency - all IGs depend on HL7 Terminology"
    }],
    "uri" : "http://terminology.hl7.org/ImplementationGuide/hl7.terminology",
    "packageId" : "hl7.terminology.r4",
    "version" : "7.1.0"
  },
  {
    "id" : "hl7ext",
    "extension" : [{
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/implementationguide-dependency-comment",
      "valueMarkdown" : "Automatically added as a dependency - all IGs depend on the HL7 Extension Pack"
    }],
    "uri" : "http://hl7.org/fhir/extensions/ImplementationGuide/hl7.fhir.uv.extensions",
    "packageId" : "hl7.fhir.uv.extensions.r4",
    "version" : "5.3.0"
  },
  {
    "id" : "hl7_fhir_uv_ipa",
    "uri" : "http://hl7.org/fhir/uv/ipa/ImplementationGuide/hl7.fhir.uv.ipa",
    "packageId" : "hl7.fhir.uv.ipa",
    "version" : "1.1.0"
  },
  {
    "id" : "hl7_fhir_uv_ips",
    "uri" : "http://hl7.org/fhir/uv/ips/ImplementationGuide/hl7.fhir.uv.ips",
    "packageId" : "hl7.fhir.uv.ips",
    "version" : "2.0.0"
  },
  {
    "id" : "hl7_fhir_eu_base",
    "uri" : "http://hl7.eu/fhir/base/ImplementationGuide/hl7.fhir.eu.base",
    "packageId" : "hl7.fhir.eu.base",
    "version" : "2.0.0"
  },
  {
    "id" : "hl7_fhir_fi_base",
    "uri" : "https://hl7.fi/fhir/finnish-base-profiles/ImplementationGuide/hl7.fhir.fi.base",
    "packageId" : "hl7.fhir.fi.base",
    "version" : "2.0.0"
  },
  {
    "id" : "hl7_fhir_eu_eps",
    "uri" : "http://hl7.eu/fhir/eps/ImplementationGuide/hl7.fhir.eu.eps",
    "packageId" : "hl7.fhir.eu.eps",
    "version" : "current"
  },
  {
    "id" : "hl7_fhir_uv_security_label_ds4p",
    "uri" : "http://hl7.org/fhir/uv/security-label-ds4p/ImplementationGuide/hl7.fhir.uv.security-label-ds4p",
    "packageId" : "hl7.fhir.uv.security-label-ds4p",
    "version" : "1.0.0"
  }],
  "definition" : {
    "extension" : [{
      "extension" : [{
        "url" : "code",
        "valueString" : "copyrightyear"
      },
      {
        "url" : "value",
        "valueString" : "2023+"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "releaselabel"
      },
      {
        "url" : "value",
        "valueString" : "ci-build"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "auto-oid-root"
      },
      {
        "url" : "value",
        "valueString" : "1.2.246.537.6.990.18.5.777"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "pin-canonicals"
      },
      {
        "url" : "value",
        "valueString" : "pin-all"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "autoload-resources"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "path-liquid"
      },
      {
        "url" : "value",
        "valueString" : "template/liquid"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "path-liquid"
      },
      {
        "url" : "value",
        "valueString" : "input/liquid"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "path-qa"
      },
      {
        "url" : "value",
        "valueString" : "temp/qa"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "path-temp"
      },
      {
        "url" : "value",
        "valueString" : "temp/pages"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "path-output"
      },
      {
        "url" : "value",
        "valueString" : "output"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "path-suppressed-warnings"
      },
      {
        "url" : "value",
        "valueString" : "input/ignoreWarnings.txt"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "path-history"
      },
      {
        "url" : "value",
        "valueString" : "https://mikaelrinnetmaki.fi/ips/ig/history.html"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "template-html"
      },
      {
        "url" : "value",
        "valueString" : "template-page.html"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "template-md"
      },
      {
        "url" : "value",
        "valueString" : "template-page-md.html"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "apply-contact"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "apply-context"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "apply-copyright"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "apply-jurisdiction"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "apply-license"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "apply-publisher"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "apply-version"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "apply-wg"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "active-tables"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "fmm-definition"
      },
      {
        "url" : "value",
        "valueString" : "http://hl7.org/fhir/versions.html#maturity"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "propagate-status"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "excludelogbinaryformat"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "tabbed-snapshots"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueString" : "i18n-default-lang"
      },
      {
        "url" : "value",
        "valueString" : "en"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-internal-dependency",
      "valueCode" : "hl7.fhir.uv.tools.r4#1.1.2"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "copyrightyear"
      },
      {
        "url" : "value",
        "valueString" : "2023+"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "releaselabel"
      },
      {
        "url" : "value",
        "valueString" : "ci-build"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "auto-oid-root"
      },
      {
        "url" : "value",
        "valueString" : "1.2.246.537.6.990.18.5.777"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "pin-canonicals"
      },
      {
        "url" : "value",
        "valueString" : "pin-all"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "autoload-resources"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "path-liquid"
      },
      {
        "url" : "value",
        "valueString" : "template/liquid"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "path-liquid"
      },
      {
        "url" : "value",
        "valueString" : "input/liquid"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "path-qa"
      },
      {
        "url" : "value",
        "valueString" : "temp/qa"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "path-temp"
      },
      {
        "url" : "value",
        "valueString" : "temp/pages"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "path-output"
      },
      {
        "url" : "value",
        "valueString" : "output"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "path-suppressed-warnings"
      },
      {
        "url" : "value",
        "valueString" : "input/ignoreWarnings.txt"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "path-history"
      },
      {
        "url" : "value",
        "valueString" : "https://mikaelrinnetmaki.fi/ips/ig/history.html"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "template-html"
      },
      {
        "url" : "value",
        "valueString" : "template-page.html"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "template-md"
      },
      {
        "url" : "value",
        "valueString" : "template-page-md.html"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "apply-contact"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "apply-context"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "apply-copyright"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "apply-jurisdiction"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "apply-license"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "apply-publisher"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "apply-version"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "apply-wg"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "active-tables"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "fmm-definition"
      },
      {
        "url" : "value",
        "valueString" : "http://hl7.org/fhir/versions.html#maturity"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "propagate-status"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "excludelogbinaryformat"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "tabbed-snapshots"
      },
      {
        "url" : "value",
        "valueString" : "true"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    },
    {
      "extension" : [{
        "url" : "code",
        "valueCode" : "i18n-default-lang"
      },
      {
        "url" : "value",
        "valueString" : "en"
      }],
      "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
    }],
    "resource" : [{
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Consent"
      }],
      "reference" : {
        "reference" : "Consent/8d139b91-6567-4372-9329-0a2faf7cae99"
      },
      "name" : "Advance-directives",
      "description" : "Advance directives for my treatment",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "AllergyIntolerance"
      }],
      "reference" : {
        "reference" : "AllergyIntolerance/61bea1b2-13a3-4e5f-9d2d-1d5a02bd0eef"
      },
      "name" : "AllergyIntoleranceApple",
      "description" : "Allergy to apple",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "AllergyIntolerance"
      }],
      "reference" : {
        "reference" : "AllergyIntolerance/cdbc0f23-524a-423b-9114-ee0f06a815b3"
      },
      "name" : "AllergyIntoleranceBirch",
      "description" : "Allergy to birch pollen",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "AllergyIntolerance"
      }],
      "reference" : {
        "reference" : "AllergyIntolerance/e7ba84d4-87f4-4170-805b-c2c516c4fcab"
      },
      "name" : "AllergyIntoleranceMedicationNoKnown",
      "description" : "No known medication allergies",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "AllergyIntolerance"
      }],
      "reference" : {
        "reference" : "AllergyIntolerance/6728beb7-b028-4976-9ea8-ccc29336756f"
      },
      "name" : "AllergyIntoleranceNut",
      "description" : "Allergy to nuts",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Condition"
      }],
      "reference" : {
        "reference" : "Condition/1e591fa2-f118-4ef4-9103-9b9fe5d3da75"
      },
      "name" : "ConditionCollarbone",
      "description" : "Past broken collarbone",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Condition"
      }],
      "reference" : {
        "reference" : "Condition/1558c456-efa1-4b3d-abe2-1522c6048bc7"
      },
      "name" : "ConditionDiabetesT1",
      "description" : "Type 1 diabetes",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Condition"
      }],
      "reference" : {
        "reference" : "Condition/ead8fa45-4c6b-47b5-876b-6c01090d2c49"
      },
      "name" : "ConditionFinger",
      "description" : "Past broken finger",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Condition"
      }],
      "reference" : {
        "reference" : "Condition/c279fd61-c4da-406b-a14b-b6166b956f83"
      },
      "name" : "ConditionHypercholesterolemia",
      "description" : "Diabetes related hypercholesterolemia",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Condition"
      }],
      "reference" : {
        "reference" : "Condition/2c4dc13c-2927-4cd7-b86e-1a3b89493d2b"
      },
      "name" : "ConditionPulmonaryEmbolism",
      "description" : "Past pulmonary embolism",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Condition"
      }],
      "reference" : {
        "reference" : "Condition/8cb43587-94e6-4520-8b71-bbdab015ce0a"
      },
      "name" : "ConditionRetinopathy",
      "description" : "Diabetes related retinopathy",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Condition"
      }],
      "reference" : {
        "reference" : "Condition/22e07a7b-4d9b-406d-93bc-dc60de933f1f"
      },
      "name" : "ConditionShoulder",
      "description" : "Past problem with shoulder",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Condition"
      }],
      "reference" : {
        "reference" : "Condition/af227524-ca64-46ed-8aad-c17f1a712af5"
      },
      "name" : "ConditionSight",
      "description" : "Mild myopia",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Condition"
      }],
      "reference" : {
        "reference" : "Condition/d621ec37-44d1-455a-9f95-b62ee1e6f7f1"
      },
      "name" : "ConditionVocalChord-1",
      "description" : "Dysphonia due to vocal cord problems",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Condition"
      }],
      "reference" : {
        "reference" : "Condition/14534413-2ea5-4988-9f2a-a7f6c6059353"
      },
      "name" : "ConditionVocalChord-2",
      "description" : "Disputed diagnosis of disease in larynx",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Consent"
      }],
      "reference" : {
        "reference" : "Consent/0b8b4bfe-12e8-4dcc-9299-27fd76e464ce"
      },
      "name" : "Consent-data-use-healthcare",
      "description" : "Consent for the use of my data in healthcare",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Consent"
      }],
      "reference" : {
        "reference" : "Consent/e7fd44af-ae28-4994-a04f-37d8e52864a1"
      },
      "name" : "Consent-data-use-research",
      "description" : "Consent for the use of *de-identified information* for research, including machine learning training",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Consent"
      }],
      "reference" : {
        "reference" : "Consent/fc6ca80d-ce07-47d9-a1c0-49e955ae166b"
      },
      "name" : "Deny-data-use-for-marketing",
      "description" : "Deny the use of my data for marketing",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Consent"
      }],
      "reference" : {
        "reference" : "Consent/c67f1ac1-5013-47dc-88ad-73d8eca510b0"
      },
      "name" : "Deny-data-use-for-ml-training",
      "description" : "Deny the use of *re-identifiable* data for machine learning training",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Device"
      }],
      "reference" : {
        "reference" : "Device/f2cfe332-9d2f-4216-9e89-452aa5fac885"
      },
      "name" : "DeviceAbbottFreestyleLibre3",
      "description" : "Abbott Freestyle Libre 3 continuous glucose monitoring system",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Device"
      }],
      "reference" : {
        "reference" : "Device/9c49dff9-84b0-45f6-9e52-e8fa4b186473"
      },
      "name" : "DeviceCamAPS",
      "description" : "CamAPS hybrid closed loop insulin delivery system algorithm",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Device"
      }],
      "reference" : {
        "reference" : "Device/876781b9-0db0-429a-877b-23e17e4d8443"
      },
      "name" : "DeviceDexcomG6",
      "description" : "Dexcom G6 continuous glucose monitoring system",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Device"
      }],
      "reference" : {
        "reference" : "Device/97b044bd-17ff-4fe0-a52d-af4d4731a0b9"
      },
      "name" : "DeviceMylifeLoop",
      "description" : "mylife Loop automated insulin delivery system",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "DeviceUseStatement"
      }],
      "reference" : {
        "reference" : "DeviceUseStatement/2ba85ad7-9e3e-4468-a10f-7c7d13114f0f"
      },
      "name" : "DeviceUseStatementCamAPSFX",
      "description" : "Use of the CamAPS FX hybrid closed loop insulin delivery system algorithm since October 6, 2023",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "DeviceUseStatement"
      }],
      "reference" : {
        "reference" : "DeviceUseStatement/85861b49-a76c-4ecf-a4db-8e9e67b72068"
      },
      "name" : "DeviceUseStatementDexcomG6",
      "description" : "Use of the Dexcom G6 continuous glucose monitoring (CGM) system since October 6, 2023 until November 30, 2024",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "DeviceUseStatement"
      }],
      "reference" : {
        "reference" : "DeviceUseStatement/25ba5f1a-90b3-49a8-a251-ac402bb4ccc8"
      },
      "name" : "DeviceUseStatementFreestyleLibre3",
      "description" : "Use of the Abbott Freestyle Libre 3 continuous glucose monitoring (CGM) system since November 30, 2024",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "DeviceUseStatement"
      }],
      "reference" : {
        "reference" : "DeviceUseStatement/905180fb-dc21-4b81-95d8-e2918657ce22"
      },
      "name" : "DeviceUseStatementMylifeLoop2023",
      "description" : "Use of the mylife Loop automated insulin delivery system since October 6, 2023",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "DeviceUseStatement"
      }],
      "reference" : {
        "reference" : "DeviceUseStatement/96001cc6-0b17-434e-8405-ed37dfddc76a"
      },
      "name" : "DeviceUseStatementYpsoPump",
      "description" : "Use of the mylife YpsoPump insulin pump since October 6, 2023",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Device"
      }],
      "reference" : {
        "reference" : "Device/a88f7ff5-7803-43f5-a6bb-3c542736ce5e"
      },
      "name" : "DeviceYpsopump",
      "description" : "Ypsopump insulin pump",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Immunization"
      }],
      "reference" : {
        "reference" : "Immunization/d9828658-c9dd-478c-8573-c514cd834f5f"
      },
      "name" : "ImmunizationCovid1",
      "description" : "Covid vaccination 1, Comirnaty",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Immunization"
      }],
      "reference" : {
        "reference" : "Immunization/f3fff46d-7755-4af3-a334-a3d3899d8a58"
      },
      "name" : "ImmunizationCovid2",
      "description" : "Covid vaccination 2, Comirnaty",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Immunization"
      }],
      "reference" : {
        "reference" : "Immunization/aac217a5-cd2f-4217-b5ff-c55e9f7c3378"
      },
      "name" : "ImmunizationCovid3",
      "description" : "Covid vaccination 3, Spikevax",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Immunization"
      }],
      "reference" : {
        "reference" : "Immunization/9c0744c0-9b0a-4796-b653-452a0098625f"
      },
      "name" : "ImmunizationCovid4",
      "description" : "Covid vaccination 4, Comirnaty",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Immunization"
      }],
      "reference" : {
        "reference" : "Immunization/244fb199-b9b2-49ef-85cd-09e5cdbc83af"
      },
      "name" : "ImmunizationHepatitisA1",
      "description" : "Hepatitis A vaccination 1 / 2",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Immunization"
      }],
      "reference" : {
        "reference" : "Immunization/97345cda-49d9-453c-8c9c-01edc6607cc7"
      },
      "name" : "ImmunizationHepatitisA2",
      "description" : "Hepatitis A vaccination 2 / 2",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Immunization"
      }],
      "reference" : {
        "reference" : "Immunization/a0ca2399-1f86-487b-ad6c-3e64081ae945"
      },
      "name" : "ImmunizationHepatitisB1",
      "description" : "Hepatitis B vaccination 1 / 3",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Immunization"
      }],
      "reference" : {
        "reference" : "Immunization/d33a6a70-9c27-4b4b-a3bb-731fc2e43fb2"
      },
      "name" : "ImmunizationHepatitisB2",
      "description" : "Hepatitis B vaccination 2 / 3",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Immunization"
      }],
      "reference" : {
        "reference" : "Immunization/f871751d-14fe-4672-bc2f-6a6e83e6ac73"
      },
      "name" : "ImmunizationHepatitisB3",
      "description" : "Hepatitis B vaccination 3 / 3",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Immunization"
      }],
      "reference" : {
        "reference" : "Immunization/cae0ed26-c654-403c-8c85-ff4432949786"
      },
      "name" : "ImmunizationInfluenza1",
      "description" : "Vaxigrip influenza vaccine 2014",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Immunization"
      }],
      "reference" : {
        "reference" : "Immunization/b54184da-87e6-4c0f-a85a-9546a5cc9783"
      },
      "name" : "ImmunizationInfluenza2",
      "description" : "Vaxigrip influenza vaccine 2015",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Immunization"
      }],
      "reference" : {
        "reference" : "Immunization/04dfd1be-9483-485d-8030-a9ce3a264363"
      },
      "name" : "ImmunizationInfluenza3",
      "description" : "Vaxigriptetra influenza vaccine 2019",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Immunization"
      }],
      "reference" : {
        "reference" : "Immunization/5906618a-e76b-44b5-b670-7a0820075bae"
      },
      "name" : "ImmunizationInfluenza4",
      "description" : "Vaxigriptetra influenza vaccine 2022",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Immunization"
      }],
      "reference" : {
        "reference" : "Immunization/bfe1d5a4-be0e-403a-a27c-16ef74aca3b3"
      },
      "name" : "ImmunizationInfluenza5",
      "description" : "Vaxigriptetra influenza vaccine 2023",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Immunization"
      }],
      "reference" : {
        "reference" : "Immunization/cf4545bb-604d-45de-a7da-95baf181286b"
      },
      "name" : "ImmunizationMeningitis",
      "description" : "MeningoVac A+C meningococcal vaccine",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Immunization"
      }],
      "reference" : {
        "reference" : "Immunization/f1649cba-fde7-4d54-8fcd-37b6240017ac"
      },
      "name" : "ImmunizationPolio",
      "description" : "Imovax Polio vaccine",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Immunization"
      }],
      "reference" : {
        "reference" : "Immunization/5a3c0871-af41-4f63-9615-d98308d9e794"
      },
      "name" : "ImmunizationTetanus1",
      "description" : "Tetanus booster 2003",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Immunization"
      }],
      "reference" : {
        "reference" : "Immunization/bd632ca0-6661-4b9d-bbf6-7ffd3154e700"
      },
      "name" : "ImmunizationTetanus2",
      "description" : "Tetanus booster 2015",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Immunization"
      }],
      "reference" : {
        "reference" : "Immunization/6b8e54e6-6023-4911-9a43-91b73066dc08"
      },
      "name" : "ImmunizationTyphoidFever",
      "description" : "Typherix typhoid fever vaccine 2019",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Immunization"
      }],
      "reference" : {
        "reference" : "Immunization/6cfe08b7-55a1-40d9-9010-484f59b13ff2"
      },
      "name" : "ImmunizationYellowFever",
      "description" : "Yellow fever vaccination",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Composition"
      }],
      "reference" : {
        "reference" : "Composition/c69a5242-339d-4101-adc7-96728f2f517f"
      },
      "name" : "International Patient Summary",
      "description" : "International Patient Summary for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Bundle"
      }],
      "reference" : {
        "reference" : "Bundle/IpsBundle"
      },
      "name" : "IpsBundle",
      "description" : "International Patient Summary for Mikael as a FHIR Bundle",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Medication"
      }],
      "reference" : {
        "reference" : "Medication/9a241a9a-d6ee-4361-af90-9aa702499329"
      },
      "name" : "MedicationEzetimibe",
      "description" : "Ezetimibe",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Medication"
      }],
      "reference" : {
        "reference" : "Medication/e6f153f4-6188-4dc4-9f19-f4179b9ee720"
      },
      "name" : "MedicationInsulinNovorapid",
      "description" : "Insulin Novorapid",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "MedicationRequest"
      }],
      "reference" : {
        "reference" : "MedicationRequest/58b57392-03fb-4a5f-90b9-117f82754431"
      },
      "name" : "MedicationRequestExetimibe",
      "description" : "Prescription for Ezetimibe",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "MedicationRequest"
      }],
      "reference" : {
        "reference" : "MedicationRequest/847b849a-eb83-4387-b60b-46eb8d39ebfd"
      },
      "name" : "MedicationRequestInsulinNovorapid",
      "description" : "Prescription for Insulin Novorapid",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "MedicationRequest"
      }],
      "reference" : {
        "reference" : "MedicationRequest/83e47f0e-cfb3-4ada-9bdb-7ad7223e0260"
      },
      "name" : "MedicationRequestRosuvastatin10mg",
      "description" : "Prescription for Rosuvastatin",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "MedicationRequest"
      }],
      "reference" : {
        "reference" : "MedicationRequest/03fd8e6f-d898-4fc9-9e79-3dc7132c721d"
      },
      "name" : "MedicationRequestRosuvastatin5mg",
      "description" : "Prescription for Rosuvastatin 5mg, stopped (replaced by 10mg)",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Medication"
      }],
      "reference" : {
        "reference" : "Medication/1af60d57-5a04-42d4-b63e-f509652c57f2"
      },
      "name" : "MedicationRosuvastatin10mg",
      "description" : "Rosuvastatin 10 mg",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Medication"
      }],
      "reference" : {
        "reference" : "Medication/9a265107-bd19-4ea4-bc5d-6fd94e8d7c88"
      },
      "name" : "MedicationRosuvastatin5mg",
      "description" : "Rosuvastatin 5 mg",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "MedicationStatement"
      }],
      "reference" : {
        "reference" : "MedicationStatement/17725642-fd58-4f71-a9e6-1dee30e048bf"
      },
      "name" : "MedicationStatementEzetimibe",
      "description" : "I use Rosuvastatin and Ezetimibe for diabetes related hypercholesterolemia.",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "MedicationStatement"
      }],
      "reference" : {
        "reference" : "MedicationStatement/bb2d0be6-24fd-4e1f-8fa4-10e058ed2775"
      },
      "name" : "MedicationStatementInsulinNovorapid",
      "description" : "I use Insulin Novorapid for Type 1 diabetes",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "MedicationStatement"
      }],
      "reference" : {
        "reference" : "MedicationStatement/f3f4ff44-62be-440c-9e79-1a5de2d64016"
      },
      "name" : "MedicationStatementRosuvastatin",
      "description" : "I use Rosuvastatin and Ezetimibe for diabetes related hypercholesterolemia.",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Patient"
      }],
      "reference" : {
        "reference" : "Patient/b4ac89c5-6589-417f-beef-d3fb1ef9c70f"
      },
      "name" : "Mikael",
      "description" : "Mikael Rinnetmäki, the patient",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/432d2590-6b3a-4e3f-b38c-6a0cc8dc9243"
      },
      "name" : "Observation-alcohol-use",
      "description" : "Observation of alcohol use for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/125cef80-fe5c-40db-976f-c6d51e099519"
      },
      "name" : "Observation-b-erybla-1",
      "description" : "Observation of B -EryBla (erytroblastit) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/3db4dd0f-789d-492e-baa8-74b3994e89e9"
      },
      "name" : "Observation-b-eryt-1",
      "description" : "Observation of B -Erytrosyytit for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/c00df5d3-5bf4-4093-9a1b-b877ff75a1d3"
      },
      "name" : "Observation-f-calpro-1",
      "description" : "Observation of F -Calpro (kalprotektiini) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/88f6c5a2-1b8e-42e0-b5a0-a2e5c1f7d9e4"
      },
      "name" : "Observation-lab-b-hb-1",
      "description" : "Observation of B -Hb (hemoglobiini) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/1d2c3f4a-5b6e-7f8a-9b0c-d1e2f3a4b5c6"
      },
      "name" : "Observation-lab-b-hba1c-1",
      "description" : "Observation of B -HbA1c (hemoglobiini-A1c) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/c7d8e9f0-a1b2-c3d4-e5f6-a7b8c9d0e1f2"
      },
      "name" : "Observation-lab-b-hkr-1",
      "description" : "Observation of B -HKR (hematokriitti) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/f3a4b5c6-d7e8-f9a0-b1c2-d3e4f5a6b7c8"
      },
      "name" : "Observation-lab-b-leuk-1",
      "description" : "Observation of B -Leuk (leukosyytit eli valkosolut) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/a9b0c1d2-e3f4-a5b6-c7d8-e9f0a1b2c3d4"
      },
      "name" : "Observation-lab-b-trom-1",
      "description" : "Observation of B -Trom (verihiutaleet) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/5c6d7e8f-9a0b-1c2d-3e4f-5a6b7c8d9e0f"
      },
      "name" : "Observation-lab-e-mch-1",
      "description" : "Observation of E -MCH (hemoglobiini, keskimassa) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/e1f2a3b4-c5d6-e7f8-9a0b-1c2d3e4f5a6b"
      },
      "name" : "Observation-lab-e-mcv-1",
      "description" : "Observation of E -MCV (keskimääräinen punasolun tilavuus) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/1a2b3c4d-5e6f-7a8b-9c0d-1e2f3a4b5c6d"
      },
      "name" : "Observation-lab-e-rdw-1",
      "description" : "Observation of E -RDW (punasolujen kokojakauma) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/8a9b0c1d-2e3f-4a5b-6c7d-8e9f0a1b2c3d"
      },
      "name" : "Observation-lab-fp-fe-1",
      "description" : "Observation of fP-Fe (rauta) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/0e1f2a3b-4c5d-6e7f-8a9b-0c1d2e3f4a5b"
      },
      "name" : "Observation-lab-fp-transf-1",
      "description" : "Observation of fP-Transf (transferriini) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/4a5b6c7d-8e9f-0a1b-2c3d-4e5f6a7b8c9d"
      },
      "name" : "Observation-lab-p-at3-1",
      "description" : "Observation of P -AT3 (antitrombiini III) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/0a1b2c3d-4e5f-6a7b-8c9d-0e1f2a3b4c5d"
      },
      "name" : "Observation-lab-p-b2gpabg-1",
      "description" : "Observation of P -B2GPAbG (beeta-2-glykoproteiini, IgG-vasta-aineet) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/6c7d8e9f-0a1b-2c3d-4e5f-6a7b8c9d0e1f"
      },
      "name" : "Observation-lab-p-b2gpabm-1",
      "description" : "Observation of P -B2GPAbM (beeta-2-glykoproteiini, IgM-vasta-aineet) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/c6d7e8f9-a0b1-c2d3-e4f5-a6b7c8d9e0f1"
      },
      "name" : "Observation-lab-p-ferrit-1",
      "description" : "Observation of P -Ferrit (ferritiini) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/7d8e9f0a-1b2c-3d4e-5f6a-7b8c9d0e1f2a"
      },
      "name" : "Observation-lab-p-k-1",
      "description" : "Observation of P -K (kalium) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/2a3b4c5d-6e7f-8a9b-0c1d-2e3f4a5b6c7d"
      },
      "name" : "Observation-lab-p-kardabg-1",
      "description" : "Observation of P -KardAbG (kardiolipiini, IgG-vasta-aineet) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/8e9f0a1b-2c3d-4e5f-6a7b-8c9d0e1f2a3b"
      },
      "name" : "Observation-lab-p-kardabm-1",
      "description" : "Observation of P -KardAbM (kardiolipiini, IgM-vasta-aineet) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/3e4f5a6b-7c8d-9e0f-1a2b-3c4d5e6f7a8b"
      },
      "name" : "Observation-lab-p-kol-1",
      "description" : "Observation of P -Kol (kokonaiskolesteroli) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/9f0a1b2c-3d4e-5f6a-7b8c-9d0e1f2a3b4c"
      },
      "name" : "Observation-lab-p-kol-hdl-1",
      "description" : "Observation of P -Kol-HDL (HDL-kolesteroli) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/5b6c7d8e-9f0a-1b2c-3d4e-5f6a7b8c9d0e"
      },
      "name" : "Observation-lab-p-kol-ldl-1",
      "description" : "Observation of P -Kol-LDL (LDL-kolesteroli) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/1f2a3b4c-5d6e-7f8a-9b0c-d1e2f3a4b5c6"
      },
      "name" : "Observation-lab-p-krea-1",
      "description" : "Observation of P -Krea (kreatiniini) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/4e5f6a7b-8c9d-0e1f-2a3b-4c5d6e7f8a9b"
      },
      "name" : "Observation-lab-p-luakptt-1",
      "description" : "Observation of P -LuakPTT (lupusantikoagulantti, PTT) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/a0b1c2d3-e4f5-6a7b-8c9d-e0f1a2b3c4d5"
      },
      "name" : "Observation-lab-p-luakrvv-1",
      "description" : "Observation of P -LuakRVV (lupusantikoagulantti, dRVVT) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/d7e8f9a0-b1c2-d3e4-f5a6-b7c8d9e0f1a2"
      },
      "name" : "Observation-lab-p-na-1",
      "description" : "Observation of P -Na (natrium) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/e5f6a7b8-c9d0-e1f2-a3b4-c5d6e7f8a9b0"
      },
      "name" : "Observation-lab-p-pc-1",
      "description" : "Observation of P -PC (proteiini C) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/1b2c3d4e-5f6a-7b8c-9d0e-1f2a3b4c5d6e"
      },
      "name" : "Observation-lab-p-ps-agv-1",
      "description" : "Observation of P -PS-AgV (proteiini S, antigeeni, vapaa) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/9a0b1c2d-3e4f-5a6b-7c8d-9e0f1a2b3c4d"
      },
      "name" : "Observation-lab-p-traika-1",
      "description" : "Observation of P -TrAika (trombiiniaika) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/b3c4d5e6-f7a8-9b0c-1d2e-3f4a5b6c7d8e"
      },
      "name" : "Observation-lab-p-trigly-1",
      "description" : "Observation of P -Trigly (triglyseridi) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/7f8a9b0c-1d2e-3f4a-5b6c-7d8e9f0a1b2c"
      },
      "name" : "Observation-lab-p-tt-inr-1",
      "description" : "Observation of P -TT-INR (tromboplastiiniaika, INR-tulostus) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/d3e4f5a6-b7c8-d9e0-f1a2-b3c4d5e6f7a8"
      },
      "name" : "Observation-lab-p-tt-spa-1",
      "description" : "Observation of P -TT-SPA (tromboplastiiniaika, SPA-tulostus) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/96b4cbd4-8862-4f09-9ac8-d65f4c6e88bc"
      },
      "name" : "Observation-lab-pt-gfrepi-1",
      "description" : "Observation of Pt-GFReEPI (glomerulussuodosnopeus, estimoitu) 1 for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/6f7a8b9c-0d1e-2f3a-4b5c-6d7e8f9a0b1c"
      },
      "name" : "Observation-lab-pt-gfrepi-2",
      "description" : "Observation of Pt-GFReEPI (glomerulussuodosnopeus, estimoitu) 2 for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/2e3f4a5b-6c7d-8e9f-0a1b-2c3d4e5f6a7b"
      },
      "name" : "Observation-lab-trfesat-1",
      "description" : "Observation of TrFeSat (transferriinin rautakyllästeisyys) for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/9bd79ab3-7b0c-40e2-ad65-b1f7ec42b8bc"
      },
      "name" : "Observation-lab-u-alb-1",
      "description" : "Observation of U -Alb (albumiini) 1 for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/2c3d4e5f-6a7b-8c9d-0e1f-2a3b4c5d6e7f"
      },
      "name" : "Observation-lab-u-alb-2",
      "description" : "Observation of U -Alb (albumiini) 2 for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/07e4f795-134d-4704-a776-ce30216d988e"
      },
      "name" : "Observation-lab-u-albkre-1",
      "description" : "Observation of U -Alb/Kre (albumiini-kreatiniinisuhde) 1 for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/04d80b58-af0f-40d1-8cca-2a416bebbc74"
      },
      "name" : "Observation-lab-u-albkre-2",
      "description" : "Observation of U -Alb/Kre (albumiini-kreatiniinisuhde) 2 for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/4384b8a1-0a26-405a-9519-08035d9ab72a"
      },
      "name" : "Observation-lab-u-krea-1",
      "description" : "Observation of U -Krea (kreatiniini) 1 for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/26868547-dc76-45a1-9f6e-3ce6fe2d4e61"
      },
      "name" : "Observation-lab-u-krea-2",
      "description" : "Observation of U -Krea (kreatiniini) 2 for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/ec8d3ccb-d68c-433f-8db7-5bf1fcaf0328"
      },
      "name" : "Observation-tobacco-use",
      "description" : "Observation of tobacco use for Mikael",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/87fd93df-3a9e-433a-a824-97702a294dce"
      },
      "name" : "Observation-vitals-bloodpressure-1",
      "description" : "Observation of blood pressure for Mikael, performed at a clinic 2025-10-24 (1/2)",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/55e62594-fc71-4437-ad8c-13acaf51d2cd"
      },
      "name" : "Observation-vitals-bloodpressure-2",
      "description" : "Observation of blood pressure for Mikael, performed at a clinic 2025-10-24 (2/2)",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/8b3f6d5f-a6bc-47c4-9e9f-e664c81ef6e9"
      },
      "name" : "Observation-vitals-bloodpressure-3",
      "description" : "Observation of blood pressure for Mikael 2026-01-04T15:48:09+02:00",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Observation"
      }],
      "reference" : {
        "reference" : "Observation/b06784f5-9e17-41b1-8ab0-09d8eb824f9a"
      },
      "name" : "Observation-vitals-bloodpressure-4",
      "description" : "Observation of blood pressure for Mikael 2026-01-04T15:49:06+02:00",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Procedure"
      }],
      "reference" : {
        "reference" : "Procedure/f134bd3a-755a-444a-9364-0e4e1cef2520"
      },
      "name" : "ProcedureRingFinger",
      "description" : "Surgical operation to fix a fraccture of the left ring finger",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Provenance"
      }],
      "reference" : {
        "reference" : "Provenance/acf8c98e-6bf1-451b-aa6c-bd47bc1a4da9"
      },
      "name" : "Provenance-ai-use",
      "description" : "Declaration of the use of AI in the creation of this patient summary",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "Provenance"
      }],
      "reference" : {
        "reference" : "Provenance/1f5bd080-2962-4a52-ae9f-d2209abef49b"
      },
      "name" : "Provenance-ips-creation",
      "description" : "Declaration of this patient summary being crafted by hand by the patient themselves",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "CapabilityStatement"
      }],
      "reference" : {
        "reference" : "CapabilityStatement/ips-client-capability-statement-01"
      },
      "name" : "Sensotrend IPS Client Capability Statement",
      "description" : "The metadata about the IPS Client implementation, including the supported resources and operations.",
      "exampleBoolean" : true
    },
    {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
        "valueString" : "CapabilityStatement"
      }],
      "reference" : {
        "reference" : "CapabilityStatement/ips-server-capability-statement"
      },
      "name" : "Sensotrend IPS Server Capability Statement",
      "description" : "The metadata about the IPS Server implementation, including the supported resources and operations.",
      "exampleBoolean" : true
    }],
    "page" : {
      "extension" : [{
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-page-name",
        "valueUrl" : "toc.html"
      }],
      "nameUrl" : "toc.html",
      "title" : "Table of Contents",
      "generation" : "html",
      "page" : [{
        "extension" : [{
          "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-page-name",
          "valueUrl" : "index.html"
        }],
        "nameUrl" : "index.html",
        "title" : "Home",
        "generation" : "markdown"
      }]
    },
    "parameter" : [{
      "code" : "path-resource",
      "value" : "input/capabilities"
    },
    {
      "code" : "path-resource",
      "value" : "input/examples"
    },
    {
      "code" : "path-resource",
      "value" : "input/extensions"
    },
    {
      "code" : "path-resource",
      "value" : "input/models"
    },
    {
      "code" : "path-resource",
      "value" : "input/operations"
    },
    {
      "code" : "path-resource",
      "value" : "input/profiles"
    },
    {
      "code" : "path-resource",
      "value" : "input/resources"
    },
    {
      "code" : "path-resource",
      "value" : "input/vocabulary"
    },
    {
      "code" : "path-resource",
      "value" : "input/maps"
    },
    {
      "code" : "path-resource",
      "value" : "input/testing"
    },
    {
      "code" : "path-resource",
      "value" : "input/history"
    },
    {
      "code" : "path-resource",
      "value" : "fsh-generated/resources"
    },
    {
      "code" : "path-pages",
      "value" : "template/config"
    },
    {
      "code" : "path-pages",
      "value" : "input/images"
    },
    {
      "code" : "path-tx-cache",
      "value" : "input-cache/txcache"
    }]
  }
}

```
