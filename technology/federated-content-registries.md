---
layout:
  width: default
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
  tags:
    visible: true
  actions:
    visible: true
  anchors:
    visible: true
---

# Federated Content Registries

Creators, rightsholders and organisations can publish verifiable declarations about digital content to federated registries. These declarations associate content-derived ISCC identifiers with rights, licences, provenance, AI-related preferences and other metadata.

Instead of relying on one central database, different registries can serve different sectors, communities, jurisdictions or use cases while remaining interoperable through common technical standards.

## Verifiable declarations

Each declaration links an ISCC identifier to structured metadata and is digitally signed by the declaring party. This makes the origin and integrity of the declaration independently verifiable.

Declarations can contain information such as:

* rights and licences
* provenance and attribution
* AI-use preferences (opt-out)
* AI-transparency flags (FAIA)
* product and descriptive metadata

The media files themselves do not need to be stored in the registry. Registries contain the declarations and the information required to discover, resolve and verify them.

## Independent registries, common infrastructure

Registries can be operated independently by publishers, collecting societies, public institutions, creator organisations or other trusted actors.

Each operator can define its own governance model, access rules and requirements for declarers while using the same technical mechanisms for content identification, declarations and verification.

This enables sector-specific, local or purpose-specific registries to coexist without requiring a single central registration authority.

## Federation and aggregation

Federation connects independent registries.

Participating registries publish synchronisation records that can be replicated between nodes. A node can synchronise records from one or multiple registries and create an aggregated local view across them.

This allows declarations from independently operated registries to be discovered and verified through a common infrastructure while registry operators retain control over their own services and metadata.

## Access at any scale

Declarations can be accessed through APIs or through synchronised registry nodes.

**APIs** provide straightforward access for individual lookups and application integrations.

For high-volume use, organisations can **operate their own node and synchronise selected registries directly into their infrastructure**. Platforms, search engines and AI providers can then search and match registry records locally without making an external API request for every asset.

This supports continuous synchronisation, multi-registry aggregation and large-scale content matching.

A newly published declaration can therefore become available to participating systems within seconds.

## Open and configurable

Federation does not require every registry to follow the same governance model or expose the same metadata.

Registry operators determine who can publish declarations, which credentials are required and which information is publicly accessible or permissioned.

Common standards ensure that participating registries remain interoperable and that declarations can be discovered and verified across the wider ecosystem.

## A registry ecosystem instead of a central database

The objective is not to replace existing rights and metadata systems with a new central database.

Federated content registries provide a common infrastructure through which independently governed systems can publish, exchange, discover and verify declarations about digital content.

This creates a basis for a European infrastructure of federated registries for digital content: local governance, common standards and interoperable access.
