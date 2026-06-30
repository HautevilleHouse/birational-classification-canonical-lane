# EG2 Public Note (Capture and Restart)

Mature wording: `transport / local-to-global transfer`.

In-paper anchor: `paper/BIRATIONAL_CLASSIFICATION_PREPRINT.md` (`BCL_G2`).

## Goal
Expand the compressed capture/restart language into the local-to-global transport gate for `proving persistence of admissible birational reductions, flips, fibrations, and endpoint models through a multi-lane birational-classification super-architecture`.

## Objects

- transport carrier: the admissible evolution or routed lattice declared in the preprint.
- capture floor: `sigma_model`.
- restart law: the normalization/re-entry rule that keeps corrective steps inside the admissible class.
- carried losses: defect, restart, and normalization losses that must remain explicit.

## Closure Criterion

`BCL_G2` closes when `sigma_model` survives admissible losses and restart corrections: defect stays above capture floor across admissible losses.
This is the transport contribution to `M_BCL`.

## Lemma Chain and Proof Payload

### Lemma EG2.1 (transport accounting)
Every transport step used by the lane is charged to the declared defect ledger instead of being absorbed into prose.

Payload: verify that the capture constant `sigma_model` is present in the constants registry and extraction inputs.

### Lemma EG2.2 (restart preservation)
Restart or normalization preserves the declared admissible class and does not create an untracked remainder.

Payload: inspect the repro script and guard output for the gate tied to `sigma_model`.

### Theorem EG2.3 (capture gate closure)
If transport accounting and restart preservation hold, then `BCL_G2` carries the local control forward without breaking admissibility.

## Current Instantiation

- gate: `BCL_G2`
- artifact key: `sigma_model`
- mature equivalent: `transport / local-to-global transfer`
- audit surface: `repro/run_repro.sh` and `repro/certificate_runtime.json`
