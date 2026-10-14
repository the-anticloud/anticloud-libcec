# Onboarding — LIBCEC

**Project:** LIBCEC  
**Category:** CONSUMER_ELECTRONICS  
**Upstream:** see BENCH.json  
**Pinned commit:** `fe9df5ddf7356daa521f893c16872a09c8e6fb59`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `0cc2a5562c3dfe96e63842ad8c6cf4236ea9044e788229b3e8834d052820a899`  
**Date:** October 2026

## First hour

1. Read `README.md` — what the project is and what it measures.
2. Read `ISOLATED_LAB_RESULTS/03_Result_Register.md` — the 16 checks and their
   evidence hashes.
3. Run the suite: `python tools/run_bench.py --out BENCH.json`.
4. Verify a hash: recompute SHA3-256 of a file in `04_Evidence/` and compare.

## First day

- `10_TECHNICAL_HANDOFF` — architecture and interfaces
- `11_TUTORIAL_DEVELOPERS` — build and test
- `18_COMMAND_LINE_INTERFACE` — CLI reference
- `27_DEPENDENCIES` — the offline dependency mirror

## Getting help

lois@0-1.gg · 0-1.gg
