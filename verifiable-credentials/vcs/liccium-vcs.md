# Liccium VCs

The Liccium app serves as a VC issuer service by implementing and managing various verification processes.

By way of a social verification process, users can confirm their ownership of social media accounts by linking their wallet address to their social profiles using authentication and cryptographic techniques.

The app also facilitates domain verification. This involves adding a digital signature as a TXT verification record to the DNS records of a user's domain to demonstrate ownership and establish trust in content declarations and claims. By utilising an established trust framework and infrastructure on the web and providing relevant personal identifiable information, the app and its process enhances the credibility of the verification.

In its role as a witness, the Liccium app will supervise challenges and digital signatures to establish a connection between the wallet address of a declaring party and their social media accounts or internet domain ownership at the time of declaration.

Once these procedures are completed successfully, Liccium issues the respective VCs to the users.

* VCs are **self-sovereign**, which means that creators and rightsholders are the primary owner and controller of their credentials. They can choose where to host, and when and how to use the credentials. The holder can also control the level of access granted to others and can revoke access at any time;
* VCs are **portable**, which means that once issued the holder can move credentials between different systems and platforms. The holder may also decide to use them with other applications or services as needed without loss of information or functionality;
* VCs are **interoperable**, which means that credentials issued by one system can be recognized and accepted by other systems, even if they are built on different technologies or operated by different organisations. Third party Applications can independently verify VCs that use different DID methods to identify the holder or issuer, using different DID methods to access public keys, and different encryption methods (e.g., ECDSA, EdDSA);
* VCs can also be **restricted in duration**. This means they support the ability to set a time limit on how long a verifiable credential is valid. Limited validity can be useful for credentials that expire, such as professional licence or certifications;
* VCs are **revocable**, which means that they can be revoked or cancelled in case of expiry. This is important for maintaining the integrity of the credential system and ensuring that only valid and accurate information is being shared. The revocation can be initiated by the issuer of the credential or by the individual who owns the credential. It can be enforced by the systems that recognize and accept the credential.

{% hint style="info" %}
Liccium uses the Rebase protocol to issue and verify portable and interoperable credentials (VCs) that can create a social graph and serve as identity verifications across social media, DNS, etc.
{% endhint %}
