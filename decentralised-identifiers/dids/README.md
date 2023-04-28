# DIDs

Verifiable credentials and decentralised identifiers (DIDs) are closely related technologies that are often used together to provide secure and decentralised digital identity systems.

Decentralised identifiers (DIDs) are unique identifiers that can be used to identify individuals, entities, or other subjects, objects or even machines across multiple systems and networks. DIDs provide a way to create and control digital identities without relying on centralised identity providers. They are designed to be persistent, globally resolvable, and under the control of the individual or entity they represent. DIDs can be used in a wide range of applications, including decentralised authentication, access control, and digital asset management. They can also serve as a means to authenticate and authorise digital transactions, such as the issuance and presentation of verifiable credentials.

{% code overflow="wrap" %}
```
DECENTRALIZED IDENTIFIERS (DIDs) v1.0, CORE ARCHITECTURE, DATA MODEL, AND REPRESENTATIONS, ABSTRACTS

"Decentralized identifiers (DIDs) are a new type of identifier that enables verifiable, decentralized digital identity. A DID refers to any subject (e.g., a person, organization, thing, data model, abstract entity, etc.) as determined by the controller of the DID. In contrast to typical, federated identifiers, DIDs have been designed so that they may be decoupled from centralized registries, identity providers, and certificate authorities. Specifically, while other parties might be used to help enable the discovery of information related to a DID, the design enables the controller of a DID to prove control over it without requiring permission from any other party. DIDs are URIs that associate a DID subject with a DID document allowing trustable interactions associated with that subject.

Each DID document can express cryptographic material, verification methods, or services, which provide a set of mechanisms enabling a DID controller to prove control of the DID. Services enable trusted interactions associated with the DID subject. A DID might provide the means to return the DID subject itself, if the DID subject is an information resource such as a data model."

```
{% endcode %}

Source: [https://www.w3.org/TR/did-core](https://www.w3.org/TR/did-core/)
