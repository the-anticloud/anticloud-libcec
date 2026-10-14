# Students — LIBCEC

**Project:** LIBCEC  
**Category:** CONSUMER_ELECTRONICS  
**Upstream:** see BENCH.json  
**Pinned commit:** `fe9df5ddf7356daa521f893c16872a09c8e6fb59`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `0cc2a5562c3dfe96e63842ad8c6cf4236ea9044e788229b3e8834d052820a899`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `fe9df5ddf7356daa521f893c16872a09c8e6fb59`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `0cc2a5562c3dfe96e63842ad8c6cf4236ea9044e788229b3e8834d052820a899`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.
