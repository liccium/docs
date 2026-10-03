# Managing declarations

Rights, metadata and preferences change over time. Liccium B2B Services let your organisation update its declarations while keeping a verifiable history of what was declared and when.

## Updating and superseding

To update a declaration – for example after a change of licensing terms or AI preferences – your organisation submits a new declaration for the same asset. The new declaration supersedes the earlier one. The earlier declaration remains part of the provenance chain, so anyone resolving the asset can see both the current declaration and its history.

## Redaction

Redaction withdraws a declaration from discovery. A redacted declaration no longer appears in ISCC similarity search, but it still exists: its identifier still resolves, marked as redacted, it remains in the provenance chain, and later declarations can still supersede it. Redaction can be reversed. Only the declarer can redact its own declarations.

## Deletion

Deletion removes a declaration's metadata from Liccium-controlled systems. A deleted declaration is replaced by a public deletion marker, so that verifying parties can recognise that a declaration existed and has been deleted.

## What remains after redaction or deletion

Public declarations may already have been indexed, copied, cached or stored by third parties, and may be held on distributed infrastructure. Such copies are outside the control of Liccium and your organisation. Prior versions, timestamps and technical integrity records may also be retained as part of the declaration history.

The Redaction and Deletion API is documented on the [Liccium API and Developer Platform](https://dev.liccium.com).
