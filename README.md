# The First-Passage Obstruction: An Exact Reduction of Divergent Collatz Dynamics

**Paper W — Closing the Series A–V**

Closes the research program of Papers A–V by stating precisely what has been proved and what remains open. The central contribution is an exact reduction: Conjecture DSC (Deterministic Synchronization Collapse) implies the Collatz conjecture.

> This repository does not claim a proof of the Collatz conjecture.

---

## Overview

The paper distils the series into four exact theorems and one open conjecture. The Collatz conjecture is reduced to a statement about the first-passage probability of a specific deterministic map from a fixed starting point to a fixed target — a question in combinatorics and 2-adic dynamics with no probabilistic assumptions.

The central results are:

- **Theorem 1.1 (HCL)**: r_{K₂} ≡ r_{K₁} (mod 2^{K₁}); conditional density = 2^{−(K₂−K₁)}
- **Theorem 1.2 (DSC-pre)**: All orbits in Sᵢ(N) end their Kᵢ-cascade at the same residue q_{cascade} ≡ 3^{L_{Kᵢ}} r_{Kᵢ} (mod 2^{K_{i+1}}), with q_{cascade} ≢ r_{K_{i+1}} (mod 2^{K_{i+1}})
- **Theorem 1.3 (FPO)**: |S_{i+1}(N)|/|Sᵢ(N)| equals the first-passage probability FPP_{q_{cascade} → r_{K_{i+1}}} — a purely deterministic quantity
- **Theorem 1.4 (Monotonicity)**: Height records are strictly increasing; each K ≥ 4 is achieved at most once per orbit
- **Theorem 3.1 (Main Reduction)**: Conjecture DSC ⟹ Collatz conjecture

---

## Main Results

### Proved (Rigorous)

| Result | Method | Status |
|--------|--------|--------|
| Theorem HCL: Hensel conditional density exact | Hensel nesting | ✓ proved |
| Theorem DSC-pre: deterministic cascade endpoint | Cascade algebra | ✓ proved |
| Theorem FPO: prefix density = first-passage probability | Exact reduction | ✓ proved |
| Theorem Monotonicity: height records strictly increasing | Cascade theory | ✓ proved |
| Theorem 3.1: DSC ⟹ Collatz | Logical reduction | ✓ proved |

### Open

| Problem | Status |
|---------|--------|
| Open Problem 4.1: prove FPP(q_{cascade} → r_{K_{i+1}}) ≤ 2^{−(K_{i+1}−Kᵢ)} for all Kᵢ ≥ 4 | Open |

---

## Structure

```
§1   The exact proven results (algebraic + conditional)
§2   The observed phenomenon
§3   The main reduction: DSC ⟹ Collatz     ✓
§4   The remaining gap                      open
§5   What has been achieved
§6   Summary table: Papers A–W
```

---

## Open Problems

- **Open Problem 4.1**: Prove that FPP(q_{cascade} → r_{K_{i+1}}) ≤ 2^{−(K_{i+1}−Kᵢ)} uniformly for all Kᵢ ≥ 4

---

## Repository Structure

```
collatz-first-passage/
├── README.md
├── paper/
│   └── paper_w_first_passage_obstruction.pdf
└── LICENSE
```

---

## Related Work

This paper is part of a series on Collatz dynamics:

- [collatz-act1](https://github.com/KAMANOI/collatz-act1) — Foundational paper: prime survival dynamics and Chen-type theorem (v11)
- [collatz-renewal-structure](https://github.com/KAMANOI/collatz-renewal-structure) — Paper A: exact operator structure and finite information memory
- [collatz-finite-mixing-geometry](https://github.com/KAMANOI/collatz-finite-mixing-geometry) — Paper B: finite-level mixing geometry
- [collatz-spectral-amplification](https://github.com/KAMANOI/collatz-spectral-amplification) — Paper C: spectral amplification
- [collatz-scale-coherence](https://github.com/KAMANOI/collatz-scale-coherence) — Paper D: scale-coherence rigidity
- [collatz-valuation-renewal](https://github.com/KAMANOI/collatz-valuation-renewal) — Valuation renewal, finite residue connectivity, and orbitwise gap
- [collatz-residual-core](https://github.com/KAMANOI/collatz-residual-core) — The residual core: structural decomposition
- [collatz-congruence-synchronization](https://github.com/KAMANOI/collatz-congruence-synchronization) — Paper H: nested congruence constraints on synchronization
- [collatz-record-renewal](https://github.com/KAMANOI/collatz-record-renewal) — Paper N: record renewal compatibility
- [collatz-hensel-escape](https://github.com/KAMANOI/collatz-hensel-escape) — Paper O: Hensel memory and 2-adic escape target
- [collatz-hensel-scarcity](https://github.com/KAMANOI/collatz-hensel-scarcity) — Paper T: Hensel conditional scarcity and telescoping contradiction
- [collatz-prefix-counting](https://github.com/KAMANOI/collatz-prefix-counting) — Paper V: direct prefix counting and synchronization collapse
- [collatz-first-passage](https://github.com/KAMANOI/collatz-first-passage) — Paper W: first-passage obstruction (closes series A–V)
- [collatz-series-summary](https://github.com/KAMANOI/collatz-series-summary) — Series summary: research program on Collatz synchronization dynamics
- [collatz-prime-survival](https://github.com/KAMANOI/collatz-prime-survival) — Paper X v20: prime survival in affine Collatz dynamics

---

## Author

Hiroki Kamanoi
hirokikamanoi@gmail.com
2026
