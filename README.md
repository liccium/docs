---
cover: .gitbook/assets/Liccium horizontal 1990-480.png
coverY: 0
layout:
  width: default
  cover:
    visible: true
    size: hero
    mask: none
  title:
    visible: false
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

# Introduction

***

## Introduction

Liccium is software for content authentication and rights management. It enables creators and rightsholders to sign their original works and publish verifiable declarations about them – stating authorship, rights and licensing terms, preferences on AI training, and the extent of any AI involvement in creation. Supported by Verifiable Credentials, these declarations establish who made a claim and when, creating a reliable basis for attribution, licensing and authenticity.

### How Liccium works

Liccium does not embed information in the file. Each declaration refers instead to a content fingerprint (ISO 24138) derived from the work itself. Since anyone holding a copy can regenerate the fingerprint independently, the declaration remains discoverable wherever the work travels – even after it has been renamed, converted, re-encoded or stripped of its metadata.

Declarations are published to public, federated registries rather than a single central database. There, people and automated systems can identify a work, confirm the origin and integrity of the claims made about it, and resolve its rights, licences and associated metadata.

Because declarations are separate from the file, they can also be made for works that have already been distributed, and updated as licensing terms, preferences or regulatory requirements change – while the history of earlier declarations remains on record.

### Who Liccium is for

Liccium serves those who make claims about content, and those who need to act on them.

|       | Creators                       | Rightsholders                                               | Intermediaries                                          |
| ----- | ------------------------------ | ----------------------------------------------------------- | ------------------------------------------------------- |
| Image | Photographers, illustrators    | Stock photo platforms, publishers, photo licensing agencies | News agencies                                           |
| Audio | Bands, songwriters, podcasters | Record labels, music publishers, studios                    | Music distributors, collective management organisations |
| Text  | Authors, journalists, bloggers | Publishers, literary agencies                               | News and ebook distributors, libraries                  |
| Video | Video creators                 | Producers and broadcasters                                  | Video distributors                                      |

Individual creators use the [Liccium Desktop app](https://claude.ai/chat/products/liccium-desktop-app/README.md) to fingerprint their work on their own computer and publish declarations. Media organisations use [Liccium B2B Services](https://claude.ai/chat/liccium-b2b-services/README.md) to declare entire catalogues from their existing systems through an API.

Digital platforms, AI developers and regulators access the registries to check licensing terms, respect reservations of text and data mining rights, and recognise disclosures of AI involvement. Internet users can look up the provenance of content they encounter and see who claims to have made it, under which terms it is offered, and whether AI was involved.

### Why it matters

Digital content now circulates faster and further than the information that describes it. Metadata is routinely stripped or altered as files are shared, compressed and republished, and watermarks can be removed or degraded. As a result, authorship, rights and licensing terms are lost precisely where they are needed.

Generative AI has sharpened the problem in two ways. Synthetic and manipulated media are produced at a scale that makes it increasingly difficult to distinguish human-created from AI-generated content, and copyrighted works are used to train AI models, often without permission or compensation.

Liccium addresses this with three capabilities:

* Persistent provenance – declarations remain connected to the content through its fingerprint, even when files are modified or metadata is removed.
* Machine-readable rights – rightsholders state in a structured form whether content is openly available, licensed under certain conditions, or reserved from uses such as AI training.
* Accountable use – AI developers, platforms and regulators can consult the registries systematically, so that the use of content and the composition of training data can be checked against the stated terms of rightsholders.
