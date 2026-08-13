# TelePort — Audit Chain Blockchain Anchors

Every day, the current **audit-chain head hash** is anchored to the Bitcoin
blockchain via [OpenTimestamps](https://opentimestamps.org) (free community
calendar — batches thousands of hashes into one donation-funded transaction).

**Why:** the audit log is a hash chain — altering *any* past event breaks every
hash after it. Anchoring the daily head hash to Bitcoin proves the chain was
not tampered with, verifiable by anyone, forever, with zero server access.

**Verify any receipt (no account, no server):**
```bash
pip install opentimestamps   # or: brew/apt — official tool
ots verify audit-anchors/<date>.ots
```

| Date | Head hash | Head time (UTC) | Receipt | Verify |
|------|-----------|-----------------|---------|--------|
| 2026-08-10 | `e9509accea585212940c81e13f1802cd3a28fe6c45a23134eb2a9239e4ba7984` | 2026-08-10T19:04:47.169Z | `2026-08-10.ots` | `ots verify audit-anchors/2026-08-10.ots` |
| 2026-08-11 | `8f3d9aa630cc4960f3229dd6f2e909491f52e409ce19a940b9f540492f089fcf` | 2026-08-11T00:21:56.501Z | `2026-08-11.ots` | `ots verify audit-anchors/2026-08-11.ots` |
| 2026-08-12 | `785d1fddcb5fc0d46c35041b3d899f906809f4886ec145a9214d126eccfb83b9` | 2026-08-11T19:08:09.657Z | `2026-08-12.ots` | `ots verify audit-anchors/2026-08-12.ots` |
