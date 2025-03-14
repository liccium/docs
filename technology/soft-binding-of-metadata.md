---
layout:
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
---

# Soft Binding of Metadata

Soft binding represents a new approach to securely linking rights and metadata to digital content without embedding them directly into the media file itself. Instead, metadata and rights declarations are stored externally and cryptographically bound to the content using ISCC codes. This ensures that rights and metadata remain discoverable, accessible, and verifiable independently of the original file, even if the file is modified, converted or metadata is removed. Unlike traditional ‘hard binding’ methods such as C2PA, where metadata is embedded in a file and can be removed, soft binding externalises the metadata while maintaining a cryptographically verifiable link to the content. Soft Binding represents a major advance in digital content authenticity, providing a flexible, tamper-proof and interoperable solution that fits into Liccium's broader vision for decentralised content authentication.

<figure><img src="../.gitbook/assets/soft binding@2x.png" alt="" width="375"><figcaption><p>Liccium Soft-Binding</p></figcaption></figure>

Key advantages of Soft Binding include:

* **Metadata Resilience:**\
  Metadata and rights declarations remain intact and verifiable, even if the original content file is modified or metadata is removed.
* **Scalable Rights Management:**\
  Enables automated, large-scale management of rights declarations, licensing terms, and metadata across entire industries or platforms.
* **Flexible Metadata Integration:**\
  Supports integration of industry-specific or custom metadata through modular plugins, allowing tailored rights management solutions for diverse sectors and content types.



{% hint style="info" %}
<img src="../.gitbook/assets/ISO-logo.png" alt="" data-size="line"> Following the successful publication of ISO 24138 ISCC, ISO TC 46/SC 9/WG 18 will continue with a technical report (TR) on “soft binding” to enhance digital content authenticity standards. [https://www.iso.org/committee/48836.html](https://www.iso.org/committee/48836.html)
{% endhint %}
