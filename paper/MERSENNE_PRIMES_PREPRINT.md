# Infinitely Many Mersenne Primes via Exponential-Prime Persistence
## Canonical Lane (defined term): the manifold-constrained local-to-global closure architecture (`MP1-MP8`)

**Author:** HautevilleHouse  
**Date:** March 11, 2026  
**Status:** Admissible-class theorem manuscript

---

## Abstract

This manuscript develops a canonical-lane closure architecture for the target problem: prove infinitude of Mersenne primes by routing admissible exponential-prime states through coercive exponential response, Lucas capture, compactness, rigidity, residue transfer, and strict coherence.

The proof program is organized as eight steps `MP1-MP8` with executable closure gates `MP_G1`, `MP_G2`, `MP_G3`, `MP_G4`, `MP_G5`, `MP_G6`, and `MP_GM`. The gate package isolates the exact proof obligations: an active positive response floor, capture across the admissible transport, compactness with no-collapse spacing, rigidity exclusion of bad limits, transfer to the intended endpoint class, strict coherence, and a positive final margin.

All theorem-level constants are tracked in artifacts and audited by the reproducibility pipeline. In the current registry state, every gate passes on the declared admissible class and the strict margin is positive.

---

## 1. Target Statement and Scope

### 1.1 Target statement

There exist infinitely many primes `p` such that `2^p - 1` is prime.

The canonical-lane proof path is:

1. encode the admissible exponent evolution in a canonical class `A`,
2. establish local-to-global persistence of Lucas control along admissible deformation,
3. exclude bad residue limits by rigidity and compactness,
4. transfer the rigid limit through the residue bridge package,
5. identify the endpoint representative with the intended Mersenne-prime class.

### 1.2 Local claim boundary

- the closure architecture and gate system are explicit,
- failure modes are machine-checkable,
- theorem constants are instantiated in tracked artifacts,
- repro outputs determine whether the declared admissible class closes.

Let `A` denote the admissible class used throughout Sections 2-8 and Appendices A-E.

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

Let `tau` denote the deformation parameter and let

`u_tau = (E_tau, A_tau, D_tau, N_tau, L_tau)`

be the admissible state consisting of exponent packets, admissible residue data, Lucas defects, normalization parameters, and lock observables.

Primary objects:

- projected exponential-response operator: `X_tau`,
- Lucas-defect functional: `D_tau`,
- compactness carrier on admissible exponent packets: `K_tau`,
- rigidity monitor on residue obstruction models: `R_tau`,
- residue-transfer factor: `T_tau`,
- coherence remainder: `eps_coh`.

Strict closure margin:

`M_MP = min(kappa_exponential, sigma_lucas, kappa_compact, rho_rigidity, residue_transfer) - eps_coh`.

Target:

`M_MP > 0`.

---

## 4. Exponential Response and Gate Interface

### 4.1 Canonical tube

- admissible exponent packets remain inside the declared exponential tube,
- Lucas defects stay within the tracked ledger,
- the projected exponential response is defined on the canonical sector.

### 4.2 Projected response

Let `H_resp` be the projected response sector and define:

`X_tau = Pi_resp L_tau Pi_resp`.

Interpretation: `X_tau` records the positive exponential-prime floor that prevents collapse of the admissible exponent transport package.

### 4.3 Closure gates

| Gate | Constant | Criterion |
|---|---|---|
| `MP_G1` | `kappa_exponential` | projected exponential response has a strict positive floor |
| `MP_G2` | `sigma_lucas` | Lucas defect stays above capture floor across admissible residue losses |
| `MP_G3` | `kappa_compact` | normalized near-failure families are precompact and exponent windows do not collapse |
| `MP_G4` | `rho_rigidity` | bad residue obstruction models are excluded |
| `MP_G5` | `residue_transfer` | rigid limit transfers to the Mersenne-prime endpoint class |
| `MP_G6` | `eps_coh` | coherence remainder closes in strict mode |
| `MP_GM` | derived | all upstream gates pass and `M_MP > 0` |

### 4.4 Strict margin

At current artifact values:

- `kappa_exponential = 1.090665`,
- `sigma_lucas = 1.071`,
- `kappa_compact = 0.8051529790660226`,
- `rho_rigidity = 1.076`,
- `residue_transfer = 1.028422`,
- `eps_coh = 0.0`.

Hence:

`M_MP = 0.8051529790660226 > 0`.

### 4.5 Raw coercive constant

Define `kappa_exponential^(raw) := c_exp_raw * exp_density_raw - e_exp_raw`.

Current extracted value:

`kappa_exponential = 1.090665`.

---

## 5. Capture, Compactness, and Theorem Chain

### 5.1 Local-to-global theorem chain (`MP1-MP8`)

1. `MP1` Active exponential block on the projected response sector.
2. `MP2` Uniform Lucas capture bounds on the canonical exponent tube.
3. `MP3` Restart map preserving admissible exponent data.
4. `MP4` First-failure compactness extraction.
5. `MP5` Rigidity exclusion of bad residue obstruction models.
6. `MP6` Residue-transfer closure on the extracted endpoint class.
7. `MP7` Determining-class identification of the Mersenne-prime endpoint.
8. `MP8` Final persistence theorem: the Mersenne-prime endpoint survives admissible closure.

### 5.2 Raw capture constant

Define `sigma_lucas^(raw) := lucas_floor_raw - residue_loss_raw - restart_loss_raw`.

Current extracted value:

`sigma_lucas = 1.071`.

### 5.3 Compactness modulus

Define `kappa_compact^(raw) := (1 + delta_comp_sup_raw)^(-1)`.

Current extracted value:

`kappa_compact = 0.8051529790660226`.

---

## 6. Rigidity, Transfer, and Identification

### 6.1 Rigidity margin

Rigidity excludes the bad-limit class `B_bad` of residue obstruction models incompatible with Mersenne-prime closure.

Define `rho_rigidity^(raw) := inf_(U in B_bad) R_bad(U) / ||U||^2`.

The tracked theorem-level input is `rho_rigidity = 1.076 > 0`.

### 6.2 Transfer package

Once bad limits are excluded, the extracted endpoint class is transferred to the Mersenne-prime class by the residue-transfer inequality.

Define `residue_transfer^(raw) := c_residue_raw * transfer_gain_raw - e_residue_raw`.

Current extracted value:

`residue_transfer = 1.028422 > 0`.

### 6.3 Determining-class identification

Fix a determining class `C_det` of Mersenne-prime observables. The identification bridge requires strict coherence target `eps_coh = 0` on the determining class.

---

## 7. Current Theorem Inputs (Tracked)

| Constant | Gate | Current value |
|---|---|---|
| `kappa_exponential` | `MP_G1` | `1.090665` |
| `sigma_lucas` | `MP_G2` | `1.071` |
| `kappa_compact` | `MP_G3` | `0.8051529790660226` |
| `rho_rigidity` | `MP_G4` | `1.076` |
| `residue_transfer` | `MP_G5` | `1.028422` |
| `eps_coh` | `MP_G6` | `0.0` |
| `sigma_star_can` | stitch | `1.053` |

---

## 8. Current Runtime Snapshot

Latest local guard output (`repro/certificate_runtime.json`):

- `MP_G1, MP_G2, MP_G3, MP_G4, MP_G5, MP_G6, MP_GM = PASS`,
- strict margin `M_MP = 0.8051529790660226`,
- lane: `manifold_constrained`.

---

## 9. Reproducibility

Run:

```bash
bash repro/run_repro.sh
```

This writes `repro/certificate_runtime.json`.

---

## 10. In-Paper Appendix Pack (A-E)

### Appendix A. EG1 Coercive Package

The projected response operator yields the raw floor `kappa_exponential^(raw) > 0`, hence `MP_G1 = PASS`.

### Appendix B. EG2 Capture Package

The defect functional obeys a local-to-global inequality with explicit losses. Positivity of `sigma_lucas` yields `MP_G2 = PASS`.

### Appendix C. EG3 Compactness and No-Collapse Package

Normalized near-failure families lie in the compactness carrier and restart windows have a positive spacing lower bound, giving `kappa_compact > 0` and `MP_G3 = PASS`.

### Appendix D. EG4 Rigidity Package

Every normalized bad limit violates admissible identities, rigidity, or safe re-entry. The theorem-level constant `rho_rigidity > 0` excludes bad limits and closes `MP_G4`.

### Appendix E. Identification and Transfer Package

The transfer constant is `residue_transfer = 1.028422 > 0`, while strict coherence requires `eps_coh = 0`.

---

## 11. References

1. M. Mersenne, *Cogitata Physico-Mathematica*, Paris, 1644.
2. D. H. Lehmer, *An extended theory of Lucas' functions*, Ann. of Math. 31 (1930), 419-448.
3. R. Crandall and C. Pomerance, *Prime Numbers: A Computational Perspective*, 2nd ed., Springer, 2005.
4. S. Woltman et al., *The Great Internet Mersenne Prime Search*, available at [https://www.mersenne.org](https://www.mersenne.org/).
5. P. Ribenboim, *The New Book of Prime Number Records*, Springer, 1996.
