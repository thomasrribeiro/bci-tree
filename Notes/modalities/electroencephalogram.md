2025-02-07 18:03

Sources: 

Tags:

**Electroencephalogram (EEG)** is a [[passive sensing]] technique that measures [[electrophysiological brain activity]] by recording differences in electric potentials, i.e., voltages, on the scalp.

![[eeg_setup.png|300]]

# Theory

Some simplifications can be made by considering the following characteristics:
- non-magnetic tissues
- electrical conductivity of brain tissue on the order of $\sigma =0.3 \frac{\text{S}}{\text{m}}$
- low frequency of brain activity (up to the order of $100\text{Hz}$)

Under these quasi-static approximations, the time-dependent components of the [[electric field]] and the [[magnetic field]] are negligible. [[Faraday's law]] simplifies to: $$\nabla \times \mathbf{E} = 0.$$where $\mathbf{E}(\mathbf{x},t)$ is the electric field, measured in volts per meter $\frac{\text{V}}{\text{m}}$. This implies that the electric field is conservative and can be expressed as the gradient of a scalar potential $\phi(\mathbf{x},t)$: $$\mathbf{E}=-\nabla \phi$$where $\phi(\mathbf{x},t)$ is called the electric potential, measured in volts $\text{V}$. Additionally, the [[Ampère-Maxwell's law]] simplifies to: $$
\begin{align}
\mu_0\mathbf{J} &= \nabla \times \mathbf{B} \\[1.5ex]
\mu_0(\nabla \cdot\mathbf{J}) &= \nabla \cdot(\nabla \times \mathbf{B}) \\[1.5ex]
\nabla \cdot\mathbf{J} &= 0
\end{align}
$$since the divergence of a curl is zero.

Neuronal activity generates primary currents due to transmembrane ionic fluxes. These currents give rise to a primary current density $\mathbf{J}_p(\mathbf{x},t)$, measured in amperes per squared meter $\frac{\text{A}}{\text{m}^2}$, which represents the flow of charge carriers in the extracellular space. The total current density $\mathbf{J}(\mathbf{x},t)$ consists, then, of two components $$\mathbf{J}=\mathbf{J}_p + \mathbf{J}_v$$where $\mathbf{J}_v(\mathbf{x},t)$ is the volume current density induced by passive conduction in brain tissue. Applying [[Ohm's law]], we obtain: $$\mathbf{J}_v=-\sigma\nabla\phi$$where $\sigma(\mathbf{x}, t)$ is the electrical conductivity measured in ohm meter $\Omega\cdot\text{m}$. Then, after substitution we get: $$\nabla\cdot(\sigma\nabla\phi)=\nabla\cdot\mathbf{J}_p.$$EEG measures the electric potential at electrode positions $\mathbf{x}_\text{sensors}$ relative to a reference electric potential at an electrode position $A$, i.e., voltages: $$V(\mathbf{x}_\text{sensors}, t)=\phi(\mathbf{x}_\text{sensors}, t) - \phi(A, t)$$![[eeg_recording.png]]