# Infinitely Many Mersenne Primes via Exponential-Prime Persistence
## Canonical Lane (defined term): the manifold-constrained local-to-global closure architecture (`MP1-MP8`)

Canonical Lane research workspace for a flagship problem in computational and analytic number theory:
proving that infinitely many primes of the form `2^p - 1` exist through an admissible exponential-prime closure architecture.

## Main Manuscript

- [paper/MERSENNE_PRIMES_PREPRINT.md](paper/MERSENNE_PRIMES_PREPRINT.md)
- [paper/CANONICAL_ROUTING_INDEX.md](paper/CANONICAL_ROUTING_INDEX.md)

## Structure

- `paper/`
  - `MERSENNE_PRIMES_PREPRINT.md`
  - `CANONICAL_ROUTING_INDEX.md`
  - `EXTRACTION_SPEC.md`

- `notes/`
  - `EG1_public.md`
  - `EG2_public.md`
  - `EG3_public.md`
  - `EG4_public.md`
  - `IDENTIFICATION_BRIDGE.md`

- `repro/`
  - `REPRO_PACK.md`
  - `THIRD_PARTY_RERUN_PROTOCOL.md`
  - `run_repro.sh`
  - `repro_manifest.json`
  - `certificate_baseline.json`

- `scripts/`
  - `mp_closure_guard.py`
  - `extract_constants.py`
  - `promote_constants.py`
  - `update_manifest.py`
  - `release_gate.py`
  - `README.md`

- `artifacts/`
  - `constants_extraction_inputs.json`
  - `constants_extracted.json`
  - `constants_registry.json`
  - `stitch_constants.json`
  - `promotion_report.json`

## Local Reproducibility Command

```bash
bash repro/run_repro.sh
```

This writes `repro/certificate_runtime.json`.

## How To Read This Professionally

1. Theorem chain first: read `paper/MERSENNE_PRIMES_PREPRINT.md`.
2. Constants provenance second: audit `paper/EXTRACTION_SPEC.md`, `artifacts/constants_extraction_inputs.json`, `artifacts/constants_extracted.json`, and `artifacts/promotion_report.json`.
3. Pipeline third: run `bash repro/run_repro.sh` to audit hashes, provenance, and gates; it is reproducibility infrastructure, not theorem generation.

Release modes:

- `normalized`: `status=normalized_placeholder` allowed when explicitly labeled.
- `fully_extracted`: requires `status=derived_numeric` for all required constants and stitch keys.

Current MP runner policy:

- `repro/run_repro.sh` extracts, promotes, runs `scripts/mp_closure_guard.py`, updates `repro/repro_manifest.json`, and enforces `fully_extracted` release-gate mode.

## Routing Rule (inclusion discipline)

Every claim-bearing item must be routed through all three layers:

1. main preprint section/appendix,
2. mirror note under `notes/`,
3. artifact key consumed by `scripts/mp_closure_guard.py`.

Routing map: [paper/CANONICAL_ROUTING_INDEX.md](paper/CANONICAL_ROUTING_INDEX.md)

## Citation

- Metadata: [CITATION.cff](CITATION.cff)
- Manuscript target: [paper/MERSENNE_PRIMES_PREPRINT.md](paper/MERSENNE_PRIMES_PREPRINT.md)

## Authorship

- Program author: **HautevilleHouse**
- Canonical attribution source: [`CITATION.cff`](CITATION.cff)
