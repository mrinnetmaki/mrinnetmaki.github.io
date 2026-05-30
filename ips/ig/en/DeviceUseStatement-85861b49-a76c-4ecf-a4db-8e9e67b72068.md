# DeviceUseStatementDexcomG6 - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **DeviceUseStatementDexcomG6**

## Example DeviceUseStatement: DeviceUseStatementDexcomG6

Profiles: [DeviceUseStatement (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-DeviceUseStatement-uv-ips.html), [DeviceUseStatement (EPS)](https://build.fhir.org/ig/hl7-eu/eps/StructureDefinition-deviceUseStatement-eu-eps.html)

Security Labels: [patient reported (Details: v3 Code System ObservationValue code PATRPT = 'patient reported')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html), [patient asserted (Details: v3 Code System ObservationValue code PATAST = 'patient asserted')](http://hl7.org/fhir/R4/v3/ObservationValue/cs.html)

**status**: Active

**subject**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**timing**: 2023-10-06 --> 2024-11-30

**recordedOn**: 2023-12-27

**source**: [Mikael Rinnetmäki, the patient](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**device**: [Dexcom G6 continuous glucose monitoring (CGM) system](Bundle-IpsBundle.md#urn-uuid-876781b9-0db0-429a-877b-23e17e4d8443)

**reasonCode**: Type 1 diabetes mellitus

**reasonReference**: [Type 1 diabetes mellitus](Bundle-IpsBundle.md#urn-uuid-1558c456-efa1-4b3d-abe2-1522c6048bc7)

**note**: By urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f

> 

I switched from Dexcom G6 CGM to Abbott Freestyle Libre 3+ in November 2024, but still use Dexcom occasionally. I find Dexcom sensors to be more accurate. Libre tends to show lower readings for me, compared to fingerstick measurements (with all glucometers I've tried).




## Resource Content

```json
{
  "resourceType" : "DeviceUseStatement",
  "id" : "85861b49-a76c-4ecf-a4db-8e9e67b72068",
  "meta" : {
    "profile" : ["http://hl7.org/fhir/uv/ips/StructureDefinition/DeviceUseStatement-uv-ips",
    "http://hl7.eu/fhir/eps/StructureDefinition/deviceUseStatement-eu-eps"],
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
  "status" : "active",
  "subject" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  },
  "timingPeriod" : {
    "start" : "2023-10-06",
    "end" : "2024-11-30"
  },
  "recordedOn" : "2023-12-27",
  "source" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki, the patient"
  },
  "device" : {
    "reference" : "urn:uuid:876781b9-0db0-429a-877b-23e17e4d8443",
    "display" : "Dexcom G6 continuous glucose monitoring (CGM) system"
  },
  "reasonCode" : [{
    "coding" : [{
      "system" : "http://snomed.info/sct",
      "code" : "46635009",
      "display" : "Type 1 diabetes mellitus"
    }],
    "text" : "Type 1 diabetes mellitus"
  }],
  "reasonReference" : [{
    "reference" : "urn:uuid:1558c456-efa1-4b3d-abe2-1522c6048bc7",
    "display" : "Type 1 diabetes mellitus"
  }],
  "note" : [{
    "authorReference" : {
      "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
      "display" : "Mikael Rinnetmäki, the patient"
    },
    "text" : "I switched from Dexcom G6 CGM to Abbott Freestyle Libre 3+ in November 2024, but still use Dexcom occasionally. I find Dexcom sensors to be more accurate. Libre tends to show lower readings for me, compared to fingerstick measurements (with all glucometers I've tried)."
  }]
}

```
