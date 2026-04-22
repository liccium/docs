# Liccium plugins

Liccium plugins enable the integration of use-case- or industry-specific metadata to declarations or other services provided by 3rd parties to the Liccium app. These plugins enhance the app's generic functionality for creators and rightsholders. With Liccium they can seamlessly embed metadata and bind external metadata to their content, thereby customising the app to their specific needs.

<figure><img src="../../.gitbook/assets/Liccium Plugins@2x.png" alt=""><figcaption><p>Liccium Plugins</p></figcaption></figure>

## IPTC photo metadata

Photographers and photojournalists currently use the IPTC standards to attach technical, descriptive, and administrative metadata or copyright information to their images. With Liccium, they can inseparably bind IPTC photo metadata to their content even if the content has been altered or manipulated, or metadata have been stripped from the content.

<figure><img src="../../.gitbook/assets/IPTC 2@2x.png" alt="" width="375"><figcaption></figcaption></figure>

## AI Preferences (Opt-out)

With the evolving landscape of AI, there's a pressing need for an application that allows content creators and rightsholders to declare their permissions regarding TDM.&#x20;

The EU's DSM Directive on Copyright provides a default condition for TDM, but there's ambiguity when rightsholders want to opt-out or explicitly give permission. The TDM·AI protocol is motivated by the need to:

1. Provide clarity and ease for rightsholders to declare their TDM preferences (reservations or permissions).
2. Offer a decentralised, immutable, and verifiable system for these declarations.
3. Ensure that AI providers and other stakeholders can easily understand and respect these declarations.

Liccium offers a protocol to facilitate machine-readable opt-out declarations for Text and Data Mining (TDM) for AI providers based on the DSM Directive on Copyright 2019/790, Article 4, leveraging the benefits of the International Standard Content Code ([ISCC](https://iscc.codes)) and [Creator Credentials](https://docs.creatorcredentials.com/).

<figure><img src="../../.gitbook/assets/tdmai 2@2x.png" alt="" width="375"><figcaption></figcaption></figure>

The declaration binds a machine-readable declaration to the content by the rightsholder limiting commercial TDM usage.

For more information, please visit the TDM·AI homepage:  [https://tdmai.org/](https://tdmai.org/)

{% embed url="https://tdmai.org" %}
TDM·AI
{% endembed %}

## C2PA Metadata

The Coalition for Content Provenance and Authenticity (C2PA) is developing technical specifications for establishing content provenance and authenticity. They are refining a proposed ISO standard (ISO 22144) that uses capture devices within a trusted execution environment and software applications to certify the source and provenance of media content. Content creators and publishers can use apps that are based on this standard to embed cryptographically verifiable metadata containing information about the asset’s creation and edit actions, copyright, licenses, capture device details, and software used. The assertions are designed to be hashed and gathered into a verifiable claim that is digitally signed, ensuring the integrity of the claim.

Using the Liccium app, users can create a C2PA manifest from their metadata and embed the manifest into media asset. The C2PA method stores information directly within the media file. If embedded metadata is removed or inaccessible, the content can’t be checked for authenticity.&#x20;

That’s why Liccium not only includes C2PA metadata inside the file but additionally creates a separate record of the data outside the file. This record is inextricably connected to the content’s unique fingerprint (ISCC), ensuring the data can still be verified even if it’s removed from the file itself.&#x20;

<figure><img src="../../.gitbook/assets/c2pa@2x.png" alt="" width="375"><figcaption></figcaption></figure>

## FAIR AI Attribution (FAIA)

With generative AI increasingly shaping the production of text, images, audio, and video, creators, publishers, and researchers need a consistent way to indicate whether and how AI has contributed to their content. Without it, readers cannot tell human work from machine output, regulators cannot enforce disclosure obligations, and downstream users cannot assess provenance or reproducibility.

The FAIR AI Attribution (FAIA) framework is motivated by the need to:

1. Enable transparent documentation of AI involvement in content creation.
2. Support compliance with emerging regulatory frameworks, such as Article 50 of the EU AI Act.
3. Strengthen provenance, reproducibility, and trust in digital media and publishing ecosystems.

Each declaration carries one of three flags – HCC (Human-Created Content), AAC (AI-Assisted Creation), or AIG (AI-Generated) – optionally qualified with an activity code that describes the type of contribution plus the information about which system and version was used.

<figure><img src="../../.gitbook/assets/CleanShot 2026-04-22 at 08.54.24@2x.png" alt="" width="563"><figcaption></figcaption></figure>
