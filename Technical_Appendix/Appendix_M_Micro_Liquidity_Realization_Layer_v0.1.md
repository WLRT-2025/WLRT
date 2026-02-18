# Appendix M — Micro-Liquidity Realization Layer (MLRL) v0.1

**Status:** Draft-Validated (empirical, single dataset)  
**Scope:** WLRT Core-compatible derivative appendix (U_micro)  
**Fixation date:** 2026-02-18  

---

## M.1 Purpose

This appendix formalizes a micro-level observable layer of liquidity realization consistent with WLRT Core principles.

It does not introduce a trading signal.
It documents an empirically observed mechanism linking:

- localized liquidity realization
- structural compression
- subsequent regime expansion

---

## M.2 Definition of Micro-Event (MEC-T)

A Micro-Event is defined over a fixed number of trades.

Let:

- N = fixed number of trades per window  
- ΔP_cluster = max(price) − min(price) inside window  
- V_cluster = sum(quantity) inside window  

Define intensity:

I = V_cluster / ΔP_cluster

The window is transaction-count based, not time-based.

---

## M.3 Interpretation

Execution represents realized liquidity and satisfaction of both counterparties.

After execution, participants often exit the local zone.
This creates temporary local depletion or restructuring of liquidity.

High intensity therefore corresponds to:

- dense realization
- local structural compression
- formation of a temporary “hole” in the liquidity field

---

## M.4 Post-Event Reaction

For a forward horizon H trades:

R(H) = ΔP_forward(H) / ΔP_cluster

Empirical observation (single dataset):

- Intensity positively correlates with R(H)
- Nonlinear threshold effect observed
- No persistent directional bias detected

Micro-intensity predicts regime expansion, not direction.

---

## M.5 Relation to LFI

This layer does not redefine LFI.

High intensity events may be interpreted as micro-scale fragility impulses consistent with LFI dynamics.

Aggregation to structural LFI is not yet defined.

---

## M.6 Constraints

This layer:

- does not encode direction
- does not generate trade signals
- does not modify WLRT Core semantics
