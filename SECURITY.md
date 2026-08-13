# Security Policy

## Purpose of this repository

This repository intentionally contains **only cryptographic audit receipts**
(OpenTimestamps `.ots` files and a public `LEDGER.md` of SHA-256 hashes). It
must never contain source code, patient data, credentials, or any other
sensitive material — by design and enforced by the repository's `.gitignore`.

## Reporting a leak or vulnerability

If you believe a real patient record, credential, or any other sensitive
material has ever been published here — or you find a vulnerability in how
this repository is maintained:

1. **Do not open a public issue** about patient data or credentials.
2. Email **privacy@totuslife.org** immediately with:
   - The file/commit you believe is affected
   - Why you believe it is sensitive
   - (Optional) your contact details

We acknowledge reports within 2 business days and take action
(removal + revocation) as appropriate.

## What we commit to

- The `.gitignore` blocks everything except `audit-anchors/` and `README.md`
- The automated anchor process writes only hashes and `.ots` receipts
- No PHI, no source code, no secrets — verified on every push
