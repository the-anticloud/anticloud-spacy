# Students — SPACY

**Project:** SPACY  
**Category:** PHILOSOPHY_SEMANTICS  
**Upstream:** https://github.com/explosion/spaCy  
**Pinned commit:** `c2dabfce56ad2991685ec85783cd59637a5d7b8f`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `e79c411d10586e449961367a04429849fb13873c3e775726efaa7c5bc40d7449`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `c2dabfce56ad2991685ec85783cd59637a5d7b8f`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `e79c411d10586e449961367a04429849fb13873c3e775726efaa7c5bc40d7449`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.
