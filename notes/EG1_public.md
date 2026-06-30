# EG1 Public Note (Projected Response Floor)

Mature wording: `projection / protected core`.

In-paper anchor: `paper/BIRATIONAL_CLASSIFICATION_PREPRINT.md` (`BCL_G1`).

## Goal
Make the projected response floor explicit as the protected-core gate for `proving persistence of admissible birational reductions, flips, fibrations, and endpoint models through a multi-lane birational-classification super-architecture`.

## Objects

- admissible class: the declared class `A` in the main preprint.
- canonical/base object package: let `u_tau = (B_tau, M_tau, D_tau, N_tau, L_tau)` denote the admissible state of birational packets, model data, defect ledgers, normalization parameters, and lock observables.
- projected core: the response sector controlled by `kappa_birational`.
- carried remainder interface: downstream defect and coherence terms remain outside the protected core rather than being hidden in it.

## Closure Criterion

`BCL_G1` closes when `kappa_birational` satisfies the response-floor requirement: projected response has a strict positive floor.
This is the first protected-core contribution to the strict margin `M_BCL`.

## Lemma Chain and Proof Payload

### Lemma EG1.1 (projection reduction)
On the declared admissible class, the response object may be read on the projected sector without changing the target gate.

Payload: verify that all quantities used by `kappa_birational` are defined on the projected sector named in the main preprint.

### Lemma EG1.2 (protected-core floor)
If the projected response floor is positive on the admissible sector, then the core cannot collapse before the later transport and remainder gates are evaluated.

Payload: check the artifact key `kappa_birational` and the corresponding extraction input/provenance record.

### Theorem EG1.3 (core gate closure)
If Lemmas EG1.1-EG1.2 hold and the runtime artifact accepts `kappa_birational`, then `BCL_G1` supplies the projected/protected-core input to `M_BCL`.

## Current Instantiation

- gate: `BCL_G1`
- artifact key: `kappa_birational`
- mature equivalent: `projection / protected core`
- audit surface: `artifacts/constants_registry.json`, `artifacts/constants_extracted.json`, and `repro/certificate_runtime.json`
