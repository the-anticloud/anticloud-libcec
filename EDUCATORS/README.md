# Educators — LIBCEC

**Project:** LIBCEC  
**Category:** CONSUMER_ELECTRONICS  
**Upstream:** see BENCH.json  
**Pinned commit:** `fe9df5ddf7356daa521f893c16872a09c8e6fb59`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `0cc2a5562c3dfe96e63842ad8c6cf4236ea9044e788229b3e8834d052820a899`  
**Date:** October 2026

## Teaching with LIBCEC

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `0cc2a5562c3dfe96e63842ad8c6cf4236ea9044e788229b3e8834d052820a899` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.
