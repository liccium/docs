# The levels of trust

The Liccium app employs wallet software as the foundation for user verification. By creating a digital signature with the private key of the wallet, the app establishes a “base level” of trust. Through a successful digital challenge during the sign-in or sign-up process, the user's control of the private key of a specific wallet address can be verified.

This cryptographic wallet authentication not only ensures user privacy as well as secure and trustworthy access to the app. It also confirms that a pseudonymous user controls a specific wallet address expressed as did:ethr or did:pkh.

Based on the pseudonymous, decentralised identity established by their wallet, content creators and rightsholders can choose to disclose varying levels of personal attributes and information about their social graph or personal identity to establish trust in their declarations, assertions, or claims.

By employing different self-verification methods and utilising institutional credentials from trust services, the level of trust in the declarations will be significantly increased.

Self-issued credentials gain their authority directly from their users, proving their control of wallets, e-mail accounts, social media accounts, web domains, credit cards, or control of their physical address.

The tables below classify the different levels of trust, the processes involved, the trust bases used to establish them, and the type of credentials.

For self-issued credentials on trust levels 1-6, the Liccium app will act as a witnessing service for the user’s own verification process.

Eventually, the Liccium model aims to scale and become an effective trust and reputation system operating on various trust levels, ranging from social authentication to more sophisticated approaches based on SSI, higher-assurance KYC, advanced or qualified certificates based on novel eIDAS 2 regulation, thereby representing a hierarchical trust model. This will utilise either an existing and established trust framework and infrastructure on the web or a new public-key infrastructure such as the European Blockchain Services Infrastructure (EBSI).

| **Trust Level**                          | **Process**                         | **Trust Base**                                        | **Credential Type** |
| ---------------------------------------- | ----------------------------------- | ----------------------------------------------------- | ------------------- |
| Base Level 1: Pseudonymous               | Cryptographic wallet authentication | Control of private key of a specific wallet address   | Self-issued         |
| Level 2: Self-claimed                    | E-mail verification                 | Control of a particular email account                 | Self-issued         |
| <p></p><p>Level 3: Socially-verified</p> | Social verification                 | Control of specific accounts on social media          | Self-issued         |
| Level 4: Domain-verified                 | Domain verification                 | Control of DNS settings of a specific internet domain | Self-issued         |
| Level 5: Credit / Debit Card             | Use of credit/debit card            | Control of credit/debit card                          | Self-issued         |
|                                          |                                     |                                                       |                     |
| Level 6: KYC                             | Verification of a physical address  | Physical address verification                         | Self-issued         |



In future versions of the Liccium app, self-issued credentials will be augmented by verifiable credentials issued by 3rd-party trust services, where the VC issuer services are utilised as the relevant source of trust. These credentials could be issued by online identity verification services that enable the association of users with governmentally issued personally identifiable information (PII).

An additional level of trust and security is established by using browser certificates such as Let's Encrypt and qualified web authentication certificates (QWAC). This establishes the reputation of the issuer DID (did:web) and the web domain. However, browser certificates rely on a functioning DNS system as the certificates are issued based on the domain name of a website.

To further enhance trust, the legal entity providing the issuer service may acquire and use QCerts for eSeal to sign the creator credentials, providing an additional level of security.

These levels even aim at compliance with the revision of the Regulation on electronic identification and trust services, eIDAS 2.0.

| **Trust Level**                                     | **Process**                                       | **Trust Base**                                      | **Credential Type**     |
| --------------------------------------------------- | ------------------------------------------------- | --------------------------------------------------- | ----------------------- |
| <p></p><p>Level 7: Online Identity Verification</p> | Identity verification by 3rd-party trust services | Governmentally issued PII                           | Issued by trust service |
| Level 8: DID:web certification                      | Certification of did:web                          | Browser certificates \ (e.g., Let’s Encrypt, QWAC)  | Issued by trust service |
| Level 9: DID certification                          | Certification of legal entity                     | Qualified Certificates for eSeal (QCERTS for eSeal) | Issued by trust service |
