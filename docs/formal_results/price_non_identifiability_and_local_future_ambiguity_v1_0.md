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

---

## 2. Non-Uniqueness of Local Admissible Futures

### Definition 3. Structural Transition
A structural transition is a change of liquidity state
\[
L_1 \to L_2
\]
with \(L_1 \neq L_2\).

### Definition 4. Admissible Local Transition
A local admissible transition from a liquidity state \(L\) is a perturbation
\[
L \to L + \delta L,
\]
such that \(L + \delta L \in \mathcal{L}\).

### Definition 5. Local Admissible Future Set
The local admissible future set at state \(L\) is defined as
\[
\mathcal{F}(L) = \{L + \delta L \;|\; \delta L \text{ admissible}\}.
\]

### Theorem 2. Non-Uniqueness of Local Admissible Futures

There exist liquidity states \(L_1 \neq L_2\) such that
\[
\Phi[L_1] = \Phi[L_2],
\]
but
\[
\mathcal{F}(L_1) \neq \mathcal{F}(L_2).
\]

### Proof

By Theorem 1, there exist \(L_1 \neq L_2\) such that
\[
\Phi[L_1] = \Phi[L_2].
\]

Since equality of \(\Phi\) does not impose pointwise equality of liquidity distributions, there exists a subset of \(I\) on which \(L_1\) and \(L_2\) differ.

Consider a perturbation \(\delta L\) supported on a region where admissibility is preserved for one state but violated for the other (e.g., due to non-negativity constraints).

Then there exists \(\delta L\) such that
\[
L_1 + \delta L \in \mathcal{L}, \quad \text{but} \quad L_2 + \delta L \notin \mathcal{L}.
\]

Therefore,
\[
\delta L \in \mathcal{F}(L_1), \quad \delta L \notin \mathcal{F}(L_2),
\]
and hence
\[
\mathcal{F}(L_1) \neq \mathcal{F}(L_2).
\]

### Corollary 2. Indeterminacy of Local Structural Evolution

Observable price does not uniquely determine the admissible local evolution of the system.

### Corollary 3. Observable Ambiguity of Response

Two states with identical price may admit structurally incompatible responses to the same perturbation.

### Example

Let \(I = [-1,1]\), \(w(p)=1\), and define
\[
L_1(p)=1, \quad L_2(p)=1+\varepsilon p, \quad 0<\varepsilon<1.
\]

Then
\[
\Phi[L_1] = \Phi[L_2].
\]

Consider a localized perturbation \(\delta L\) near \(p=-1\). For sufficiently small perturbations, admissibility may be preserved for \(L_1\) but violated for \(L_2\), demonstrating that admissible future sets differ despite identical price.

---

## 3. Remarks

### Remark 1. Structural Nature of the Result

The results presented in this document are purely structural.  
They do not rely on probabilistic assumptions, stochastic modeling, or specific market microstructure.

The statements follow solely from the properties of observable aggregation and admissible state space structure.

---

### Remark 2. Scope Limitation

The theorems establish limitations of price-based inference.

They do not provide:
- predictive models,
- trading strategies,
- or reconstruction procedures.

---

### Remark 3. Role within WLRT

Within the WLRT framework, these results define a minimal external layer.

They formalize the limits of observable-based reasoning without exposing internal structural mechanisms of the theory.

---

### Remark 4. Interpretation

The results imply that observable price alone is insufficient to determine:
- the underlying liquidity state,
- or the set of admissible local structural transitions.

This establishes a fundamental ambiguity in observable-driven interpretation of system dynamics.

---
