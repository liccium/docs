# TDM·AI 𐂂 – Asset-Based Opt-Out

## Making an asset-baset opt-out declaration

TDM·AI is a protocol that lets creators and rightsholders bind machine-readable opt-out declarations for text and data mining (TDM) directly to their digital content. It is specifically designed to effectively exclude content from unauthorised data sets used to train models and applications of generative AI, making use of the benefits of the International Standard Content Code (ISCC) and[ ](https://docs.creatorcredentials.com/)Creator Credentials.

<figure><img src="../.gitbook/assets/tdmai-deer.png" alt="" width="375"><figcaption><p>"Deer AI – Please remove our content!"</p></figcaption></figure>

### Motivation

In the evolving digital landscape, there's an urgent need for creators and rightsholders to control how their content is used, especially concerning AI training. TDM·AI addresses this need by providing a standardized method for machine-readable declarations, ensuring that AI developers can easily recognize and respect these preferences.

### Recommendation

Liccium's TDM·AI protocol describes the method of "soft-binding" rights reservations to ISCC codes, such as an opt-out declaration. To be effective, rights reservations must be:

* **Inseparably bound to the content** (unit, work or asset based approach), allowing sharing and distribution of content;
* Easily discoverable, accessible and **machine-readable** (legal requirement in the EU);
* Functional when **content already has been shared and distributed**;
* Resilient to content manipulation or alteration;
* **Resilient to the removal of embedded metadata** and visible or invisible watermarks;
* Containing verifiable attribution through digital signatures and certificates which authenticate the declaration's source and prevent false claims;
* **Functional for all media types and file formats**;
* Utilising verifiable timestamps;
* Based on reliable and transparent international standards (ISO, W3C).

For more detailed information, visit the [TDM·AI documentation](https://docs.tdmai.org/).

{% embed url="https://tdmai.org" %}
TDM·AI Protocol
{% endembed %}

### Key Components

#### International Standard Content Code (ISCC)

The ISCC is an open system for content-derived identification of digital media across various formats, including text, image, audio, and video. It allows for the generation of unique identifiers without the need for prior registration, ensuring robustness even when metadata is removed or content is altered.

#### Creator Credentials

Creator Credentials are cryptographically verifiable credentials based on W3C recommendations. They provide a self-sovereign, portable, and interoperable framework for digital identity management, enhancing trust and authenticity in declarations made by creators and rightsholders.

#### Metadata Binding Approaches

TDM·AI proposes a "soft-binding" method, associating rightsholder preferences with content-derived identifiers like ISCC codes. This approach ensures that preferences remain linked to the content even if metadata is stripped or the content is modified.

## Protocol Specification

The TDM·AI protocol defines machine-readable declarations for rightsholders to specify their preferences regarding TDM for AI training purposes. These declarations can either prohibit or permit the use of content for training generative AI models.

### **Example of an Opt-out Declaration:**

{% code overflow="wrap" %}
```json
{
  "iscc": "ISCC:KEC7VSV5QH7FTV7N5YVD5UMF4TUKFFGDGCOI4UDFKE4FNPW6C3L7J2Y",
  "TDMAI": false,
  "TDMAI_summary": "Content must not be used for training generative AI.",
  "TDMAI_policy": "Automated analysis of the work to extract information from it, especially about patterns, trends, and correlations for the purpose of training models and applications of generative AI, is reserved. Text and Data Mining (TDM) is permitted for general-purpose AI systems that do not generate synthetic audio, image, video, or text content and for scientific research purposes or for temporary acts of reproduction as provided for in Article 5(1) of Directive 2001/29/EC."
}
```
{% endcode %}

For more detailed information, visit the [TDM·AI documentation](https://docs.tdmai.org/).

{% embed url="https://tdmai.org" %}
