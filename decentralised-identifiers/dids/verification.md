# Verification

Decentralised identifiers and VCs enable trust without the need for permission from centralised authorities. They can be cryptographically verified by anyone to ensure that they have not been tampered with or falsified.

Verification requires a first step involving verifying the identity of the credential issuer. This can be accomplished by retrieving the DID document from the .well-known domain of the did:web and verifying whether the issuer is a trusted entity. The public key, signature, and payload from the DID document can be used to verify the credentialSubject.

If the verifiable credential is related to an ISCC declaration, the credentialSubject will contain a did:pkh or a did:ethr. In technical terms, a declaration can be considered valid if the wallet of the party making the declaration matches the did:pkh or did:ethr referenced in the “id” field of the VC's “credentialSubject” payload.

{% hint style="info" %}
Liccium uses the Veramo JavaScript framework to issue and verify DIDs and verifiable credentials.
{% endhint %}
