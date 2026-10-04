# Declaration API

The Declaration API receives declarations submitted by your organisation, validates them and publishes valid declarations to the Liccium Registries. All functions are available through the API, so declarations can be generated and submitted automatically from your existing workflows.

## What a declaration request contains

* the ISCC of the asset;
* the declaration metadata;
* your organisation's identifier as declarer, as a decentralised identifier (DID);
* the digital signature over the metadata, made with your organisation's key;
* the certificate chain or Verifiable Credential that authenticates the signature;
* a trusted timestamp (RFC 3161).

Requests are authenticated with an API key issued through the Liccium API and Developer Platform.

## What the API does

1. Validates the declaration data against the Liccium schema.
2. Verifies the digital signature and the attached certificates or credentials.
3. Verifies the timestamp.
4. Publishes the valid declaration to the Liccium Registries and returns its declaration identifier (CID).

Declarations carrying AI preferences can also be published to the TDM·AI registry (Optout.directory), and declarations carrying FAIA information to the FAIA registry. Declarations may also be synchronised to other compatible registries and distributed infrastructure supported by the Liccium Services.

## Publication and hosting

Published declarations are hosted, indexed and made available for resolution by Liccium as part of the hosted declaration service. The metadata of a public declaration may be persistently stored on peer-to-peer or comparable distributed infrastructure, and may be synchronised, copied or stored by third parties.

## Authorisation

Each declaration is authorised by your organisation. Authorisation can happen automatically through your systems, approval workflows or signing processes, as agreed during onboarding.

## Liccium API and Developer Platform

The full API reference, including request and response examples, is available on the [Liccium API and Developer Platform](https://dev.liccium.com).
