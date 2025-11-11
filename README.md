# GALAHAD: Geometry-Adaptive Lyapunov-Assured Hybrid Optimizer

[![CRAN status](https://www.r-pkg.org/badges/version/GALAHAD)](https://CRAN.R-project.org/package=GALAHAD)
[![Downloads](https://cranlogs.r-pkg.org/badges/GALAHAD)](https://CRAN.R-project.org/package=GALAHAD)
[![DOI (CRAN)](https://img.shields.io/badge/DOI-10.32614%2FCRAN.package.GALAHAD-blue.svg)](https://doi.org/10.32614/CRAN.package.GALAHAD)
[![DOI (Zenodo)](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.17552616-blue.svg)](https://doi.org/10.5281/zenodo.17552616)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

---

> For the full reproducibility statement, algorithmic framework, and references, see the  
> [CRAN README](https://cran.r-project.org/package=GALAHAD/readme/README.html).

---

## Overview

**GALAHAD** (Geometry-Adaptive Lyapunov-Assured Hybrid Optimizer) is a biologically informed optimization framework that integrates Lyapunov-stability principles, trust-region methods, and geometry-aware updates.  
It was developed to handle parameter spaces containing a mix of positive-only, logarithmic, and unconstrained variables — common in biological and environmental modeling.

Unlike conventional Euclidean optimizers, **GALAHAD** maintains numerical stability across heterogeneous parameter geometries, improving convergence behavior for small, noisy, or ill-conditioned datasets.  

---

## Key Features

| Capability | Description |
|-------------|--------------|
| **Per-geometry parameter updates** | Handles logarithmic, positive, and unconstrained parameters under a unified optimizer |
| **Trust-region projection** | Adapts step length to local curvature and scaling |
| **Lyapunov stability checks** | Ensures ΔV ≤ 0 at each iteration for numerical robustness |
| **Hybrid step-size control** | Combines Polyak and Barzilai–Borwein adaptive heuristics |
| **Halpern averaging** | Reduces oscillations in noisy or irregular datasets |

---

## Installation

Install the latest CRAN release:

```r
install.packages("GALAHAD")
