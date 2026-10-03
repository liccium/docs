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

# Liccium B2B Services

Liccium B2B Services enable organisations to generate content fingerprints (ISO 24138) for their media assets, connect them to rights information, product metadata, provenance information and AI-related declarations, and publish these as signed, verifiable declarations to the Liccium Registries.

The services are designed for organisations that manage large catalogues – publishers, stock and photo agencies, music labels, platforms, libraries, archives and membership organisations. They are accessed through an API and integrate with existing content, product and asset management systems.

## How it works

1. **Fingerprint** – your organisation generates ISCC codes for its assets within its own environment. The assets do not leave your infrastructure.
2. **Describe** – you add the ISCC codes to your existing product and rights metadata, structured in the formats accepted by the API, including machine-readable AI preferences and AI transparency information.
3. **Sign** – your organisation signs each declaration with its own key, authenticated by an electronic seal certificate or a Verifiable Credential.
4. **Declare** – the Declaration API validates the declaration, verifies the signature and credentials, adds a trusted timestamp and publishes it to the Liccium Registries.
5. **Resolve** – platforms, AI developers, retailers and other parties can regenerate the fingerprint from a copy of an asset and find your declaration through the registries and APIs.

## Service modules

| Module                       | What it does                                                                                                                     |
| ---------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| ISCC generation              | Generates content fingerprints for text, images, audio and video in your own environment                                         |
| Declaration metadata         | Defines the rights, product and AI-related information carried by a declaration, and supports mapping from your existing systems |
| Declaration API              | Validates, timestamps and publishes signed declarations                                                                          |
| Certificates and credentials | Authenticates your organisation as the declarer, with keys under your exclusive control                                          |
| Managing declarations        | Updates, supersedes, redacts and deletes published declarations                                                                  |
| Access and resolution        | Makes declarations available through the Metadata API, the Search API and registry nodes                                         |

## What your organisation can declare

* rights information and licensing terms;
* product and title metadata, links and standard identifiers;
* reservations of text and data mining rights and other machine-readable AI preferences;
* AI transparency information, using FAIA;
* sector-specific metadata, for example IPTC for images.

Declarations carrying AI preferences are also published to the TDM·AI registry ([Optout.directory](https://optout.directory)), and declarations carrying FAIA information to the [FAIA registry](https://faia.io).

## Your data stays in your environment

By default, the ISCC generator and any integration components run on servers or cloud infrastructure that your organisation controls. Your assets and internal source data remain within your environment. Liccium receives only the declarations you submit and hosts them in the Liccium Registries.

Your organisation also generates and exclusively controls the keys used to sign declarations. Liccium does not generate, store or have access to your private keys.

## Getting started

Implementing Liccium B2B Services is a joint project. Liccium supports onboarding, metadata mapping and integration, and your organisation provides a technical contact with knowledge of your catalogue and systems.&#x20;

The full technical documentation, API reference and API key management are available on the Liccium API and Developer Platform.

{% embed url="https://dev.liccium.com" %}
