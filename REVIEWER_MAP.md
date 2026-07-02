# Reviewer Map

## Claim Scope

- Canonical-lane claim: inside the `manifold_constrained` lane, if the theorem chain in this repository holds and the guard certificate passes, the repository-level closure claim is satisfied.
- Standard target claim: carried by the in-repo bridge theorems tying the lane to the target statement.

## Theorem Dependency Chain

1. `EG1`: coercive response and active control floor.
2. `EG2`: capture and admissible continuation.
3. `EG3`: compactness and no-collapse spacing.
4. `EG4`: rigidity and transfer.
5. Identification bridge: strict coherence on the determining class.
6. Scalar closure: `MP_G1, MP_G2, MP_G3, MP_G4, MP_G5, MP_G6, MP_GM` all `PASS`.

Primary files:

- `paper/MERSENNE_PRIMES_PREPRINT.md`
- `notes/EG1_public.md`
- `notes/EG2_public.md`
- `notes/EG3_public.md`
- `notes/EG4_public.md`
- `notes/IDENTIFICATION_BRIDGE.md`

## Closure Gates

| Gate | Constant | Description |
|------|----------|-------------|
| `MP_G1` | `kappa_exponential` | projected exponential response has a strict positive floor |
| `MP_G2` | `sigma_lucas` | Lucas defect stays above capture floor across admissible residue losses |
| `MP_G3` | `kappa_compact` | normalized near-failure families are precompact and exponent windows do not collapse |
| `MP_G4` | `rho_rigidity` | bad residue obstruction models are excluded |
| `MP_G5` | `residue_transfer` | rigid limit transfers to the Mersenne-prime endpoint class |
| `MP_G6` | `eps_coh` | strict coherence / identification closure |
| `MP_GM` | derived | final strict margin |

## Falsification Conditions

- `repro/certificate_runtime.json` has any non-`PASS` gate.
- `lane.active_lane != "manifold_constrained"`.
- `all_pass != true`.
- Any manifest hash mismatch under `repro/repro_manifest.json`.
- A certified counterexample to any EG theorem statement used in the paper.
