# Access and resolution

Declarations are useful when others can find them. Liccium provides several ways for platforms, AI developers, retailers, intermediaries and other parties to discover, resolve and verify declarations published to the Liccium Registries.

## Search API

The Search API finds declarations by ISCC. Because ISCC codes are similarity-preserving, a party that holds a copy of an asset – even a modified or re-encoded one – can generate its ISCC and find declarations for the same or similar content. Results include similarity information and the provenance chain of each declaration.

## Metadata API

The Metadata API retrieves the full record of a declaration by its identifier (CID): the public metadata, plugin information, declarer identity, credentials, signatures and timestamps. It enables:

* verification of content and its declared rights by platforms and their users;
* compliance checks on content use, licensing conditions and AI preferences at scale;
* recognition of redacted and deleted declarations through explicit status signals.

## Registry nodes

Organisations can operate their own nodes within the federated registry infrastructure, using peer-to-peer synchronisation.

| Node type             | Purpose                                                                                                                                  |
| --------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| Declaration registry  | Media organisations, membership organisations or platforms host and manage their own registry for their declarations and rights metadata |
| Verification registry | Platforms and AI developers synchronise large volumes of declaration metadata for fast, local verification                               |

Registry operators can define governance rules, access permissions and metadata structures for their sector.

## Access terms

API access, metadata resolution and peer-to-peer node synchronisation are offered as separate services and are not included in declaration processing or hosting, unless agreed otherwise.

API references for the Search API and Metadata API are available on the [Liccium API and Developer Platform](https://dev.liccium.com).&#x20;
