# DeviceMylifeLoop - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **DeviceMylifeLoop**

## Example Device: DeviceMylifeLoop

Profiles: [Device (IPS)](http://hl7.org/fhir/uv/ips/STU2/StructureDefinition-Device-uv-ips.html), [Device (EPS)](https://build.fhir.org/ig/hl7-eu/eps/StructureDefinition-device-eu-eps.html)

Security Labels: patient reported (Details: ObservationValue code PATRPT = 'patient reported'), patient asserted (Details: ObservationValue code PATAST = 'patient asserted')

**status**: Active

**manufacturer**: Ypsomed AG

### DeviceNames

| | | |
| :--- | :--- | :--- |
| - | **Name** | **Type** |
| * | mylife Loop | manufacturer-name |

**type**: Invasive interstitial fluid glucose monitoring/insulin infusion system

**patient**: [Mikael Rinnetmäki](Bundle-IpsBundle.md#urn-uuid-b4ac89c5-6589-417f-beef-d3fb1ef9c70f)



## Resource Content

```json
{
  "resourceType" : "Device",
  "id" : "97b044bd-17ff-4fe0-a52d-af4d4731a0b9",
  "meta" : {
    "profile" : ["http://hl7.org/fhir/uv/ips/StructureDefinition/Device-uv-ips",
    "http://hl7.eu/fhir/eps/StructureDefinition/device-eu-eps"],
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
  "manufacturer" : "Ypsomed AG",
  "deviceName" : [{
    "name" : "mylife Loop",
    "type" : "manufacturer-name"
  }],
  "type" : {
    "coding" : [{
      "system" : "http://snomed.info/sct",
      "code" : "702203005",
      "display" : "Invasive interstitial fluid glucose monitoring/insulin infusion system"
    }]
  },
  "patient" : {
    "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
    "display" : "Mikael Rinnetmäki"
  }
}

```
