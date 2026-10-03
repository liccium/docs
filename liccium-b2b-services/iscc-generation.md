# ISCC generation

The International Standard Content Code (ISCC, ISO 24138:2024) is a content fingerprint derived from the asset itself – from its text, image, audio or video content – using cryptographic and similarity-preserving hashes. Anyone with access to an identical or sufficiently similar copy of the asset can generate the same or a similar ISCC, without access to your systems.

## Generation in your environment

The ISCC generator runs within your organisation's own environment – on your own servers, in a private cloud or in a cloud account you control, for example on Amazon Web Services. Your assets do not leave your infrastructure to be fingerprinted.

The generator is based on open-source software published under the Apache 2.0 licence:

| Component                     | Repository                                     |
| ----------------------------- | ---------------------------------------------- |
| ISCC codec and algorithms     | [iscc-core](https://github.com/iscc/iscc-core) |
| ISCC library                  | [iscc-lib](https://github.com/iscc/iscc-lib)   |
| ISCC software development kit | [iscc-sdk](https://github.com/iscc/iscc-sdk)   |

If you prefer, Liccium can generate ISCC codes on your behalf. The technical arrangements and data processing requirements are agreed individually.

## What an ISCC does and does not state

An ISCC identifies an asset. Generating it does not, by itself, make any statement about authorship, ownership, licensing or any other legal status of the asset, and it has no effect on the rights in the asset.

Such statements are made in a declaration – a separate, digitally signed record that connects the ISCC to your rights information and metadata. See Declaration metadata.
