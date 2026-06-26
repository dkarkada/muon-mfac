# Muon

This repository contains the experiments for the paper ["Muon vs. Gradient Descent: Contrasting their Learning Dynamics in Matrix Factorization."](https://www.youtube.com/watch?v=E4WlUXrJgy4)

Authors: Mark Rhee, Jamie Simon, Dhruva Karkada.

## Analysis Notebooks

- [fig1.ipynb](fig1.ipynb) - Spectral learning dynamics of Muon vs. SGD on matrix factorization: singular-value trajectories, training losses, and conservation laws
- [fig2.ipynb](fig2.ipynb) - Flow maps and loss-surface slices for the scalar problem $L(p,q) = \frac{1}{2}(1-pq)^2$, comparing gradient flow against Muon flow
- [fig3.ipynb](fig3.ipynb) - Planted low-rank recovery and subspace alignment across the under-, exactly-, and over-parameterized regimes ($d/n = 0.25, 1.0, 4.0$)
- [fig4.ipynb](fig4.ipynb) - Spiked learning rate schedule in the exactly-parameterized setting ($n = d = 25$) with orthogonal initialization at scale $\alpha = 10^{-4}$: singular-value trajectories, loss, and learning rate schedule over 16 iterations, demonstrating two-step alignment followed by geometric annealing to convergence

Figures are written to [plots/](plots).

## Requirements

See [pyproject.toml](pyproject.toml) for dependencies. `uv` virtual environment recommended. Python 3.13+ required.
