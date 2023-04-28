# ISCC-ID

<figure><img src="../../.gitbook/assets/ISCC Registry.png" alt=""><figcaption><p>Source: <a href="https://testnet.iscc.id/">https://testnet.iscc.id/</a></p></figcaption></figure>

Each declaration of an ISCC on a public blockchain network generates a unique, short, owned, persistent, verifiable, and resolvable identifier called the ISCC-ID.

This identifier is the result of a content declaration, and it resolves to the ISCC, primary declaration metadata, the address of the declaring wallet, and other on-chain data. ISCC-IDs are globally unique even if the same ISCC code is registered multiple times by different declarers on different blockchains.

The ISCC-ID is “owned” by the declarant, and it can be verified that the declaration transaction for a specific ISCC has been cryptographically signed by the private key of the declarer.

{% code overflow="wrap" %}
```
ISCC-ID

"Public ISCC-CODE declarations from different blockchains are monitored by ISCC-OBSERVERs and registered with an iscc-registry via its REST API. The iscc-registry calculates, and indexes ISCC-IDs based on the events received from observers. The resulting ISCC-IDs are identifiers for digital media assets with the following mandatory information attached:

an ISCC-CODE, which is a content-based identifier and fingerprint of a media asset;
a DECLARER, which is the blockchain address of entity that signed a declaration transaction;
a timestamp of the declaration.

An ISCC declaration can optionally provide:

a URL with extended metadata about the digital media asset;
a redirection target that can be used like a URL-shortener (e.g., https://iscc-reg.tld/<iscc-id>);
the blockchain address of a registrar that facilitated the declaration."
```
{% endcode %}

Source: [https://github.com/iscc/iscc-registry](https://github.com/iscc/iscc-registry)
