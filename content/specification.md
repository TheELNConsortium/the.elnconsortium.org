---
featured_image: "/bg.webp"
description: The ELN Specification
---

# Specification

The ELN file format is based on Research Object Crate (RO-Crate) specification.

It can be summarized as a zipped RO-Crate.

The up-to-date specification is available on the GitHub respository:

[SPECIFICATION.md](https://github.com/TheELNConsortium/TheELNFileFormat/blob/master/SPECIFICATION.md)

## Verify a .eln

Use this app to verify a .eln validity: https://check-eln.streamlit.app/

## IANA media type

The `.eln` is an officially recognized media-type by IANA: [vnd.eln+zip](https://www.iana.org/assignments/media-types/application/vnd.eln+zip).

# FAQ | Frequently asked questions

We regularly encounter recurring, incorrect criticisms of the .eln file format. These points have previously been addressed, yet they continue to resurface.

## Myth 1: The .eln file format does not allow semantic annotation
This is incorrect. The .eln file format enables semantic annotation by allowing each entry to include an identifier that can reference an external semantic definition (for example, an ontology PURL). This mechanism supports explicit linking to controlled vocabularies and ontologies, facilitating interoperable, machine-readable semantics.

## Myth 2: The .eln file format does not allow for profile validation
This is not true. At its core, the .eln file format is built around a JSON‑LD representation that can be validated against JSON Schema using a wide range of existing tools. Example files are validated as part of the publishing workflow, and stricter or custom validation profiles can be implemented for specific use cases when required.
