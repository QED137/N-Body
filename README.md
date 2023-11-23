From classical mechanics gives a few handful way of looking at the problem of classical dynamics. Lagrangian and Hamiltonian point of view is essentially similar to each other, but preferences of one over the other depend on the nature of the problem. Hamiltonian method opens a new way of visualizing the problem in the phase space. Since, N-body problem consists of large number of particles, so Hamiltonian point of view is more feasible. \\
The motion of N point masses in their mutual gravitational field is the classical N -body problem.
The Hamiltonian of a system is 

    $$H= \sum_{i=1}^{N} \frac{\boldsymbol{{p}}^2_i}{2m_i}-\sum_{i=1}^{N}\sum_{j=i+1}^{N}\frac{G m_i m_j}{|\boldsymbol{q}_i-\boldsymbol{q}_j|}$$

With canonical momentum $\boldsymbol{p}_i=mv_i$.
$m_i$ is the mass of particle located at $r_i$.
\begin{gather}\label{dynamical}
    \boldsymbol{q}_i=\frac{\partial H}{\partial \boldsymbol{p}_i}
    \implies \frac{d\boldsymbol{r}_i}{dt}=\boldsymbol{v}_i\\
    \boldsymbol{p}_i=-\frac{\partial H}{\partial \boldsymbol{q}_i}
    \implies \frac{d\boldsymbol{v}_i}{dt}=\boldsymbol{a}_i
\end{gather}
Where $a_i$ is the acceleration,
\begin{equation}\label{acceleration}
    \boldsymbol{a}_i(t)=\sum_{j\neq i}^{N} =Gm_j\frac{\boldsymbol{r}_{ij}}{r^3_{ij}}
\end{equation}
Where 
\begin{gather}\label{absr}
    \boldsymbol{r}_{ij}=\boldsymbol{r}_j(t)-\boldsymbol{r}_i(t)\\
    r_{ij}= |\boldsymbol{r}_{ij}|
\end{gather}
Another formula that will be required further is the jerk
\begin{equation}\label{jerk}
    \boldsymbol{\dot{a}}_i(t)=\sum_{j\neq i}^{N} Gm_j \left(\frac{\boldsymbol{v}_{ij}}{r^3_{ij}}-\frac{3(\boldsymbol{v}_{ij}\cdot\boldsymbol{r}_{ij})}{r_{ij}}\boldsymbol{r}_{ij} \right)
\end{equation}
$\boldsymbol{v}$ is velocity of $i$th particle.
