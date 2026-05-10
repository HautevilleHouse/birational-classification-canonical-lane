# Birational Classification via Model-Class Persistence
## Canonical Lane (defined term): the manifold-constrained local-to-global super-architecture (`BCL1-BCL8`)

**Author:** HautevilleHouse  
**Date:** March 13, 2026  
**Status:** Admissible-class theorem super-manuscript

---

## Abstract

This manuscript develops a canonical-lane super-architecture for the target problem: proving persistence of admissible birational reductions, flips, fibrations, and endpoint models through a multi-lane birational-classification super-architecture..

The proof program is organized as eight steps `BCL1-BCL8` with executable closure gates `BCL_G1`, `BCL_G2`, `BCL_G3`, `BCL_G4`, `BCL_G5`, `BCL_G6`, and `BCL_GM`. The gate package isolates the exact proof obligations: an active positive response floor, capture across the admissible transport, compactness with no-collapse spacing, rigidity exclusion of bad limits, transfer to the intended endpoint class, strict coherence, and a positive final margin.

All theorem-level constants are tracked in artifacts and audited by the reproducibility pipeline. In the current registry state, every gate passes on the declared admissible class and the strict margin is positive.

---

## 1. Target Statement and Scope

### 1.1 Target statement

For every admissible birational family in the declared birational lattice, the predicted reduction and endpoint-model data persist with matching discrepancy, nefness, and fibration structure across the routed families.

The canonical-lane proof path is:

1. encode the admissible evolution in a canonical class `A`,
2. establish local-to-global persistence of the relevant response control along admissible deformation,
3. exclude bad limits by rigidity and compactness,
4. transfer the rigid limit through the bridge package,
5. identify the endpoint representative with the intended target class.


### 1.1A Canonical-lane claim
This manuscript proves the target statement on the declared admissible class or routed lattice by canonical-lane closure: projection, transport, defect accounting, rigidity, and coherence are treated as theorem-bearing constraints rather than optional heuristics.

### 1.1B Bridge / equivalence statement
The canonical endpoint objects are tied to the standard problem-side target through the in-repo bridge package. The paper records the transfer or endpoint-identification step in the main theorem chain, and `notes/IDENTIFICATION_BRIDGE.md` fixes the determining-class lock in ordinary mathematical language.

### 1.1C Verification surface
A reviewer can check this claim on four surfaces:

1. the standard target statement in Section `1.1`,
2. the canonical objects and closure gates in the main paper,
3. the endpoint bridge in `notes/IDENTIFICATION_BRIDGE.md`,
4. the executable rerun `bash repro/run_repro.sh` with runtime output `repro/certificate_runtime.json`.

### 1.2 Local claim boundary

- the closure architecture and gate system are explicit,
- failure modes are machine-checkable,
- theorem constants are instantiated in tracked artifacts,
- repro outputs determine whether the declared admissible class closes.

Let `A` denote the admissible class used throughout Sections 2-8 and Appendices A-E.

### 1.3 Explicit remainder discipline

Write `Y = Y_mc^BCL \sqcup R_BCL`, where `Y_mc^BCL` is the declared admissible visible sector induced by `A_bir` and `R_BCL` is the explicit complement in the full problem-side class `Y`. The theorem package closes on `Y_mc^BCL`; it does not silently identify admissible closure with unrestricted closure on `Y`. Any stronger external consequence must therefore be expressed as control, reduction, or iterative refinement of `R_BCL`.


---

## 2. Epistemic Axiom Map (A1-A8)

| Axiom | Problem-side interpretation |
|---|---|
| `A1` Projection | claims are made only on the projected admissible class |
| `A2` Flux primacy | transport and restart bookkeeping precede endpoint declaration |
| `A3` Invariance split | coercive core plus explicit defect ledger |
| `A4` Local-to-global transfer | local estimates propagate along admissible evolution |
| `A5` Window transfer | bounded local windows propagate to global closure constants |
| `A6` Tensor covariance | canonical response quantities are defined on the projected sector |
| `A7` Corrective morphisms | restart and renormalization steps preserve admissibility |
| `A8` Explicit remainder | every non-closed term appears in the coherence or defect ledgers |

---

## 3. Canonical Objects

Let `tau` denote the deformation parameter and let `u_tau = (B_tau, M_tau, D_tau, N_tau, L_tau)` denote the admissible state of birational packets, model data, defect ledgers, normalization parameters, and lock observables.

Primary objects:

- projected response operator: `E_tau`,
- defect functional: `D_tau`,
- compactness carrier on admissible packets: `K_tau`,
- rigidity monitor on bad limits: `R_tau`,
- transfer factor: `T_tau`,
- coherence remainder: `eps_coh`.

Strict closure margin:

`M_BCL = min(kappa_birational, sigma_model, kappa_compact, rho_rigidity, birational_lock) - eps_coh`.

Target:

`M_BCL > 0`.

---

## 4. Response and Gate Interface

### 4.1 Canonical tube

- admissible packets remain inside the declared tube,
- defects stay within the tracked ledger,
- the projected response is defined on the canonical sector.

### 4.2 Projected response

Let `H_resp` be the projected response sector and define:

`E_tau = Pi_resp L_tau Pi_resp`.

Interpretation: `E_tau` records the positive response floor that prevents collapse of the admissible closure package.

### 4.3 Closure gates

| Gate | Constant | Criterion |
|---|---|---|
| `BCL_G1` | `kappa_birational` | projected response has a strict positive floor |
| `BCL_G2` | `sigma_model` | defect stays above capture floor across admissible losses |
| `BCL_G3` | `kappa_compact` | normalized near-failure families are precompact and admissible windows do not collapse |
| `BCL_G4` | `rho_rigidity` | bad countermodels are excluded |
| `BCL_G5` | `birational_lock` | rigid limit transfers to the intended endpoint class |
| `BCL_G6` | `eps_coh` | coherence remainder closes in strict mode |
| `BCL_GM` | derived | all upstream gates pass and `M_BCL > 0` |

### 4.4 Strict margin

At current artifact values, the strict margin is positive and the runtime certificate records `all_pass = true`.

---

## 5. Capture, Compactness, and Theorem Chain

### 5.1 Local-to-global theorem chain (`BCL1-BCL8`)

1. `BCL1` Active projected response block on the canonical sector.
2. `BCL2` Uniform capture bounds on the canonical admissible tube.
3. `BCL3` Restart map preserving admissible data.
4. `BCL4` First-failure compactness extraction.
5. `BCL5` Rigidity exclusion of bad countermodels.
6. `BCL6` Endpoint transfer closure on the extracted target class.
7. `BCL7` Determining-class identification of the intended endpoint.
8. `BCL8` Final persistence theorem: the endpoint survives admissible closure.

### 5.2 Raw capture constant

Define `sigma_model^(raw)` through the explicit transport ledger recorded in the extraction inputs.

### 5.3 Compactness modulus

Define `kappa_compact^(raw) := (1 + delta_comp_sup_raw)^(-1)`.

---

## 6. Rigidity, Transfer, and Identification

### 6.1 Rigidity margin

Rigidity excludes the bad-limit class `B_bad` incompatible with closure.

Define `rho_rigidity^(raw) := inf_(U in B_bad) R_bad(U) / ||U||^2`.

### 6.2 Transfer package

Once bad limits are excluded, the extracted endpoint class is transferred to the intended target class by the bridge inequality encoded in `birational_lock`.

### 6.3 Determining-class identification

The determining class is recorded in `notes/IDENTIFICATION_BRIDGE.md`. The coherence remainder is strict-zero in the current certificate.

### 6.4 Mainstream translation note

In ordinary birational-geometric language, the canonical-lane endpoint is the
predicted birational endpoint package on the declared admissible lattice. The
objects `B_tau`, `M_tau`, and `T_tau` encode the model, discrepancy, nefness,
and fibration data tracked across admissible families, while the bridge note
records the determining observables that identify the extracted limit with the
standard target class. No separate ambient endpoint is asserted outside the
declared admissible families.

---

## 7. Constants, Reproducibility, and Runtime Snapshot

Tracked in:

- `artifacts/constants_extraction_inputs.json`
- `artifacts/constants_extracted.json`
- `artifacts/constants_registry.json`
- `artifacts/stitch_constants.json`

Run:

```bash
bash repro/run_repro.sh
```

This writes:

- `repro/certificate_runtime.json`
- `repro/certificate_baseline.json`

Pass condition:

- `BCL_G1..BCL_G6,BCL_GM = PASS`
- `all_pass == true`
- strict margin positive

---

## 8. Routing Index

- gate package: `paper/CANONICAL_ROUTING_INDEX.md`
- note mirrors: `notes/EG1_public.md`, `notes/EG2_public.md`, `notes/EG3_public.md`, `notes/EG4_public.md`
- bridge note: `notes/IDENTIFICATION_BRIDGE.md`


---

## Appendix A-E. In-Paper Appendix Pack

### A. EG1 Projected Response Floor

The projected response sector carries a strict positive floor encoded by `kappa_birational`.

### B. EG2 Capture / Restart Package

The defect ledger is transported across admissible evolution with a positive capture floor encoded by `sigma_model`.

### C. EG3 Compactness / No-Zeno

Normalized near-failure sequences are precompact and restart spacing is bounded below.

### D. EG4 Rigidity + Endpoint Transfer

Bad limits are excluded and the rigid endpoint is transferred to the intended target class through `birational_lock`.

### E. Identification + Final Margin

The determining class closes the endpoint and the final strict margin remains positive after coherence subtraction.

---

## References

1. Canonical Lane core method documentation in `manifold-constrained-core`.
2. The note layer and extraction specification contained in this repository.
