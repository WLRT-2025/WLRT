# Price Non-Identifiability and Local Future Ambiguity  
### Minimal Structural Result v1.0

---

## Status
Canonical External Formal Result

## Context
This document defines a minimal formal result within the Wave Liquidity Redistribution Theory (WLRT) framework.

The result is independent of any specific implementation layer and does not disclose internal structural mechanisms of the theory.

## Scope
The purpose of this document is to establish structural limits of price-based inference in liquidity-driven systems.

The document contains:
- a formal non-identifiability theorem,
- a theorem on local admissible future ambiguity,
- corresponding corollaries and explicit construction.


## 1. Price Non-Identifiability

Let \(I \subset \mathbb{R}\) be a price interval, and let \(\mathcal{L}\) be a class of admissible liquidity distributions
\[
L : I \to \mathbb{R}_{\ge 0}.
\]

Let the observable price be defined by a scalar observation functional
\[
\Phi : \mathcal{L} \to \mathbb{R},
\qquad
P = \Phi[L],
\]
with
\[
\Phi[L] = \int_I w(p)\,L(p)\,dp,
\]
where \(w \not\equiv 0\).

### Definition 1. Liquidity State
A liquidity state is an admissible distribution \(L \in \mathcal{L}\).

### Definition 2. Price Observation
The price observation associated with a liquidity state \(L\) is the scalar value
\[
P = \Phi[L].
\]

### Theorem 1. Non-Identifiability of Liquidity State from Price Observation

Assume that \(\mathcal{L}\) contains at least two distinct admissible liquidity distributions and that the observation functional \(\Phi\) is scalar-valued as above.

Then the mapping
\[
\Phi : \mathcal{L} \to \mathbb{R}
\]
is not injective. In particular, there exist \(L_1, L_2 \in \mathcal{L}\), \(L_1 \neq L_2\), such that
\[
\Phi[L_1] = \Phi[L_2].
\]

### Proof

Since \(\Phi\) is a scalar-valued linear functional on a nontrivial class of admissible liquidity distributions, its kernel is nontrivial whenever the admissible class has effective dimension greater than one.

Let \(H \neq 0\) belong to the kernel of \(\Phi\), so that
\[
\Phi[H] = \int_I w(p)\,H(p)\,dp = 0.
\]

Choose any admissible liquidity state \(L \in \mathcal{L}\) such that \(L+H \in \mathcal{L}\). Define
\[
L_1 = L,
\qquad
L_2 = L + H.
\]

Then \(L_1 \neq L_2\), since \(H \neq 0\), while
\[
\Phi[L_2] = \Phi[L+H] = \Phi[L] + \Phi[H] = \Phi[L] = \Phi[L_1].
\]

Hence \(\Phi\) is not injective.

### Corollary 1. Price Equality Does Not Imply State Equality

There exist distinct liquidity states that generate the same observable price.
