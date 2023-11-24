
# N-Bodies Simulation: Chaos In Planetary System

This is an old computational program in Python that I completed during my Master's in Astro and Particle Physics as part of a practical course in Astronomy and Astrophysics coursework.

The gravitation appears deceptively simple when it is put into mathematical form. The weakest among the lot! Its dependence on mass and the infinite range of effects creates an insurmountable difficulty when considering any celestial body's dynamics. In common dictum, each body attracts the other, so the motion of a body has a very complicated dependence on the configurations of other bodies. The N-body problem is about this. This protocol aims to consider an assembly of N-bodies and study the cause and effect among themselves.

## The Problem

Classical mechanics gives a few handfuls of ways of looking at the problem of classical dynamics. Lagrangian and Hamiltonian points of view are essentially similar to each other, but preferences of one over the other depend on the nature of the problem. Hamiltonian method opens a new way of visualizing the problem in the phase space. Since the N-body problem consists of a large number of particles, the Hamiltonian point of view is more feasible.

The motion of N point masses in their mutual gravitational field is the classical N-body problem. The Hamiltonian of a system is

$$
H = \sum_{i=1}^{N} \frac{\boldsymbol{{p}}^2_i}{2m_i}-\sum_{i=1}^{N}\sum_{j=i+1}^{N}\frac{G m_i m_j}{|\boldsymbol{q}_i-\boldsymbol{q}_j|}
$$



With canonical momentum $\boldsymbol{p}_i=mv_i$.

$m_i$ is the mass of the particle located at $r_i$.

$$
\boldsymbol{q}_i  = \frac{\partial H}{\partial \boldsymbol{p}_i} \implies \frac{d\boldsymbol{r}_i}{dt} = \boldsymbol{v}_i
$$

and

$$
\boldsymbol{p}_i  = -\frac{\partial H}{\partial \boldsymbol{q}_i} \implies \frac{d\boldsymbol{v}_i}{dt} = \boldsymbol{a}_i
$$

Where  $a_i$  is the acceleration,


$$
\boldsymbol{a}_{i}(t) = \sum^{N}_{j\neq i} Gm_j \frac{\boldsymbol{r}}{r}
$$




Where


$$
\boldsymbol{r}_{ij}  = \boldsymbol{r}_j(t)-\boldsymbol{r}_i(t) 
r_{ij}  = |\boldsymbol{r}_{ij}|
$$


Another formula that will be required further is the jerk


$$
\boldsymbol{\dot{a}}_i(t)=\sum_{j\neq i}^{N} Gm_j \left(\frac{\boldsymbol{v}_{ij}}{r^3_{ij}}-\frac{3(\boldsymbol{v}_{ij}\cdot\boldsymbol{r}_{ij})}{r_{ij}}\boldsymbol{r}_{ij} \right)
$$


$\boldsymbol{v}$ is the velocity of the $i$th particle.

