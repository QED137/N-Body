
# N-Bodies Simulation: Chaos In Planetary System

This is an old computational program in Python that I completed during my Master's in Astro and Particle Physics as part of a practical course in Astronomy and Astrophysics coursework.

The gravitation appears deceptively simple when it is put into mathematical form. The weakest among the lot! Its dependence on mass and the infinite range of effects creates an insurmountable difficulty when considering any celestial body's dynamics. In common dictum, each body attracts the other, so the motion of a body has a very complicated dependence on the configurations of other bodies. The N-body problem is about this. This protocol aims to consider an assembly of N-bodies and study the cause and effect among themselves.

## The Problem

Classical mechanics gives a few handfuls of ways of looking at the problem of classical dynamics. Lagrangian and Hamiltonian points of view are essentially similar to each other, but preferences of one over the other depend on the nature of the problem. Hamiltonian method opens a new way of visualizing the problem in the phase space. Since the N-body problem consists of a large number of particles, the Hamiltonian point of view is more feasible.

The motion of N point masses in their mutual gravitational field is the classical N-body problem. The Hamiltonian of a system is

![H equation](https://img.shields.io/badge/H%20=%20\sum_{i=1}^{N}%20\frac{\boldsymbol{p}_i^2}{2m_i}%20-%20\sum_{i=1}^{N}\sum_{j=i+1}^{N}%20\frac{G%20m_i%20m_j}{|\boldsymbol{q}_i-\boldsymbol{q}_j}|)

With canonical momentum ![p equation](https://img.shields.io/badge/\boldsymbol{p}_i%20=%20m\boldsymbol{v}_i)

![Dynamical equation](https://img.shields.io/badge/\frac{d\boldsymbol{r}_i}{dt}%20=%20\boldsymbol{v}_i)

![Momentum equation](https://img.shields.io/badge/\frac{d\boldsymbol{v}_i}{dt}%20=%20\boldsymbol{a}_i)

Where ![Acceleration equation](https://img.shields.io/badge/\boldsymbol{a}_i(t)%20=%20\sum_{j\neq%20i}^{N}%20Gm_j\frac{\boldsymbol{r}_{ij}}{r_{ij}^3})

Where 

![r_ij equation](https://img.shields.io/badge/\boldsymbol{r}_{ij}%20=%20\boldsymbol{r}_j(t)%20-%20\boldsymbol{r}_i(t))

![r equation](https://img.shields.io/badge/r_{ij}%20=%20|\boldsymbol{r}_{ij}|)
![H equation](https://img.shields.io/badge/H%20=%20\sum_{i=1}^{N}%20\frac{\boldsymbol{p}_i^2}{2m_i}%20-%20\sum_{i=1}^{N}\sum_{j=i+1}^{N}%20\frac{G%20m_i%20m_j}{|\boldsymbol{q}_i-\boldsymbol{q}_j}|)



Another formula that will be required further is the jerk

![Jerk equation](https://img.shields.io/badge/\boldsymbol{\dot{a}}_i(t)%20=%20\sum_{j\neq%20i}^{N}%20Gm_j%20\left(\frac{\boldsymbol{v}_{ij}}{r_{ij}^3}%20-%20\frac{3(\boldsymbol{v}_{ij}\cdot\boldsymbol{r}_{ij})}{r_{ij}}\boldsymbol{r}_{ij}%20\right))

Where ![v equation](https://img.shields.io/badge/\boldsymbol{v})

