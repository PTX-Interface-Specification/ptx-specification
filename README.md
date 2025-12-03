# PTX Interface Specification

This repository hosts the neutral, multi-vendor **PTX Interface Specification** between
C-ITS On-Board Units (OBUs) and ITCS On-Board Computers (IBIS) used in public transport.

> PTX stands for "Public Transport to Everything", inspired by the term "V2X"

## What is the PTX Interface Specification?

The **PTX Interface Specification** defines an open, vendor-neutral interface
between **C-ITS On-Board Units ("OBU")** and **ITCS On-Board Computers ("IBIS")**
used in **public transport vehicles**. It enables interoperable exchange of
vehicle position, operation status, service identifiers, and C-ITS events
between independent onboard systems.

PTX improves the public transport technology ecosystem by:

- providing a **standardized communication interface** between OBU and IBIS
- reducing vendor lock-in and enabling **multi-vendor competition**
- simplifying **tendering** processes, in particular for OBUs
- ensuring long-term **interoperability and lifecycle flexibility**
- supporting future extensions through semantic versioning
- enabling modular upgrades and independent replacement of hardware components

The specification is openly published to support operators, authorities,
vendors, and integrators in building interoperable, future-proof public
transport fleets.

PTX is especially relevant for:
- Public transport operators (PTOs) and fleet owners  
- Public transport authorities (PTAs) and regulators  
- C-ITS OBU vendors  
- ITCS or AVL system vendors  
- Integrators, engineering consultancies

The goal of PTX is to define a stable, interoperable interface so that:

- OBUs and IBISs from different vendors are interoperable
- Implementations share a common, versioned set of messages and semantics
- Changes to the specification are discussed openly and applied consistently

For a summary of expected benefits to operators and procurement, see [BENEFITS.md](BENEFITS.md).

## Scope

This repository contains:

- The **human-readable specification** documents
- The **Protobuf schemas** of PTX messages, from which JSON is generated
- The **authoritative JSON Schemas** for PTX messages exchanged on the wire
- Supporting information, and possibly tools and scripts

## Governance

The specification is edited and maintained by a group of maintainers from the
participating companies. The maintainers are listed under "Contact Persons"
within the specification.

## Evolution

The PTX Interface Specification uses **semantic versioning** (major.minor.patch):

- **Patch releases** (e.g. `2.0.1`) are documentation-only updates and do  
  **not** modify the wire format. Protobuf and JSON Schema remain unchanged.

- **Minor releases** (e.g. `2.1.0`) will introduce new messages or fields.  
  In such cases, a new schema version appears under dedicated
  directories such as `schemas/proto/v2.1/`.

- **Major releases** (e.g. `3.0.0`) will break compatibility.  
  The express goal is not having to create any major releases in the future.

A PTX specification version **2.1.0** is planned for release by the end of **2026**.
It will be **fully compatible** with version 2.0.x and will introduce enhancements
with a particular focus on **safety-related functionality**.

## License

Unless otherwise noted, the contents of this repository are licensed under
the [Apache License 2.0](LICENSE).  
The PDFs are provided under the CC BY 4.0 licence .

