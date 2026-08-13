# TelePort — Public Audit Anchors

This repository contains **only cryptographic audit receipts** for Totus Life
Services' TelePort platform (teleport.totuslife.org).

## What's here

- `audit-anchors/<date>.ots` — OpenTimestamps receipt files. Each one is the
  official proof that a SHA-256 fingerprint of TelePort's audit chain was
  published to the Bitcoin blockchain on that date.
- `audit-anchors/LEDGER.md` — the daily table of date → fingerprint →
  receipt, updated by an automated process every morning.

## What's NOT here

- ❌ No patient data, health records, or personal information — ever
- ❌ No source code (the TelePort app and this website are private)
- ❌ No database credentials, API keys, or secrets
- ❌ No names, emails, or anything identifiable

The fingerprints are SHA-256 hashes — one-way digests of the audit chain.
They prove *that* a record existed and was unaltered; they reveal nothing
about the content.

## How anyone can verify (no account, no server)

```bash
pip install opentimestamps   # official free tool
ots verify audit-anchors/2026-08-12.ots
```

The tool checks the receipt against the actual Bitcoin blockchain and
confirms the exact date the fingerprint was anchored. If a record in
TelePort's audit chain were ever altered, the hash would change and the
Bitcoin-anchored receipt would no longer match — making tampering
provable by anyone, forever.

## Contact

Questions or security concerns: privacy@totuslife.org · 1-844-HI-TOTUS
