# Local Fragility Index (LFI)

## Definition

The **Local Fragility Index (LFI)** is a scalar measure of the
**local susceptibility of a liquidity field to phase transition**
under small perturbations.

Formally, LFI quantifies how close a market system is to a **loss of local
stability**, independent of the direction of subsequent price movement.

---

## What LFI Measures

LFI measures:
- concentration and depletion of available liquidity;
- imbalance between liquidity supply and absorption capacity;
- structural tension within the order flow;
- sensitivity of the system to marginal shocks.

In WLRT terms, LFI reflects the **local curvature and stress** of the liquidity field.

---

## What LFI Does NOT Measure

LFI does **not** measure:
- future price direction;
- expected return;
- volatility magnitude;
- profitability of any strategy.

High LFI indicates **fragility**, not inevitability.

---

## Conceptual Interpretation

- Low LFI  
  → liquidity field locally stable  
  → perturbations are absorbed smoothly

- Increasing LFI  
  → rising sensitivity to perturbations  
  → accumulation of unresolved liquidity imbalance

- High LFI  
  → proximity to phase transition  
  → small shocks may trigger regime change

---

## Relation to WLRT Phases

LFI is defined locally and continuously.
Phase transitions correspond to **critical LFI regimes**, not to fixed thresholds.

Different WLRT phases may share similar price behavior but differ in LFI dynamics.

---

## Scale and Invariance

LFI is:
- dimensionless;
- scale-invariant under price and volume rescaling;
- comparable across assets only after normalization.

---

## Epistemic Status

LFI is an **indicator of structural risk**, not a predictive oracle.

Its value lies in:
- early detection of instability;
- exclusion of false confidence during calm regimes;
- disciplined separation of fragility and direction.

---

## Canonical Constraint

Any application of LFI must explicitly state:
- data sources;
- temporal resolution;
- aggregation window;
- known limitations.

Absence of these invalidates interpretation.
