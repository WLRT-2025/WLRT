# WLRT — Wave Liquidity Redistribution Theory
White Paper v1.0 \
  \
  Status: Research White Paper  \
Version: 1.0  \
License: CC BY 4.0  \
Date: 2025-12-19
## Abstract
This white paper presents the Wave Liquidity Redistribution Theory (WLRT), a universal market model in which observed price dynamics emerge from wave-like redistribution of liquidity across price space. Financial markets are treated as structured dynamical systems governed by conservation, propagation, and dissipation of liquidity. Price is defined as a secondary observable derived from the state of the liquidity field rather than as a primary driver.
## 1. Motivation
Most existing market models focus on price trajectories, indicators, or agent behavior. Such approaches describe market outcomes but rarely address price formation itself. WLRT proposes a different modeling layer: price is not a fundamental variable. Price is an observable projection of internal liquidity dynamics. This document introduces the minimal linear formulation of the theory.
## 2. Price Space Representation
The market is represented as a one-dimensional price space P. The space is divided into discrete price sectors. Each sector contains an amount of effective liquidity. Liquidity may redistribute between neighboring sectors. The geometry of price space is fixed and uniform in this version.
## 3. Fundamental Quantities
The model introduces the following quantities:
- rho(P,t): liquidity density
- grad rho: liquidity gradient
- J(P,t): liquidity flux
- c: characteristic redistribution speed
- gamma: dissipation (market friction)
- S(P,t): external liquidity sources and sinks
Causal structure: liquidity gradient -> liquidity flux -> liquidity waves -> observed price
## 4. Definition of Price
Observed price is defined as the liquidity-weighted center of the system:  \
P(t) = integral(P * rho(P,t) dP) / integral(rho(P,t) dP).  \
Price reflects the instantaneous configuration of the liquidity field and does not represent discrete transactions.
## 5. Liquidity Dynamics
Liquidity redistribution is described by a damped wave equation:  \
d2 rho / dt2 + gamma * d rho / dt = c^2 * d2 rho / dP2 + dS / dt.  \
This equation captures inertia of liquidity, propagation across price levels, and dissipation due to friction and execution costs.
## 6. Market Regimes
Different classes of solutions correspond to common market regimes: standing waves correspond to range-bound markets, traveling waves to directional trends, critical damping to flat or inactive markets, and impulse responses to news-driven movements. Regime transitions arise from changes in boundary conditions or external inputs.
## 7. Conservation Properties
In the absence of external sources S, total liquidity is conserved, local inflows equal local outflows, and system behavior is scale-invariant. Violations of conservation indicate external intervention.
## 8. Interpretation of Volatility
Volatility corresponds to the amplitude of liquidity oscillations and the intensity of redistribution processes. High volatility reflects strong internal dynamics rather than randomness or noise.
## 9. GRID Trading Systems
A GRID trading system is interpreted as a discrete wave resonator. Grid boundaries create standing liquidity waves, repeated reflections generate dissipation, and profit arises from energy loss during oscillations. GRID systems are effective only in oscillatory regimes.
## 10. Failure Conditions of GRID Systems
GRID systems fail when directional liquidity flux dominates, standing waves collapse, or boundary conditions are violated. Failure represents a regime transition rather than an execution error.
## 11. Scope and Non-Claims
WLRT does not predict exact prices, does not rely on indicators, and does not assume rational or optimal agents. The theory models structural dynamics rather than forecasts.
## 12. Model Assumptions and Limitations
WLRT v1.0 assumes linear liquidity response, fixed price-space geometry, and passive liquidity behavior. These assumptions define the scope of applicability.
## 13. Conclusion
WLRT provides a minimal, causal, and geometric framework for understanding market dynamics through liquidity redistribution. Price emerges as a secondary observable of the system's internal state.

## Disclaimer
This document describes a theoretical research model and does not constitute financial or investment advice.
