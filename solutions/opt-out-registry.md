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

# Opt-out Registry

Liccium lets creators and rightsholders opt their works out of AI training. They publish a machine-readable statement that they reserve their rights – meaning the work may not be used for text and data mining (TDM), including AI training, without their permission. These opt-outs are stored in the Opt-Out Registry, where AI developers, web crawlers and platforms can find them and act on them.

Each reservation is published as a signed, timestamped declaration that refers to the content fingerprint (ISO 24138) of the work. Because anyone holding a copy of the work can regenerate the fingerprint, the reservation can be found wherever the work appears – independent of the website it was found on or the metadata it still carries.

{% embed url="https://optout.directory" %}

## The legal context

Under EU copyright law, anyone may use lawfully accessible content for text and data mining – including AI training – without asking permission. This is an exception to copyright, set out in Article 4 of the Directive on Copyright in the Digital Single Market (Directive (EU) 2019/790).

Creators and rightsholders have the right to opt out of this exception. To do so, they must reserve their rights explicitly – and for content published online, in a machine-readable form. If they do not opt out, AI developers may use their works for training. The EU AI Act requires providers of general-purpose AI models to put in place a policy to identify and comply with such reservations

## Why existing methods fall short

Rights reservations are currently expressed in two ways, and both have limits in practice:

* Domain-level signals – such as robots.txt or the W3C TDM Reservation Protocol (TDMRep) on a website – express the policy of the website operator. They cannot express the preferences of each individual rightsholder whose works appear on that website, and they no longer apply once a work is copied to another domain.
* Metadata embedded in the file can be removed in seconds – deliberately, or as a side effect of conversion, compression or redistribution. When the metadata is gone, so is the reservation.

Reservations expressed in trade metadata, for example in ONIX records exchanged between publishers and retailers, do not reach AI developers at all.

## Registry-based reservations – the TDM·AI protocol

The Opt-Out Registry adds a layer that is independent of where a work is hosted and of the metadata embedded in it. It is based on TDM·AI, an open protocol for registry-based opt-out declarations. Under TDM·AI, a reservation is connected to the work through its content fingerprint (ISO 24138) – a method known as soft binding – and stored in federated registries. It remains discoverable when the work has been copied to another domain, converted to another format or stripped of its metadata, and it can be made for works that have already been distributed.

Each reservation under TDM·AI is:

* connected to the content itself, not to a file, a location or embedded metadata;
* machine-readable, using the TDM·AI vocabulary;
* signed by the declarer, and supported by certificates or Verifiable Credentials that identify who made the reservation;
* timestamped by a trusted Time Stamping Authority, recording when it was made;
* applicable to all media types – text, images, audio and video;
* resolvable by anyone, through the registries and APIs;
* based on international standards – ISCC (ISO 24138) for content identification, and W3C Verifiable Credentials and Decentralized Identifiers for declarer identity.

A reservation can be updated or withdrawn by the declarer at any time. The history of earlier declarations remains on record.

The protocol specification is published on [tdmai.org](https://tdmai.org).

{% embed url="https://tdmai.org" %}

## Making a reservation

| Who                                                  | How                                                                                                  |
| ---------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| Individual creators and rightsholders                | With the TDMrep plugin in the Liccium Desktop app – for a single work, a folder or an entire library |
| Publishers, agencies, labels and other organisations | Through the Declaration API of Liccium B2B Services – for entire catalogues, from existing systems   |

A declaration states whether the work is opted out, and can link to a policy page with licensing terms – for example where AI developers can request a licence. The same declaration can also carry a FAIA disclosure of AI involvement in the work.&#x20;

## Finding and respecting reservations

AI developers, web crawlers and platforms can check works against the registry before using them:

1. Generate ISCC codes for the works in a data set, as part of data collection or processing.
2. Search the registry by ISCC. Because ISCC codes are similarity-preserving, the search also finds reservations for modified versions of a work – cropped, re-encoded or converted.
3. Resolve the declaration and check its signature, timestamp and declarer.
4. Act on the reservation – exclude the work from training, or obtain a licence under the terms the rightsholder has linked to.

## Benefits for AI developers

Under the EU AI Act, providers of general-purpose AI models must have a policy to identify and comply with opt-outs from AI training. The Opt-Out Registry gives them a machine-readable source for these opt-outs that does not depend on where a work was found or on the metadata it carries. It replaces manual checks of each rightsholder's preferences.

Because ISCC codes are similarity-preserving, a search also finds opt-outs for modified versions of a work – cropped, re-encoded or converted. Each opt-out is signed and timestamped, so a developer can document which works were checked, which opt-outs were found, and when the opt-out was made. That record can support their copyright compliance policy and their reporting obligations.

## What a reservation does

An opt-out states the rightsholder's reservation in a form that can be found and verified. It does not technically prevent the use of a work, and it does not remove works from data sets that have already been collected. Its effect depends on AI developers and other parties checking the registry and respecting what it states – which the legal framework increasingly requires of them.

## Accessing the registry

The registry can be accessed in three ways, depending on the volume of content to be checked.

| Access                      | Description                                                                                                                                                                                                                                       |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Optout.directory            | The public interface to the registry. Anyone can search opt-outs by ISCC or declaration ID, view the associated metadata and check the signatures.                                                                                                |
| Search API and Metadata API | For automated checks. The Search API finds opt-outs by ISCC, including for modified versions of a work; the Metadata API retrieves the full, signed declaration. Documented on the [Liccium API and Developer Platform](https://dev.liccium.com). |
| Reader node                 | A registry node that runs on your own infrastructure and synchronises all declarations, for checking large data sets locally – without sending queries to an external service.                                                                    |
