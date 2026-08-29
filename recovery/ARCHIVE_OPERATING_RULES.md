# The Origin of Matter — Archive Operating Rules

These rules are mandatory for future publication development.

## Artifact states

Every output must be labeled as exactly one of:

1. **Generated** — produced in a temporary runtime or conversation.
2. **Verified** — rendered/preflighted and scientifically/layout checked.
3. **Persistently archived** — exact raw bytes independently re-found/read back from persistent storage.

A file may be generated and verified without being persistently archived.

## Temporary-link rule

ChatGPT `sandbox:` links and runtime `/mnt/data` paths are temporary delivery mechanisms. They must never be treated as the only copy of a milestone.

## Required milestone metadata

Every substantial milestone should preserve, at minimum:

- version number;
- exact filename;
- title/scope;
- page count;
- exact byte size;
- SHA-256;
- source/provenance notes;
- render/preflight status;
- hierarchy depth;
- evidence-firewall notes;
- primary-source anchors;
- reconstruction notes;
- persistent storage location(s).

## Binary archive rule

When a connector cannot upload arbitrary binary bytes directly, do **not** claim that a PDF has been uploaded. Preserve all recoverable text, hashes, manifests, Library/Drive identifiers, and reconstruction specifications in GitHub, then use a binary-capable route for the actual PDF. After upload, independently verify the remote binary or its hash before marking it archived.

## Reconstruction hierarchy

Preferred reconstruction anchor order:

1. highest exact persistent continuous master;
2. exact persistent part/chapter PDFs;
3. exact milestone binaries;
4. GitHub milestone README/specification text;
5. recovery ledgers and hashes;
6. conversation/project scientific text and source citations;
7. regenerated layout/illustrations after content is restored.

## Current verified continuous-master anchor

As of the 2026-08-29 recovery audit, the highest exact continuous master located in the persistent Library is v132:

`The_Origin_of_Matter_Continuous_Encyclopedic_Master_Assembly_v132_Global_Glyph_Table_Wrap_Repair.pdf`

SHA-256: `219b261f352be0d7d969c677b3d8097239197f54632e0268854478ce60c67f3a`

357 pages; 8,454,899 bytes.
