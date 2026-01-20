# WLRT Core — Canonical Freeze Declaration (Including EEM)

**Status:** FROZEN  
**Scope:** WLRT Core (v3.x lineage; forward-compatible with v4.0)  
**Fixation date:** 2026-01-20  
**Repository:** WLRT-2025/WLRT

## 1. Object of Freeze

The following WLRT Core components are canonically frozen and must not be conceptually modified within this scope:

- Phase Space & Phase Logic
- Local Fragility Index (LFI)
- Ultra-Short Regime (USR)
- Phase Irreversibility Principle
- Redistribution Logic
- Decision-Aware Agents (DAA)
- Phase Time Module
- **Emergency Economics Module (EEM)** — fixed as **Appendix E**

## 2. Inclusion of EEM (Appendix E)

The **Emergency Economics Module (EEM)** is recognized as a **Core structural module**:

- Non-optional for analysis of **high-LFI regimes**
- Logically consistent with the existing Core invariants
- Domain-independent (no market- or sector-specific assumptions)

EEM introduces an explicit **inter-event memory** requirement through **Stability Reserve (SR)** accumulation logic, without introducing new Core primitives.

## 3. Canonical Invariant Relation

EEM makes explicit a Core-consistent relation:

> Repeated high-LFI events without stability accumulation lead to increasing effective fragility and degraded execution viability.

## 4. Prohibited Modifications

After this freeze, the following are prohibited within WLRT Core:

- Introduction of new primitives
- Re-definition of LFI or phase logic
- Removal, weakening, or “application-only” relegation of EEM
- Conversion of EEM into a normative optimization framework
- Market-, sector-, or agent-specific assumptions inside Core

## 5. Allowed Future Work (Derivative Only)

The following are allowed provided they do not alter the frozen Core semantics:

- Applied layers (ROM, EEP, LLAP, Playbooks, Service Packs)
- Empirical illustrations and case studies
- Sector-specific implementations
- Mathematical formalization in future versions
- Publication packaging (SSRN/arXiv/Zenodo), provided Core invariants are preserved

## 6. Canonical Reference

This declaration is the single source of truth for the frozen WLRT Core state in this repository.
