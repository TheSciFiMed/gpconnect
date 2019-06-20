---
title: Immunization guidance
keywords: structured design
tags: [design,structured]
sidebar: accessrecord_structured_sidebar
permalink: accessrecord_structured_development_immunization_guidance.html
summary: "FHIR resource Immunization"
---

## What is an immunisation? ##

An immunisation is the event of a patient being administered a vaccination. This may be a contemporaneous record by the clinician administering the vaccination (or by another member of the practice staff recording the event directly on behalf of the clinician) or it may be a record of an immunisation administered elsewhere as reported to the registered GP practice by the patient, a carer, guardian or other representative of the patient or another healthcare provider.

Immunisation may be given as part of a scheduled programme of immunisations such as childhood immunisations, seasonal influenza vaccination or in response to specific circumstances e.g. prior to travel, disease outbreak or occupational risk.

## Using the procedure code ##

GP Clinical Systems have not recorded the full vaccine product (dm+d code) as their main identifier for immunisation.
GP Clinical Systems record the type of vaccine administered as opposed to the vaccine product.
This may be as a procedure code or a local code which maps to a procedure code. 
The immunisation procedure code will be used as the main vaccine identifier. 
The vaccine product can be included if it is available.

## Immunisations that were not given ##

This version of the specification only includes supports immunisation which have been given to the patient.
GP Clinical Systems may capture details of circumstances where an immunisation has not been given but there was an intention to.
Planned immunisations may not be given for a variety of reasons, such as

* an explicity refusal for a specific vaccine or for any form of immunisation
* lack of consent for a vaccine to be administered
* the vaccine is temporarily decline
* a contraindication with another medication
* the patient does not attend an appointment or does not attend an open clinic (e.g. seasonal flu vaccination clinic)
* the patient is unwell or does not meet criteria for the vaccination

All circumstances of an immunisation not given are out of scope of this version.
Options are to be evaluated for the use cases where information is available for not given immunisations and for those valid use cases whether such information is most appropriately included in another resource or included in a future version of this profile.

## Reactions to an immunisation ##

Allergic or adverse reactions to an immunisation may be captured in the GP Clinical System but these are not generally directly associated to the immunisation event.
It has not been considered reliable to link any allergic or adverse reaction to the immunisation record therefore information and reactions will not be included.
For details of allergies or adverse reaction, the Allergies resource must be requested.