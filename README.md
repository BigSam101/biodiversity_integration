# Biodiversity Constraints and Power System Impacts (Belgium, PyPSA-Eur)

This repository contains analysis code investigating the impact of
biodiversity-driven wind constraints on electricity system performance
using PyPSA-Eur.

The study explores how limiting wind deployment affects system cost,
electricity prices, and reliance on backup generation, under both
deterministic and uncertainty-aware settings.

## Scope
- Belgium electricity system case study (PyPSA-Eur)
- Biodiversity constraints on wind deployment
- Sensitivity analysis of wind availability
- Scenario-based uncertainty analysis (Monte Carlo-style sampling)
- Trade-offs between cost, reliability, and renewable penetration

## Methodology
Wind generation availability is modified to represent biodiversity
constraints (e.g. land-use restrictions, ecological limits).

Two complementary analyses are performed:
- **Deterministic sensitivity analysis** across wind availability levels
- **Stochastic uncertainty analysis** using sampled wind scenarios

System performance is evaluated using:
- Total system cost
- Average electricity price
- Backup generation share

## Key Findings
- Stronger biodiversity constraints (lower wind availability) lead to:
  - Higher system costs
  - Increased reliance on backup generation
  - Greater uncertainty in system outcomes

- Increased wind availability results in:
  - Lower system costs
  - Reduced electricity prices
  - Lower dependence on backup generation

- Biodiversity constraints introduce a clear trade-off between:
  - Environmental protection
  - Economic efficiency
  - System reliability

## Repository Structure
- `notebooks/` – Main analysis notebook (`energy_mod_BE.ipynb`)
- `scripts/` – Helper functions (if added later)
- `figures/` – Generated plots

## Requirements
- Python 3.10+
- PyPSA / PyPSA-Eur
- HiGHS or Gurobi solver

## Notes
This repository contains analysis code only.
Large input data and solved network files are not included.