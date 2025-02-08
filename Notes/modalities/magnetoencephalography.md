2025-02-08 00:24

Sources: 

Tags:

**Magnetoencephalography (MEG)** is a [[passive sensing]] technique that measures [[electrophysiological brain activity]] by reconstructing primary current sources from [[magnetic field]] recordings on the scalp.

![[meg_setup.png|300]]
# Theory

We denote MEG measurement recordings $M(\mathbf{x}_\text{sensors}, t) \in Y$ to be a:
- a single component of the magnetic field $\mathbf{B}(\mathbf{x},t)$, measured in tesla $\text{T}$, for a magnetometer readout
- the spatial derivative of a component of $\mathbf{B}(\mathbf{x},t)$, $\frac{\partial B_n}{\partial x}$, e.g., $$B_n(\mathbf{x}_1,t)-B_n(\mathbf{x}_2,t)$$ for the simplest gradiometer readout, where $\mathbf{x}_1$ and $\mathbf{x}_2$ are two nearby sensor locations.

We make explicit the dependence of measurements $M(\mathbf{x}_\text{sensors}, t) \in Y$ at sensor positions $\mathbf{x}_\text{sensors}$, on the primary current density $\mathbf{J}_p(\mathbf{x},t) \in X$, measured in amperes per squared meter $\frac{\text{A}}{\text{m}^2}$, due to neuronal activity: $$M(\mathbf{x}_\text{sensors}, t)=\mathcal{F}\mathbf{J}_p + \delta M, \tag{1}$$where:
- $X$ is a Hilbert space of functions representing admissible current densities,
- $Y$ is a Hilbert space of functions representing admissible measurement recordings,
- $\delta M(\mathbf{x}_\text{sensors}, t)$ represents the noise component of the $M(\mathbf{x}_\text{sensors}, t)$ signal,
- $\mathcal{F}:X \rightarrow Y$ is an [[operator]] that models how $\mathbf{J}_p(\mathbf{x},t)$ gives rise to $M(\mathbf{x}_\text{sensors}, t)$ in the absence of noise. 

We can define the action of $\mathcal{F}$ on $\mathbf{J}_p$ more precisely as: $$(\mathcal{F}\mathbf{J}_p)(\mathcal{x}_\text{sensors}, t)=\mathcal{R}\mathbf{B}_{\mathbf{J}_p},\tag{2}$$where:
- $\mathbf{B}_{\mathbf{J}_p}(\mathbf{x},t) \in \mathcal{B}$ is the magnetic field that depends implicitly on $\mathbf{J}_p(\mathbf{x},t)$,
- $\mathcal{B}$ is a Hilbert space of functions that represents all admissible magnetic fields,
- $\mathcal{R}:\mathcal{B} \rightarrow Y$ is an operator that extracts $\mathbf{B}_{\mathbf{J}_p}(\mathbf{x},t)$ at sensor positions $\mathbf{x}_\text{sensors}$ and outputs measurements according to the sensor type (e.g. magnetometer, gradiometer)

Previously (c.f. [[electroencephalogram]]), we derived $\mathbf{B}(\mathbf{x},t)$ as the solution to the system of equations: $$\begin{align}
\nabla\cdot(\sigma\nabla\phi)&=\nabla\cdot\mathbf{J}_p \\
\sigma\nabla\phi &= \frac{1}{\mu_0}(\nabla\times\mathbf{B}) - \mathbf{J}_p 
\end{align}\tag{3}$$where $\sigma(\mathbf{x}, t)$ is the electrical conductivity, measured in ohm meter $\Omega\cdot\text{m}$, $\phi(\mathbf{x},t)$ is the electric potential, measured in volts $\text{V}$, and $\mu_0$ is the permeability of free space, measured in henry per meter $\frac{\text{H}}{\text{m}}$.

Magnetoencephalography attempts to solve the inverse of equation $(1)$, i.e., determining $\mathbf{J}_p(\mathbf{x},t)$ from $M(\mathbf{x}_\text{sensors}, t)$. Since $M(\mathbf{x}_\text{sensors}, t)$ is unlikely to lie exactly within the range of $\mathcal{F}$ due to the presence of noise and modeling inaccuracies, the problem is reformulated as finding the optimal $\mathbf{J}_p^\dagger(\mathbf{x}, t)$ whose response $\mathcal{F}\mathbf{J}_p^\dagger$ best matches $M(\mathbf{x}_\text{sensors}, t)$. This reformulation involves minimizing the distance between $M(\mathbf{x}_\text{sensors}, t)$ and $\mathcal{F}\mathbf{J}_p$, defined using a suitable metric and encoded as an objective function, or in the sense of the calculus of variations, a [[functional]] $J$: $$\min_{\mathbf{J}_p} \quad J[\mathbf{J}_p].$$A common choice for $J$ is the least-squares misfit: $$J_\text{LS}[\mathbf{J}_p] = \frac{1}{2} \|M(\mathbf{x}_\text{sensors}, t) - \mathcal{F}\mathbf{J}_p\|_2^2$$where $||M(\mathbf{x}_\text{sensors}, t)||_2^2$ is the $L^2$ norm squared in the space of vectors indexed by $\mathbf{x}_\text{sensors}$ (discrete) and $t$ (continuous, say).