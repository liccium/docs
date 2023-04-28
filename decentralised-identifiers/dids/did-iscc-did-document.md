# did:iscc DID document

A DID document contains information about a specific decentralised identifier, such as its public key, service endpoints, and other relevant data. It may also include information about the entity or object associated with the identifier, such as its name, description, and other attributes.

In the case of did:iscc, DID documents are generated from immutable data on-chain, optionally including off-chain metadata, which may be referred to in the primary declaration metadata.

All mandatory information required to construct a minimal valid DID document from an ISCC declaration is available on-chain and can be dynamically transformed and presented as a DID document by a DID driver implementation, hosted by ISCC Foundation on [https://did.iscc.id/](https://did.iscc.id/).

The did:iscc DID document contains:

* the native **ISCC code** (see “alsoKnownAs” value);
* the did:pkh, which is used to unambiguously identify the address of the **declarer’s blockchain wallet**, i.e., the controller of the DID document (see “controller” value);
* optionally, the URI (in this case, the IPFS-CID) that may **link to the primary declaration metadata** off-chain (see “serviceEndpoint” value).

{% code overflow="wrap" %}
```
EXAMPLE OF A DID:ISCC DID DOCUMENT

did:iscc:miagwptv4j2z57ci

{
 "@context": "https://www.w3id.org/ns/did/v1"
 "id": "did:iscc:miagwptv4j2z57ci",
 "controller": "did:pkh:eip155:1:0x901ee44e3bddf4bc1c08a2ed229498512f8bcfdc",
 "alsoKnownAs": "iscc:kecycpu3okiudz7tybrk5hz4jgptillat2iw7ty7eyiji4qsk5i353i",
 "service": [{
   "id":"did:iscc:miagwptv4j2z57ci#iscc-metadata",
   "type": "IsccMetadata", 
   "serviceEndpoint": "ipfs://bafybeiccys7kilr3rynlhoelrdn6ragpbfoti73h4e3oszbgd5inthicja/iscc-metadata/43.json"
 }]
} 
```
{% endcode %}

Example DID document, source: [https://github.com/iscc/iscc-registry](https://github.com/iscc/iscc-registry)
