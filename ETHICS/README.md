# Ethics — LIBCEC

**Project:** LIBCEC  
**Category:** CONSUMER_ELECTRONICS  
**Upstream:** see BENCH.json  
**Pinned commit:** `fe9df5ddf7356daa521f893c16872a09c8e6fb59`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `0cc2a5562c3dfe96e63842ad8c6cf4236ea9044e788229b3e8834d052820a899`  
**Date:** October 2026

## Position

LIBCEC is packaged for offline deployment with a verifiable audit trail. The
ethical questions this raises are answered by making the system's behaviour
checkable rather than by policy statements.

## The four commitments

1. **No hidden egress.** The deployment has no external API dependency; this is
   testable by running it with the network disconnected.
2. **Attributable output.** Every artifact is recorded in a hash chain, so what
   the system produced can be reconstructed.
3. **Operator control.** The institution owns the hardware and the keys.
4. **Refusal to overclaim.** Where a certification is not held, the project says
   so rather than implying it.

## Dual use

This project is packaged for civilian and public-sector deployment. Where an
upstream has dual-use characteristics, the licence gate and the reference-only
marking in `BENCH.json` record that.
