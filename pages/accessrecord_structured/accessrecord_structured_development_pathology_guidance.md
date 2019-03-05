---
title: Pathology guidance
keywords: getcarerecord
tags: [design,structured]
sidebar: accessrecord_structured_sidebar
permalink: accessrecord_structured_development_pathology_guidance.html
summary: "Guidance on the representation of allergies and intolerances in GP Connect"
---

# Investigations Modeling

## Patholgy Reporting in GP Practices
Currently in GP practices 
## Requesting

## Receiving Reports
### EDIFact
## Filing Reports
## Report structure

## Scope
## Available FHIR resources

| Resource name       | Description | Used in GP Connect |
|---------------------|-------------------| ----------|
| [`ProcedureRequest`](accessrecord_structured_development_medication.html) | For requesting investigations to be performed by a laboratory | Yes |
| ['DiagnosticReport'](accessrecord_structured_development_medicationrequest.html) | A reporting structure that contains results and any relevant data such as specimen details or attribution | Yes |
| [`Specimen`](accessrecord_structured_development_medicationstatement.html) | Used to make a statement about the medication a person has taken and can be 'basedOn' a record of an historic prescription that would be represented using one or more MedicationRequest resources. | Yes |
| `Observation` | Represent exactly what medication was dispensed. In some cases, this can differ slightly from what was ordered/prescribed. | No |

## Using the FHIR profiles to represent filed results
