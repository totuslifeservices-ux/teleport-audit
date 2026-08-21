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
| 2026-08-13 | `86ad64acc40addb9882064e7fe9ed9488af09f01e72eb6a4c449cb476a9c76c2` | 2026-08-12T18:16:13.766Z | `2026-08-13.ots` | `ots verify audit-anchors/2026-08-13.ots` |
| 2026-08-13 | `590ed8b05af92ad2cfc7f2a1c56e554eae339e42cf3068adf5b8168512f83b99` | 2026-08-13T16:40:51.211Z | `2026-08-13.ots` | `ots verify audit-anchors/2026-08-13.ots` |
| 2026-08-14 | `590ed8b05af92ad2cfc7f2a1c56e554eae339e42cf3068adf5b8168512f83b99` | 2026-08-13T16:40:51.211Z | `2026-08-14.ots` | `ots verify audit-anchors/2026-08-14.ots` |
| 2026-08-15 | `caf5851ae29e725c6a59b7f5e5f3460f7bc7ef80d5f2b5fdb5da70cef182c30b` | 2026-08-15T15:50:13.065Z | `2026-08-15.ots` | `ots verify audit-anchors/2026-08-15.ots` |
| 2026-08-16 | `0f50a8e469fbb4924dce1085ef2ae805040138a45f91d207ed97d8a6f6a85393` | 2026-08-15T19:34:45.090Z | `2026-08-16.ots` | `ots verify audit-anchors/2026-08-16.ots` |
| 2026-08-19 | `cfb4ea8052230eaf1b84dc3005c81315d362f422d59cbd3fb720448643a0b023` | 2026-08-19T16:08:20.522Z | `2026-08-19.ots` | `ots verify audit-anchors/2026-08-19.ots` |
| 2026-08-19 | `cfb4ea8052230eaf1b84dc3005c81315d362f422d59cbd3fb720448643a0b023` | 2026-08-19T16:08:20.522Z | `2026-08-19.ots` | `ots verify audit-anchors/2026-08-19.ots` |
| 2026-08-20 | `a8eefc12e326e6445b64c07d0c06106c50c4142c78662882a3c4a45f845d30b0` | 2026-08-20T14:13:47.237Z | `2026-08-20.ots` | `ots verify audit-anchors/2026-08-20.ots` |
| 2026-08-21 | `9ab414507eb6031002f76e0c2d0643af95df85e01f221ddacab30fc25fc6a81d` | 2026-08-21T09:48:39.603Z | `2026-08-21.ots` | `ots verify audit-anchors/2026-08-21.ots` |
