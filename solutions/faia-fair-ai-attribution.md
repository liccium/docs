# FAIA – Fair AI Attribution

## Fair AI Attribution (FAIA)

The **FAIA project** (Fair AI Attribution) develops an open, structured framework to disclose the role of artificial intelligence in content creation. FAIA is developed by [**Liccium**](https://liccium.com/) in collaboration with [**Leiden University**](https://www.universiteitleiden.nl/en) and the [**GO FAIR Foundation**](https://www.gofair.foundation/), addressing a growing need for transparency in digital publishing and research.&#x20;

As AI tools become more common in writing, publishing, and media production, transparency is no longer optional - it’s essential for trust, credibility, and compliance. With the increasing integration of generative AI tools – ranging from writing assistants to full content generators – creators, publishers, and academic researchers need a consistent and verifiable way to indicate whether and how AI has contributed to the content. FAIA provides that mechanism.

Implemented as a plugin in the Liccium software, FAIA allows creators to document and share how AI contributed to their work.

<figure><img src="../.gitbook/assets/FAIA-Slide (1).jpg" alt="" width="563"><figcaption><p>(Draft) </p></figcaption></figure>

### Goals and Scope

FAIA enables creators and rightsholders to:

* Disclose **how AI was involved** in the creation or editing of content.
* Align with **regulatory requirements** like the EU AI Act (Art. 50).
* Promote **provenance, reproducibility, and trust** in digital publishing.

The framework is implemented as a **Liccium plugin**, allowing users to flag AI involvement directly within Liccium's declaration and signing interface. These flags are machine-readable, interoperable, and persistently linked to the content.

{% embed url="https://youtu.be/s1mOJFHeCEM" %}
Video Pitch
{% endembed %}

This short video introduces the FAIA initiative. It highlights the problem of AI opacity, emerging regulation like the EU AI Act, and a practical solution for certifying content with verifiable AI involvement.

### Attribution Flags

FAIA introduces a controlled vocabulary for AI contribution, modelled after standards like the **IPTC Digital Source Type**, which can be used for visual content, and aligning with proposals like the **STM Association’s classification system**.&#x20;

{% hint style="info" %}
Recommendations for a Classification of AI Use in Academic Manuscript Preparation:

[https://stm-assoc.org/document/recommendations-for-a-classification-of-ai-use-in-academic-manuscript-preparation/](https://stm-assoc.org/document/recommendations-for-a-classification-of-ai-use-in-academic-manuscript-preparation/)

Guidance for using the IPTC Digital Source Type:

[https://www.iptc.org/std/photometadata/documentation/userguide/#\_guidance\_for\_using\_digital\_source\_type](https://www.iptc.org/std/photometadata/documentation/userguide/#_guidance_for_using_digital_source_type)
{% endhint %}

### Implementation in Liccium

Using the FAIA plugin, users can:

* Select AI involvement types during declaration process.
* Potentially provide details, e.g. provide tool versions and usage context (e.g., "ChatGPT-4, used for summarization").
* Bind this information cryptographically to the content's **ISCC code**, ensuring it travels with the media.

All declarations are verifiable, timestamped, and publicly resolvable via Liccium registries.

### Outcomes and Impact

FAIA promotes ethical publishing practices by:

* Helping creators and researchers **avoid misrepresentation**.
* Supporting **disclosure requirements** from journals, funding bodies, and institutions.
* Enabling platforms and users to **filter or verify content** based on transparency metadata.

It is designed for cross-sector use but initially focuses on **academic and trade publishing** workflows.

{% hint style="info" %}
**Project Partners:**&#x20;

[**Leiden University**](https://www.universiteitleiden.nl/en)

[**GO FAIR Foundation**](https://www.gofair.foundation/)

[**Liccium**](https://liccium.com/)
{% endhint %}
