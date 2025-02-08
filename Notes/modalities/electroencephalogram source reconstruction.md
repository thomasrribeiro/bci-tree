2025-02-08 00:01

Sources: 

Tags:

**Electroencephalogram source reconstruction** is a [[passive sensing]] technique that reconstructs primary current density sources, due to [[electrophysiological brain activity]], from electric potential recordings on the scalp obtained using [[electroencephalogram]].

# Theory

We make explicit the dependence of voltage recordings $V(\mathbf{x}_\text{sensors}, t) \in Y$ at electrode positions $\mathbf{x}_\text{sensors}$, on the primary current density $\mathbf{J}_p(\mathbf{x},t) \in X$ due to neuronal activity: $$V(\mathbf{x}_\text{sensors}, t)=\mathcal{F}\mathbf{J}_p + \delta V,$$where:
- $X$ is a Hilbert space of functions representing admissible current densities,
- $Y$ is a Hilbert space of functions representing admissible voltage recordings,
- $\delta V(\mathbf{x}_\text{sensors}, t)$ represents the noise component of the $V(\mathbf{x}_\text{sensors}, t)$ signal,
- $\mathcal{F}:X \rightarrow Y$ is an [[operator]] that models how $\mathbf{J}_p(\mathbf{x},t)$ gives rise to $V(\mathbf{x}_\text{sensors}, t)$ in the absence of noise. 

We can define the action of $\mathcal{F}$ on $\mathbf{J}_p$ more precisely as: $$(\mathcal{F}\mathbf{J}_p)(\mathcal{x}_\text{sensors}, t)=\mathcal{R}\phi_{\mathbf{J}_p},$$where:
- $\phi_{\mathbf{J}_p}(\mathbf{x},t) \in \Phi$ is the electric potential that depends implicitly on $\mathbf{J}_p(\mathbf{x},t)$
- $\Phi$ is a Hilbert space of functions that represents all admissible electric potentials
- $\mathcal{R}:\Phi \rightarrow Y$ is a sampling operator that extracts $\phi_{\mathbf{J}_p}(\mathbf{x},t)$ at electrode positions $\mathbf{x}_\text{sensors}$ and subtracts the values relative to a reference electric potential $\phi_{\mathbf{J}_p}(A,t)$ at a position $A$.

Previously (c.f. [[electroencephalogram]]), we derived $\phi(\mathbf{x},t)$ as the solution to the equation: $$\nabla\cdot(\sigma\nabla\phi)=\nabla\cdot\mathbf{J}_p.$$where $\sigma(\mathbf{x}, t)$ is the electrical conductivity measured in ohm meter $\Omega\cdot\text{m}$. Electroencephalogram source reconstruction attempts to solve the inverse problem, i.e., determining $\mathbf{J}_p(\mathbf{x},t)$ from $V(\mathbf{x}_\text{sensors}, t)$. 

Since $V(\mathbf{x}_\text{sensors}, t)$ is unlikely to lie exactly within the range of $\mathcal{F}$ due to the presence of noise and modeling inaccuracies, the problem is reformulated as finding the optimal $\mathbf{J}_p^\dagger(\mathbf{x}, t)$ whose response $\mathcal{F}[\mathbf{J}_p^\dagger]$ best matches $V(\mathbf{x}_\text{sensors}, t)$. This reformulation involves minimizing the distance between $V(\mathbf{x}_\text{sensors}, t)$ and $\mathcal{F}[\mathbf{J}_p]$, defined using a suitable metric and encoded as an objective function, or in the sense of the calculus of variations, a functional $J$: $$\min_{\mathbf{J}_p} \quad J[\mathbf{J}_p].$$A common choice for $J$ is the least-squares misfit: $$J_\text{LS}[\mathbf{J}_p] = \frac{1}{2} \|V(\mathbf{x}_\text{sensors}, t) - \mathcal{F}\mathbf{J}_p\|_2^2$$where $||V(\mathbf{x}_\text{sensors}, t)||_2^2$ is the $L^2$ norm squared in the space of vectors indexed by $\mathbf{x}_\text{sensors}$ (discrete) and $t$ (continuous, say).