# Metadata Binding

Liccium’s approach to metadata binding introduces a reliable and tamper-evident way to associate rights and metadata with digital content – without embedding any information into the file itself. Instead of relying on traditional in-file metadata or watermarking (which can be stripped, altered, or lost when metadata is removed), Liccium uses externally stored declarations – sometimes referred to as 'sidecar files' – that are cryptographically linked to the content via the International Standard Content Code (ISCC).

These external declarations include structured (FAIR) metadata, copyright claims, and usage preferences, signed by creators or rightsholders. The ISCC acts as a content-derived identifier and fingerprint, ensuring that metadata remains verifiably attached to a specific version of a work, even when the file is modified, compressed, or shared across platforms.

This approach avoids the pitfalls of embedded metadata while preserving a robust and decentralised verification mechanism. The metadata can be published in open registries, and retrieved or validated at any point – enabling trust, transparency, and traceability across content lifecycles.

By externalising metadata and maintaining a verifiable link to the original work, Liccium supports a flexible and future-proof model for content authentication, aligned with the demands of AI transparency, copyright compliance, and sustainable content governance.

<figure><img src="../.gitbook/assets/metadata binding (2).png" alt="" width="375"><figcaption></figcaption></figure>

### **Key Advantages of Metadata Binding via External Declarations**

#### **Resilience to File Modification:**

Rights declarations and metadata remain verifiable even if the original media file is altered, reformatted, or stripped of embedded metadata. The binding is content-based, not file-dependent.

#### **Scalable Rights and Policy Management:**

Enables large-scale, automated management of copyright claims, licensing preferences, and usage policies across vast content inventories, including entire platforms or publishing ecosystems.

#### **Modular and Flexible Metadata Models:**

Allows seamless integration of domain-specific schemas, legal frameworks, or custom metadata extensions through plugin architectures – adaptable to the needs of diverse sectors such as publishing, photography, music, or scientific research.
