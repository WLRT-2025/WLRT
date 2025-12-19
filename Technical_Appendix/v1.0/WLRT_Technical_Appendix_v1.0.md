# WLRT — Technical Appendix v1.0
## A. Scope and Relation to White Paper
This Technical Appendix supplements the Wave Liquidity Redistribution Theory (WLRT) —
White Paper v1.0.
Its purpose is to:
- provide formal mathematical clarifications of key concepts introduced in the White
Paper;
- explicitly state assumptions, axioms, and constraints used implicitly in the core text;
- define the limits of validity of the presented models;
- outline directions for future technical extensions without affecting the conceptual
integrity of v1.0.  \
This appendix does not introduce new theoretical claims.  \
All definitions and formulations herein are consistent with, and derived from, Sections
01_Theory and 04_Mathematical_Framework of the White Paper.
## B. Formal Definitions
### B.1 Market Liquidity
Market Liquidity (WLRT) is defined as the bounded capability of a market system to
reallocate value across price levels and time horizons with finite execution costs.  \
Formally, liquidity is treated as a functional:  \
L = L(V, D, F, I)  \
where:
- V — available liquid capital,
- D — distribution of liquidity over price levels,
- F — flows of liquidity over time,
- I — execution costs (impact, slippage, delay).  \
Liquidity is local, finite, and dynamic.
### B.2 Liquidity Distribution
Liquidity Distribution is the spatial-temporal allocation of liquid capital across price and
market scales.  \
It is represented by a density function:  \
rho_L(p, t, s) >= 0  \
where:
- p — price level,
- t — time,
- s — market scale.  \
Properties:
- non-uniform,
- time-dependent,
- partially latent (not fully observable),
- participant-dependent.
### B.3 Liquidity Redistribution
Liquidity Redistribution is the continuous evolution of liquidity distribution driven by
participant actions and external factors.  \
It is described by a conservation-type equation:  \
d rho_L / dt = div J_L + S  \
where: 
- J_L — liquidity flow vector,
- S — sources and sinks of liquidity.  \
Price changes occur as a consequence of asymmetric redistribution.
### B.4 Liquidity Wave
A Liquidity Wave is a localized, directional change in liquidity density propagating through
price and time.  \
Formally:  \
W_L(p,t) = Delta rho_L(p,t)  \
Liquidity Waves:
- have amplitude (magnitude of redistribution),
- have direction (net flow bias),
- propagate across scales,
- may superimpose.  \
Price is interpreted as the observable projection of interacting Liquidity Waves.
## C. Assumptions and Axioms
The WLRT framework relies on the following foundational assumptions:  \
Axiom 1 — Finite Liquidity  \
Liquidity is always bounded:  \
0 < L(p,t) < infinity  \
Axiom 2 — Non-Uniformity  \
Liquidity distribution is never homogeneous:  \
rho_L(p,t) != const  \
Axiom 3 — Continuous Redistribution  \
Liquidity is continuously redistributed:  \
d rho_L / dt != 0  \
Axiom 4 — Liquidity Causality  \
Liquidity redistribution drives price, not vice versa.  \
Axiom 5 — Multi-Scale Consistency  \
Structural properties of Liquidity Waves persist across scales.  
## D. Mathematical Formulation
### D.1 Liquidity Flow
Liquidity flow is defined as:  \
J_L(p,t,s) = rho_L(p,t,s) * v(p,t,s)  \
where v is the effective redistribution velocity.
### D.2 Evolution Equation
The fundamental evolution equation:  \
d rho_L / dt + div (rho_L * v) = S  \
This equation governs:  
- wave formation,
- wave propagation,
- wave dissipation.
### D.3 Price Projection
Price is defined as a functional of liquidity distribution:  \
P(t) = f(rho_L(p,t))  \
No explicit functional form is imposed in v1.0.
## E. Model Constraints and Limits
The WLRT technical model is subject to the following constraints:  
1. Observability Limit  \
Latent liquidity cannot be fully measured.
2. Resolution Tradeoff  \
Higher temporal resolution reduces market-scale visibility.
3. Market Frictions  \
Fees, delays, and spreads distort ideal wave dynamics.
4. Exogenous Shocks  \
Extreme events may temporarily violate modeled continuity.
5. Non-Stationarity  \
Market structure evolves; parameters are time-dependent.  \
WLRT describes structural tendencies, not deterministic outcomes.
## F. Notes for Future Extensions
Planned technical extensions beyond v1.0 include:
- explicit modeling of latent liquidity fields;
- stochastic source terms S(p,t);
- cross-market coupled wave systems;
- algorithmic estimation of rho_L from partial data;
- integration with agent-based and AMM-specific dynamics.  \
These extensions will be addressed in future versions without altering the core axioms.  \
Status: WLRT — Technical Appendix v1.0  \
Relation: Supplementary to White Paper v1.0  \
Consistency: Fully aligned with WLRT core theory
