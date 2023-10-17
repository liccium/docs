# The credential subject

<figure><img src="../../.gitbook/assets/credential subject.png" alt=""><figcaption></figcaption></figure>

Liccium will support issuance and verification, upload, and export of verifiable credentials of various types and subjects that can be used in different scenarios, adhering to the “open world assumption” of the Verifiable Credentials Data Model v1.1. This approach allows for the issuance and use of VCs to be flexible and adaptable in various contexts.

<pre data-overflow="wrap"><code>EXTENSIBILITY

"One of the goals of the Verifiable Credentials Data Model is to enable permissionless innovation. To achieve this, the data model needs to be extensible in a number of different ways. The data model is required to:

Model complex multi-entity relationships through the use of a graph-based data model.
Extend the machine-readable vocabularies used to describe information in the data model, without the use of a centralized system for doing so, through the use of linked data.
Support multiple types of cryptographic proof formats through the use of Data Integrity Proofs and a variety of signature suites listed in the Linked Data Cryptographic Suites Registry (LDP-REGISTRY).
Provide all of the extensibility mechanisms outlined above in a data format that is popular with software developers and web page authors, and is enabled through the use of JSON-LD.

This approach to data modelling is often called an open world assumption, meaning that any entity can say anything about any other entity. While this approach seems to conflict with building simple and predictable software systems, balancing extensibility with program correctness is always more challenging with an open world assumption than with closed software systems."

Source: <a data-footnote-ref href="#user-content-fn-1">https://www.w3.org/TR/vc-data-model/#extensibility</a>

</code></pre>



[^1]: 
