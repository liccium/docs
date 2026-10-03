# Certificates and credentials

Liccium accepts only certified declarations. Every declaration is signed by your organisation and carries evidence of who the declarer is, so that anyone resolving the declaration can establish who made the claim and which trust service vouches for it.

## Authentication methods

To sign declarations, your organisation needs one of the following:

| Method                      | Description                                                                                                                                                |
| --------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Electronic seal certificate | An advanced or qualified certificate for electronic seals (eSeal), issued to your organisation under the eIDAS Regulation by a trust service provider      |
| Verifiable Credential       | A credential issued through [Creator Credentials](https://creatorcredentials.app), or by another issuer accepted under the current technical documentation |

The Declaration API supports both methods. Organisations using a certificate can link their keys to their web domain through a `did:web` identifier. Setup instructions for X.509 certificates and `.well-known/did.json` are available on the [Liccium API and Developer Platform](https://dev.liccium.com).

## Your keys, under your control

Your organisation generates and exclusively controls the keys used to sign declarations. Keys can be held in your own hardware security module (HSM), in a cloud key management service (KMS), or by a trust service provider.

Liccium does not generate, store or have access to your private keys, unless your organisation requests this and it is agreed separately in writing.

## Verification by Liccium

When a declaration is submitted, Liccium verifies the signature, the certificate chain or credential and the timestamp. Submissions that cannot be verified, or that put the integrity or security of the registries at risk, are not published.

## Security

Your organisation is responsible for safeguarding its keys, certificates and credentials. If a key or credential is compromised, lost, revoked or expires, notify Liccium without delay.
