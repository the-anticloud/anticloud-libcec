# How to Update — LIBCEC

**Project:** `LIBCEC`
**Category:** CONSUMER_ELECTRONICS
**Domain:** consumer electronics
**Date:** 2026-10-07

---

## Update Procedure

### Checking for Updates
```bash
LIBCEC --version
LIBCEC check-update
```

### Applying Updates
```bash
pip install --upgrade LIBCEC
```

### Rolling Back
```bash
pip install LIBCEC==<previous-version>
```

### Update Policy
- **Security updates:** Applied immediately
- **Feature updates:** Monthly release cycle
- **Breaking changes:** 6-month deprecation notice

## Verification

All 16 checks PASS. Evidence: `ISOLATED_LAB_RESULTS/03_Result_Register.md`.
