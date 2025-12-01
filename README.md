# PTX Interface Specification

Interface between C-ITS On-Board Units (OBU) and ITCS On-Board Computers (IBIS) - released specification versions including Protobuf and JSON schemas

This repository hosts the neutral, multi-vendor **PTX Interface Specification** between
C-ITS On-Board Units (OBUs) and ITCS On-Board Computers (IBIS) used in public transport.

The goal of PTX is to define a stable, interoperable interface so that:

- Different C-ITS OBU vendors can integrate with different IBIS / ITCS systems.
- Implementations share a common, versioned set of messages and semantics.
- Changes to the specification are discussed openly and applied consistently.

## Scope

This repository will contain:

- The **human-readable specification** documents.
- The **Protobuf schemas** of PTX messages, from which JSON is generated.
- The **authoritative JSON Schemas** for PTX messages exchanged on the wire.
- Supporting information, and possibly tools and scripts.

## Status

> **Draft** – initial structure under development.  
> The specification is being prepared collaboratively by representatives of
multiple OBU and IBIS vendors. Contributions and review comments are welcome.

## Governance

The specification is edited and maintained by a group of maintainers from
participating companies. Processes for proposing and approving changes will be
documented in a `GOVERNANCE.md` and `CONTRIBUTING.md` file in this repository.

## License

Unless otherwise noted, the contents of this repository are licensed under
the [Apache License 2.0](LICENSE).

