# Muon

This repository contains the experiments for the paper ["Muon vs. Gradient Descent: Contrasting their Learning Dynamics in Matrix Factorization."](https://www.youtube.com/watch?v=E4WlUXrJgy4)

Authors: Mark Rhee, Jamie Simon, Dhruva Karkada.

## Analysis Notebooks

- [fig1.ipynb](fig1.ipynb) - Spectral learning dynamics of Muon vs. SGD on matrix factorization: singular-value trajectories, training losses, and conservation laws
- [fig2.ipynb](fig2.ipynb) - Flow maps and loss-surface slices for the scalar problem $L(p,q) = \frac{1}{2}(1-pq)^2$, comparing gradient flow against Muon flow
- [fig3.ipynb](fig3.ipynb) - Planted low-rank recovery and subspace alignment across the under-, exactly-, and over-parameterized regimes ($d/n = 0.25, 1.0, 4.0$)

Cached experiment outputs (`*.pkl`) are included so the plotting cells can be re-run without repeating the training sweeps. Figures are written to [plots/](plots).

## Requirements

See [pyproject.toml](pyproject.toml) for dependencies. `uv` virtual environment recommended. Python 3.13+ required.