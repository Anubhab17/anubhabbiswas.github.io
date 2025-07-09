---
title: "Probabilistic Nonlinear Forecast Reconciliation Methods: Projection, Importance Sampling, and Kalman Filtering"
collection: talks
type: "Talk"
permalink: /talks/ISF-2025
venue: "International Symposium on Forecasting (ISF) 2025, Beijing"
date: 2025-07-02
location: "Friendship Palace, Haidian dist, Beijing, China"
---

A brief discussion on a work in progress - probabilistic nonlinear forecast reconciliation

**Slides**:

You can find the slides here:
[▶️ View the slides (HTML)](/anubhabbiswas.github.io/files/ISF_presentation_2025.html)


**Abstract**:

So far probabilistic forecast reconciliation has been studied assuming linear dependencies between time series. In this study, we focus on nonlinear reconciliation, in which the time series are linked by a nonlinear function f. We assume f to be known.
We propose four probabilistic methods for nonlinear forecast reconciliation, which extend to the nonlinear case some methods already existing in the linear case.
The Non-linear Bottom-Up (NL-BU) offers a simple baseline: it samples from the joint distribution of the independent (bottom) time series, and passes them through the function f, providing a distribution for the dependent (upper) time series. The Non-linear Orthogonal Projection (NL-OP) method extends the linear projection framework to the nonlinear case by solving a constrained optimization problem using Newton-Raphson updates. We also adapt the Non-linear Bottom-Up Importance Sampling (NL-BUIS) approach for nonlinear dependencies, using the bottom-level distribution as a proposal and reweighting samples based on the upper-level likelihood. Finally, we propose a novel use of the Unscented Kalman Filter (UKF) to update bottom-level distributions using nonlinear information from the upper level, yielding coherent probabilistic forecasts.
We evaluate all methods on a simulated case. We generate two time series via autoregressive processes and derive a third by summing their squared values. Results based on the energy score show that the UKF and NL-OP methods outperform both the base and bottom-up forecasts, achieving the highest probabilistic accuracy. In terms of log score at the bottom level, both UKF and NL-OP again perform best, with BUIS offering moderate improvements over the bottom-up approach. These findings highlight the UKF and nonlinear projections as strong candidates for probabilistic reconciliation in the nonlinear setting.
Finally, the possibility and the relevance of using different probabilistic metrics to score forecasts for nonlinearly connected time series, based on the geodesic distance, is discussed.
