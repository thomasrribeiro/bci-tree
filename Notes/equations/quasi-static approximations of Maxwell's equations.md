2025-02-08 12:46

Sources: 

Tags:

The **quasi-static approximations of Maxwell's equations** simplify [[Maxwell's equations]] by neglecting terms associated with time-dependent effects and displacement currents when the system operates at low frequencies. These approximations are valid when the electromagnetic wave propagation time is much shorter than the temporal variations of the sources. 

Applied to [[electrophysiological brain activity]], the following assumptions can be made:
- non-magnetic tissues
- electrical conductivity $\sigma$ of brain tissue on the order of $0.3 \frac{\text{S}}{\text{m}}$,
- brain activity at low frequencies (up to the order of $100\text{Hz}$)

Since the time-dependent components of the [[electric field]] and the [[magnetic field]] are negligible, [[Faraday's law]] simplifies to: $$\nabla \times \mathbf{E} = 0.\tag{1}$$where $\mathbf{E}(\mathbf{x},t)$ is the electric field, measured in volts per meter $\frac{\text{V}}{\text{m}}$. This implies that the electric field is conservative and can be expressed as the gradient of a scalar potential $\phi(\mathbf{x},t)$: $$\mathbf{E}=-\nabla \phi\tag{2}$$where $\phi(\mathbf{x},t)$ is called the electric potential, measured in volts $\text{V}$. Additionally, the [[Ampère-Maxwell's law]] simplifies to: $$\mu_0\mathbf{J} = \nabla \times \mathbf{B}\tag{3}$$where $\mu_0$ is the permeability of free space, measured in henry per meter $\frac{\text{H}}{\text{m}}$, and $\mathbf{B}(\mathbf{x},t)$ is the magnetic field, measured in tesla $\text{T}$. Taking the divergence of both sides results in: $$
\begin{align}
\nabla \cdot(\mu_0\mathbf{J}) &= \nabla \cdot(\nabla \times \mathbf{B}) \\[1.5ex]
\nabla \cdot\mathbf{J} &= 0 \tag{4}
\end{align}
$$since the divergence of a curl is zero.

Neuronal activity generates primary currents due to transmembrane ionic fluxes. These currents give rise to a primary current density $\mathbf{J}_p(\mathbf{x},t)$, measured in amperes per squared meter $\frac{\text{A}}{\text{m}^2}$, which represents the flow of charge carriers in the extracellular space. The total current density $\mathbf{J}(\mathbf{x},t)$ consists, then, of two components $$\mathbf{J}=\mathbf{J}_p + \mathbf{J}_v\tag{5}$$where $\mathbf{J}_v(\mathbf{x},t)$ is the volume current density induced by passive conduction in brain tissue which is equal to: $$\mathbf{J}_v=-\sigma\nabla\phi\tag{6}$$by [[Ohm's law]], where $\sigma(\mathbf{x}, t)$ is the electrical conductivity measured in siemens per meter $\frac{\text{S}}{\text{m}}$. Substituting equations $(5)$, $(6)$ in equation $(4)$ and $(5)$, respectively, we obtain the system of equations: $$\begin{align}
\nabla\cdot(\sigma\nabla\phi)&=\nabla\cdot\mathbf{J}_p \\
\sigma\nabla\phi &= \frac{1}{\mu_0}(\nabla\times\mathbf{B}) - \mathbf{J}_p 
\end{align}\tag{7}$$