# TelePortUs — Audit Chain Blockchain Anchors

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
| 2026-08-22 | `3c2a127a01f1dd30da015017873b729486916bbb09c492a0ebe8fd4e4ed5c885` | 2026-08-22T12:21:00.545Z | `2026-08-22.ots` | `ots verify audit-anchors/2026-08-22.ots` |
| 2026-08-23 | `ff0493eb22c518738155140595c6584c3a4650a380747ec5348c9f23f1f39ace` | 2026-08-23T08:39:33.937Z | `2026-08-23.ots` | `ots verify audit-anchors/2026-08-23.ots` |
| 2026-08-24 | `7ab7bda58fcdde03c84137f89872e083d260d98f1a1211cad7b7e1fa34935b8a` | 2026-08-24T15:32:27.066Z | `2026-08-24.ots` | `ots verify audit-anchors/2026-08-24.ots` |
| 2026-08-25 | `150036708b39aa3cbcb57b09835d8179175d78832e1513b9f665d383c7e56574` | 2026-08-24T19:07:15.964Z | `2026-08-25.ots` | `ots verify audit-anchors/2026-08-25.ots` |
| 2026-08-26 | `7fdf7da677335333b13e4c90bc292be172199ef3e98f9be06d7571f5d7cc2b46` | 2026-08-25T17:01:06.409Z | `2026-08-26.ots` | `ots verify audit-anchors/2026-08-26.ots` |
| 2026-08-27 | `7fdf7da677335333b13e4c90bc292be172199ef3e98f9be06d7571f5d7cc2b46` | 2026-08-25T17:01:06.409Z | `2026-08-27.ots` | `ots verify audit-anchors/2026-08-27.ots` |
| 2026-08-29 | `e3f6ce2602bca32c5e288903bb015c3a9c57356f3b203338bfa649bb1ba17fc4` | 2026-08-28T21:24:25.017Z | `2026-08-29.ots` | `ots verify audit-anchors/2026-08-29.ots` |
| 2026-08-30 | `8d6b5dd08af562089dae1f9e21580a3795eaa507a96f82504a2003e2c9b053b1` | 2026-08-29T19:15:32.913Z | `2026-08-30.ots` | `ots verify audit-anchors/2026-08-30.ots` |
| 2026-08-31 | `2c98ee2b4c61f604e6ffd918c53491b1d6a78668e1689bc3ea6e9e9cf92efd19` | 2026-08-31T13:30:17.016Z | `2026-08-31.ots` | `ots verify audit-anchors/2026-08-31.ots` |
| 2026-09-01 | `507a193b31ebe334ac942d09b96e65e055f617ae37f136a7fc06eda3bfd84df7` | 2026-09-01T09:10:35.773Z | `2026-09-01.ots` | `ots verify audit-anchors/2026-09-01.ots` |
| 2026-09-02 | `29fb0efe22789f80310b6c084b3adda7185a4f45df05973c6c853a38e1e9b951` | 2026-09-02T11:25:41.282Z | `2026-09-02.ots` | `ots verify audit-anchors/2026-09-02.ots` |
| 2026-09-03 | `29fb0efe22789f80310b6c084b3adda7185a4f45df05973c6c853a38e1e9b951` | 2026-09-02T11:25:41.282Z | `2026-09-03.ots` | `ots verify audit-anchors/2026-09-03.ots` |
| 2026-09-04 | `29fb0efe22789f80310b6c084b3adda7185a4f45df05973c6c853a38e1e9b951` | 2026-09-02T11:25:41.282Z | `2026-09-04.ots` | `ots verify audit-anchors/2026-09-04.ots` |
| 2026-09-05 | `f5a13a7b3ac902d360ac999d7243973b8f889285c5a57188d6026e9b7ad34c9f` | 2026-09-05T11:37:06.018Z | `2026-09-05.ots` | `ots verify audit-anchors/2026-09-05.ots` |
| 2026-09-07 | `dbaa14d6986b621e6aa617525f8086d2f591047bb816add2f5938b8f1fa74a53` | 2026-09-07T15:05:47.095Z | `2026-09-07.ots` | `ots verify audit-anchors/2026-09-07.ots` |
