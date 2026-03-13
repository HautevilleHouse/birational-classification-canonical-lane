# Birational Classification via Model-Class Persistence
## Canonical Lane (defined term): the manifold-constrained local-to-global super-architecture (`BCL1-BCL8`)

Canonical Lane super-repo for a flagship umbrella problem in birational classification and algebraic geometry:
proving persistence of admissible birational reductions, flips, fibrations, and endpoint models through a multi-lane birational-classification super-architecture.

## Main Manuscript

- [paper/BIRATIONAL_CLASSIFICATION_PREPRINT.md](paper/BIRATIONAL_CLASSIFICATION_PREPRINT.md)
- [paper/CANONICAL_ROUTING_INDEX.md](paper/CANONICAL_ROUTING_INDEX.md)


## Super-Repo Role

This repository is not a single primitive endpoint case. It coordinates an admissible routed lattice whose native families are:

1. flips, divisorial contractions, and Mori-fiber reductions,
2. canonical bundle formula and adjoint transport packages,
3. abundance, semiampleness, and Iitaka endpoint packages,
4. termination, scaling, and discrepancy-control packages,
5. local-global stitching of the declared birational-classification endpoint package.

The runtime surface certifies closure of the declared super-lane, not just one local example.

## Structure

- `paper/`
  - `BIRATIONAL_CLASSIFICATION_PREPRINT.md`
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
  - `bcl_closure_guard.py`
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

1. Super-lane theorem chain first: read `paper/BIRATIONAL_CLASSIFICATION_PREPRINT.md`.
2. Routed-family mapping second: audit `paper/CANONICAL_ROUTING_INDEX.md` and the note layer.
3. Constants provenance third: audit `paper/EXTRACTION_SPEC.md`, `artifacts/constants_extraction_inputs.json`, `artifacts/constants_extracted.json`, and `artifacts/promotion_report.json`.
4. Pipeline fourth: run `bash repro/run_repro.sh` to audit hashes, provenance, and gates; it is reproducibility infrastructure, not theorem generation.

Release modes:

- `normalized`: `status=normalized_placeholder` allowed when explicitly labeled.
- `fully_extracted`: requires `status=derived_numeric` for all required constants and stitch keys.

Current BCL runner policy:

- `repro/run_repro.sh` extracts, promotes, runs `scripts/bcl_closure_guard.py`, updates `repro/repro_manifest.json`, and enforces `fully_extracted` release-gate mode.

## Routing Rule (inclusion discipline)

Every claim-bearing item must be routed through all three layers:

1. main preprint section/appendix,
2. mirror note under `notes/`,
3. artifact key consumed by `scripts/bcl_closure_guard.py`.

Routing map: [paper/CANONICAL_ROUTING_INDEX.md](paper/CANONICAL_ROUTING_INDEX.md)

## Citation

- Metadata: [CITATION.cff](CITATION.cff)
- Manuscript target: [paper/BIRATIONAL_CLASSIFICATION_PREPRINT.md](paper/BIRATIONAL_CLASSIFICATION_PREPRINT.md)

## Authorship

- Program author: **HautevilleHouse**
- Canonical attribution source: [`CITATION.cff`](CITATION.cff)
