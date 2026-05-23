# Provenance-ai-use - International Patient Summary for Mikael Rinnetmäki v0.4.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Provenance-ai-use**

## Example Provenance: Provenance-ai-use

I used Microsoft Copilot to add LOINC codes to lab results, based on the Finnish domestic Kuntaliitto codes that were present in my records. I verified the accuracy of the added codes and fixed any errors I was able to spot.



## Resource Content

```json
{
  "resourceType" : "Provenance",
  "id" : "acf8c98e-6bf1-451b-aa6c-bd47bc1a4da9",
  "meta" : {
    "security" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ObservationValue",
      "code" : "PATRPT",
      "display" : "patient reported"
    },
    {
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ObservationValue",
      "code" : "PATAST",
      "display" : "patient asserted"
    },
    {
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ObservationValue",
      "code" : "AIAST",
      "display" : "Artificial Intelligence asserted"
    }]
  },
  "target" : [{
    "reference" : "urn:uuid:88f6c5a2-1b8e-42e0-b5a0-a2e5c1f7d9e4",
    "display" : "Observation of B -Hb (hemoglobiini) for Mikael"
  },
  {
    "reference" : "urn:uuid:1d2c3f4a-5b6e-7f8a-9b0c-d1e2f3a4b5c6",
    "display" : "Observation of B -HbA1c (hemoglobiini-A1c) for Mikael"
  },
  {
    "reference" : "urn:uuid:c7d8e9f0-a1b2-c3d4-e5f6-a7b8c9d0e1f2",
    "display" : "Observation of B -HKR (hematokriitti) for Mikael"
  },
  {
    "reference" : "urn:uuid:f3a4b5c6-d7e8-f9a0-b1c2-d3e4f5a6b7c8",
    "display" : "Observation of B -Leuk (leukosyytit) for Mikael"
  },
  {
    "reference" : "urn:uuid:a9b0c1d2-e3f4-a5b6-c7d8-e9f0a1b2c3d4",
    "display" : "Observation of B -Trom (trombosyytit) for Mikael"
  },
  {
    "reference" : "urn:uuid:e1f2a3b4-c5d6-e7f8-9a0b-1c2d3e4f5a6b",
    "display" : "Observation of E -MCV (keskimääräinen erytrosyyttitilavuus) for Mikael"
  },
  {
    "reference" : "urn:uuid:1a2b3c4d-5e6f-7a8b-9c0d-1e2f3a4b5c6d",
    "display" : "Observation of E -RDW (erytrosyyttien kokojakauma) for Mikael"
  },
  {
    "reference" : "urn:uuid:5c6d7e8f-9a0b-1c2d-3e4f-5a6b7c8d9e0f",
    "display" : "Observation of E -MCH (keskimääräinen hemoglobiinimäärä) for Mikael"
  },
  {
    "reference" : "urn:uuid:8a9b0c1d-2e3f-4a5b-6c7d-8e9f0a1b2c3d",
    "display" : "Observation of fP-Fe (rauta) for Mikael"
  },
  {
    "reference" : "urn:uuid:0e1f2a3b-4c5d-6e7f-8a9b-0c1d2e3f4a5b",
    "display" : "Observation of fP-Transf (transferriini) for Mikael"
  },
  {
    "reference" : "urn:uuid:4a5b6c7d-8e9f-0a1b-2c3d-4e5f6a7b8c9d",
    "display" : "Observation of P -AT3 (antitrombiini III) for Mikael"
  },
  {
    "reference" : "urn:uuid:0a1b2c3d-4e5f-6a7b-8c9d-0e1f2a3b4c5d",
    "display" : "Observation of P -B2GPABG (beta-2-glykoproteiini AB) for Mikael"
  },
  {
    "reference" : "urn:uuid:6c7d8e9f-0a1b-2c3d-4e5f-6a7b8c9d0e1f",
    "display" : "Observation of P -B2GPABM (beta-2-glykoproteiini AB) for Mikael"
  },
  {
    "reference" : "urn:uuid:c6d7e8f9-a0b1-c2d3-e4f5-a6b7c8d9e0f1",
    "display" : "Observation of P -Ferrit (ferritiini) for Mikael"
  },
  {
    "reference" : "urn:uuid:7d8e9f0a-1b2c-3d4e-5f6a-7b8c9d0e1f2a",
    "display" : "Observation of P -K (kalium) for Mikael"
  },
  {
    "reference" : "urn:uuid:2a3b4c5d-6e7f-8a9b-0c1d-2e3f4a5b6c7d",
    "display" : "Observation of P -B2GPAbG (beeta-2-glykoproteiini, IgG-vasta-aineet) for Mikael"
  },
  {
    "reference" : "urn:uuid:8e9f0a1b-2c3d-4e5f-6a7b-8c9d0e1f2a3b",
    "display" : "Observation of P -B2GPAbM (beeta-2-glykoproteiini, IgM-vasta-aineet) for Mikael"
  },
  {
    "reference" : "urn:uuid:9f0a1b2c-3d4e-5f6a-7b8c-9d0e1f2a3b4c",
    "display" : "Observation of P -Kol-HDL (HDL-kolesteroli) for Mikael"
  },
  {
    "reference" : "urn:uuid:5b6c7d8e-9f0a-1b2c-3d4e-5f6a7b8c9d0e",
    "display" : "Observation of P -Kol-LDL (LDL-kolesteroli) for Mikael"
  },
  {
    "reference" : "urn:uuid:3e4f5a6b-7c8d-9e0f-1a2b-3c4d5e6f7a8b",
    "display" : "Observation of P -Kol (kolesteroli) for Mikael"
  },
  {
    "reference" : "urn:uuid:1f2a3b4c-5d6e-7f8a-9b0c-d1e2f3a4b5c6",
    "display" : "Observation of P -Krea (kreatiini) for Mikael"
  },
  {
    "reference" : "urn:uuid:4e5f6a7b-8c9d-0e1f-2a3b-4c5d6e7f8a9b",
    "display" : "Observation of P -LuakPTT (lupusantikoagulantti, PTT) for Mikael"
  },
  {
    "reference" : "urn:uuid:a0b1c2d3-e4f5-6a7b-8c9d-e0f1a2b3c4d5",
    "display" : "Observation of P -LuakRVV (lupusantikoagulantti, RVV) for Mikael"
  },
  {
    "reference" : "urn:uuid:d7e8f9a0-b1c2-d3e4-f5a6-b7c8d9e0f1a2",
    "display" : "Observation of P -Na (natrium) for Mikael"
  },
  {
    "reference" : "urn:uuid:e5f6a7b8-c9d0-e1f2-a3b4-c5d6e7f8a9b0",
    "display" : "Observation of P -PC (proteiini C) for Mikael"
  },
  {
    "reference" : "urn:uuid:1b2c3d4e-5f6a-7b8c-9d0e-1f2a3b4c5d6e",
    "display" : "Observation of P -PS-AgV (proteiini S, antigeeni, vapaa) for Mikael"
  },
  {
    "reference" : "urn:uuid:9a0b1c2d-3e4f-5a6b-7c8d-9e0f1a2b3c4d",
    "display" : "Observation of P -TrAika (trombiiniaika) for Mikael"
  },
  {
    "reference" : "urn:uuid:b3c4d5e6-f7a8-9b0c-1d2e-3f4a5b6c7d8e",
    "display" : "Observation of P -Trigly (triglyseridi) for Mikael"
  },
  {
    "reference" : "urn:uuid:7f8a9b0c-1d2e-3f4a-5b6c-7d8e9f0a1b2c",
    "display" : "Observation of P -TT-INR (tromboplastiiniaika, INR-tulostus) for Mikael"
  },
  {
    "reference" : "urn:uuid:d3e4f5a6-b7c8-d9e0-f1a2-b3c4d5e6f7a8",
    "display" : "Observation of P -TT-SPA (tromboplastiiniaika, SPA-tulostus) for Mikael"
  },
  {
    "reference" : "urn:uuid:96b4cbd4-8862-4f09-9ac8-d65f4c6e88bc",
    "display" : "Observation of Pt-GFReEPI (glomerulussuodosnopeus, estimoitu) 1 for Mikael"
  },
  {
    "reference" : "urn:uuid:6f7a8b9c-0d1e-2f3a-4b5c-6d7e8f9a0b1c",
    "display" : "Observation of Pt-GFReEPI (glomerulussuodosnopeus, estimoitu) 2 for Mikael"
  },
  {
    "reference" : "urn:uuid:2e3f4a5b-6c7d-8e9f-0a1b-2c3d4e5f6a7b",
    "display" : "Observation of TrFeSat (transferriinin rautakyllästeisyys) for Mikael"
  },
  {
    "reference" : "urn:uuid:9bd79ab3-7b0c-40e2-ad65-b1f7ec42b8bc",
    "display" : "Observation of U -Alb (albumiini) 1 for Mikael"
  },
  {
    "reference" : "urn:uuid:2c3d4e5f-6a7b-8c9d-0e1f-2a3b4c5d6e7f",
    "display" : "Observation of U -Alb (albumiini) 2 for Mikael"
  },
  {
    "reference" : "urn:uuid:07e4f795-134d-4704-a776-ce30216d988e",
    "display" : "Observation of U -Alb/Kre (albumiini-kreatiniinisuhde) 1 for Mikael"
  },
  {
    "reference" : "urn:uuid:04d80b58-af0f-40d1-8cca-2a416bebbc74",
    "display" : "Observation of U -Alb/Kre (albumiini-kreatiniinisuhde) 2 for Mikael"
  },
  {
    "reference" : "urn:uuid:4384b8a1-0a26-405a-9519-08035d9ab72a",
    "display" : "Observation of U -Krea (kreatiniini) 1 for Mikael"
  },
  {
    "reference" : "urn:uuid:26868547-dc76-45a1-9f6e-3ce6fe2d4e61",
    "display" : "Observation of U -Krea (kreatiniini) 2 for Mikael"
  }],
  "occurredDateTime" : "2026-01-23T17:29:00+02:00",
  "recorded" : "2026-02-13T18:41:00+02:00",
  "reason" : [{
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/v3-ActReason",
      "code" : "LABELING",
      "display" : "labeling"
    }],
    "text" : "Add LOINC codes in addition to the local Kuntaliitto codes."
  }],
  "agent" : [{
    "type" : {
      "coding" : [{
        "system" : "http://terminology.hl7.org/CodeSystem/provenance-participant-type",
        "code" : "author",
        "display" : "Author"
      }]
    },
    "role" : [{
      "coding" : [{
        "system" : "http://terminology.hl7.org/CodeSystem/v3-ParticipationType",
        "code" : "AUT",
        "display" : "author (originator)"
      }]
    },
    {
      "coding" : [{
        "system" : "http://terminology.hl7.org/CodeSystem/v3-RoleCode",
        "code" : "CLASSIFIER",
        "display" : "classifier"
      }]
    },
    {
      "coding" : [{
        "system" : "http://terminology.hl7.org/CodeSystem/extra-security-role-type",
        "code" : "humanuser",
        "display" : "human user"
      }]
    }],
    "who" : {
      "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
      "display" : "Mikael Rinnetmäki, the patient"
    }
  },
  {
    "type" : {
      "coding" : [{
        "system" : "http://terminology.hl7.org/CodeSystem/provenance-participant-type",
        "code" : "composer",
        "display" : "Composer"
      }]
    },
    "role" : [{
      "coding" : [{
        "system" : "http://terminology.hl7.org/CodeSystem/extra-security-role-type",
        "code" : "dataprocessor",
        "display" : "data processor"
      }]
    },
    {
      "coding" : [{
        "system" : "http://terminology.hl7.org/CodeSystem/v3-RoleClass",
        "code" : "AGNT",
        "display" : "agent"
      }]
    }],
    "who" : {
      "identifier" : {
        "system" : "urn:ietf:rfc:3986",
        "value" : "https://copilot.microsoft.com/"
      },
      "display" : "Copilot in Visual Studio Code"
    },
    "onBehalfOf" : {
      "reference" : "urn:uuid:b4ac89c5-6589-417f-beef-d3fb1ef9c70f",
      "display" : "Mikael Rinnetmäki, the patient"
    }
  }]
}

```
