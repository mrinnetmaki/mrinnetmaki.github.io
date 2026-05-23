# DeviceUseStatementYpsoPump - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **DeviceUseStatementYpsoPump**

## Example DeviceUseStatement: DeviceUseStatementYpsoPump

Profiles: [DeviceUseStatement (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-DeviceUseStatement-uv-ips.html), [DeviceUseStatement (EPS)](https://build.fhir.org/ig/hl7-eu/eps/StructureDefinition-deviceUseStatement-eu-eps.html)

Security Labels: patient reported (Details: ObservationValue code PATRPT = 'patient reported'), patient asserted (Details: ObservationValue code PATAST = 'patient asserted')

**status**: Active

**subject**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**timing**: 2023-10-06 --> (ongoing)

**recordedOn**: 2023-12-27

**source**: [Mikael Rinnetmäki, the patient](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)

**device**: [mylife YpsoPump insulin pump](Bundle-IpsBundle.md#urn-uuid-a88f7ff5-7803-43f5-a6bb-3c542736ce5e)

**reasonCode**: Type 1 diabetes mellitus

**reasonReference**: [Type 1 diabetes mellitus](Bundle-IpsBundle.md#urn-uuid-1558c456-efa1-4b3d-abe2-1522c6048bc7)



## Resource Content

```json
{
  "resourceType" : "DeviceUseStatement",
  "id" : "96001cc6-0b17-434e-8405-ed37dfddc76a",
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
    "start" : "2023-10-06"
  },
  "recordedOn" : "2023-12-27",
  "source" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki, the patient"
  },
  "device" : {
    "reference" : "urn:uuid:a88f7ff5-7803-43f5-a6bb-3c542736ce5e",
    "display" : "mylife YpsoPump insulin pump"
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
  }]
}

```
