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

# Opt-Out Registry

## **Overview**

The Liccium Opt-Out Registry is the first system enabling machine-readable opt-out declarations, allowing individual creators and rightsholders to formally express and make their preferences publicly available regarding the use of their content for AI training. Designed in compliance with the DSM Directive and the AI Act, the registry ensures that rightsholders can publicly declare and assert their reservations, preventing unauthorized AI model training and generative AI applications.

Built on a decentralized hash table (DHT) architecture, the Liccium Opt-Out Registry provides a tamper-proof, cryptographically verifiable, and federated system for managing opt-out declarations. The system enables automated discovery and access to machine-readable rights reservations, ensuring that AI developers, platforms, and regulators can systematically recognize opt-out signals and exclude the content from training datasets.

## **Structure**

The registry operates as a distributed key-value store where each entry represents key components of a machine-readable opt-out declaration. These declarations are digitally signed, cryptographically verifiable, ensuring authenticity and immutability of the records.

#### **Keys**

Each entry in the DHT contains the following key components:

* **Declaration ID** – A unique identifier for each declaration.
* **Metadata Hash (CID)** – A content identifier (CID) representing the cryptographic hash of the metadata.
* **ISCC Code** – A standardised International Standard Content Code (ISCC), serving as a fingerprint for the digital content, which allows to reference the actual media file.
* **Timestamp (UNIX)** – A UNIX timestamp marking when the entry was created or modified.

#### **Values**

Each key in the DHT maps to a value that includes:

* **Opt-out Expression** – A machine-readable declaration indicating the ISCC-associated content is opted out of specific uses, such as AI training.
* **Signature of the Timestamp** – A cryptographic signature ensuring the validity of the timestamp.
* **Signature of the Verifiable Credential (VC)** – A cryptographic proof linking the declaration to a legitimate rightsholder.

### **Example Entry**

Below is an example of an opt-out entry stored in the registry:

```
arduinoCopyEditsyxsatxsuefkiirzkxgv-dj7WgARAtoiA4JdeVKxiujtPBafDRzryocZ1e4dTeN826vWc-KEC37U62XOOZFLT5QYHXSFLOFAYX7QGRKQ2RDUZ4OC7CWVLPW74D42Y:
{
  "optout": {
    "TDMAI": false
  },
  "timestamp_signature": {
    "signature": "Timestamp_Token"
  },
  "vc_signature": {
    "signature": "VC_Token"
  }
}
```

## **Integration for AI Model Providers**

The Opt-Out Registry is designed for seamless and effortless integration by AI model providers, web crawlers, and media verification platforms. Setting up a node is incredibly simple for AI model providers, requiring minimal configuration to gain real-time access to machine-readable opt-out declarations. This ensures that rightsholders’ reservations regarding AI training can be automatically acknowledged, allowing AI developers to comply with copyright regulations and AI governance laws without complex infrastructure adjustments.

By operating a node, AI developers gain direct and automated access to opt-out declarations, allowing them to systematically match ISCC codes from their datasets with those declared by rightsholders. This facilitates compliance with copyright and AI transparency obligations while streamlining dataset curation processes.

### **How It Works**

1. Setting up a registry node – AI model providers deploy a node within the Liccium federated registry network, granting them real-time access to opt-out declarations with minimal setup effort.
2. Generating ISCC codes from training data – As part of their dataset processing, AI developers create ISCC fingerprints for media assets intended for training. This allows for a content-derived, format-independent identification of the data.
3. Performing a vector search – AI model providers perform a vector-based similarity search to match ISCC codes from the training data with those registered by rightsholders. This ensures that near-duplicate content and variations of the same work are identified, even if the media file has been slightly modified.
4. Matching against the opt-out registry – AI model providers can automatically query the Liccium Opt-Out Registry to compare ISCC codes from the training data with those registered by rightsholders.
5. Resolving rights reservations – If a match is found, AI model providers can resolve the opt-out declaration, verifying its authenticity, timestamp, and cryptographic signatures.
6. Enforcing compliance – AI providers exclude matching content from their training datasets as per the declared opt-out preferences, ensuring legal and ethical compliance with AI transparency and copyright laws.

### **Regulatory Compliance and Benefits**

By integrating the Liccium Registry Node, AI model providers achieve full regulatory compliance with EU copyright and AI laws while reducing administrative overhead. The system provides direct, machine-readable access to opt-out declarations, removing reliance on manual rights management.

The ability to perform a vector-based search enhances the effectiveness of compliance by identifying near-duplicate content, even when format changes or minor modifications have been applied. This ensures that rightsholders’ opt-out preferences are enforced comprehensively, reducing the risk of unauthorized content use.

This plug-and-play integration empowers AI developers to maintain regulatory compliance while streamlining the content exclusion process, ultimately fostering a more ethical and legally sound approach to AI training. By adopting the Liccium decentralised registry infrastructure, AI model providers contribute to a transparent and responsible AI ecosystem while safeguarding compliance and risk mitigation in their operations.
