# Trust Levels

Liccium enables creators, rights holders, and organisations to make **public and verifiable declarations** about digital content using ISCC fingerprints. Every declaration is cryptographically signed and can include **Verifiable Credentials (VCs)** or **certificates** to establish the **identity and authority** of the declaring party.

However, not every signature carries the same weight. To help platforms, users, and automated systems assess the **reliability and trustworthiness** of a declaration, Liccium defines **four distinct trust levels**. These levels are determined by the **type of credential** used to authenticate the signer and the **verification method** applied.

The trust model is simple, transparent, and extensible. It accommodates everything from pseudonymous creators to fully verified legal entities, and aligns with EU regulatory frameworks.

## Overview of Trust Levels

### **Low – Social Verification**

_User controls a social account (e.g. Bluesky, GitHub, X)._

At this level, a user proves control over a social media account by logging in via OAuth or SSO. Liccium witnesses the login and issues a **self-attested Verifiable Credential (VC)** confirming the user's account ownership. This provides lightweight verification for pseudonymous creators who still want to make verifiable claims tied to a persistent identity.

### **Moderate – Domain Verification**

_User controls a web domain, verified via DNS or `.well-known` endpoint._

Users prove control over a domain name by setting a DNS TXT record or hosting a DID document using the did:web method. Liccium validates this and issues a VC confirming domain control. This form of verification is well-suited for independent creators, studios, or organisations managing their own domains.

### **High – Third-Party Credential Issuer (with KYC)**

_A trusted third party confirms the user’s identity or role through KYC or affiliation check._

At this level, Verifiable Credentials are issued by **independent trust services** such as collecting societies (CMOs), professional associations, media organisations, or academic institutions. These issuers typically conduct **some form of KYC (Know Your Customer)** or internal identity validation before issuing credentials. The resulting VC binds the user to a real-world role or affiliation and provides strong assurance for verification workflows.

### **Highest – Qualified Trust Services**

_A legal entity signs declarations using a Qualified eSeal._

This level applies to declarations signed by legal entities using a **Qualified Certificate for Electronic Seal (QCert)**, issued by a **Qualified Trust Service Provider (QTSP)** in compliance with **eIDAS regulation**. These X.509 certificates are legally binding and confirm the identity of a registered company, public institution, or authorised representative. This trust level is appropriate for institutions publishing declarations with full legal certainty.

## Why Trust Levels Matter

Liccium’s infrastructure is designed to be open and permissionless – anyone can declare content. But that openness demands a way to **distinguish between claims made anonymously and those backed by real-world identities**.

By attaching credentials or certificates to declarations, creators and organisations can:

* Increase confidence in authorship and provenance
* Gain visibility in filtered or ranked views (e.g. “verified only”)
* Comply with transparency requirements for AI-generated or opt-out content
* Build a persistent reputation across declarations

Verifiers – whether humans or machines – can evaluate the **attached credential** and assign a **trust score or classification** based on this model.
