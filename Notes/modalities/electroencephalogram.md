2025-02-07 18:03

Sources: 

Tags:

**Electroencephalogram (EEG)** is a [[passive sensing]] technique that measures [[electrophysiological brain activity]] by recording differences in electric potentials, i.e., voltages, on the scalp.

![[eeg_setup.png|300]]

# Theory

From the [[quasi-static approximations of Maxwell's equations]], we obtain the system of equations: $$\begin{align}
\nabla\cdot(\sigma\nabla\phi)&=\nabla\cdot\mathbf{J}_p \\
\sigma\nabla\phi &= \frac{1}{\mu_0}(\nabla\times\mathbf{B}) - \mathbf{J}_p 
\end{align}\tag{7}$$where:
- $\sigma(\mathbf{x}, t)$ is the electrical conductivity, measured in siemens per meter $\frac{\text{S}}{\text{m}}$, 
- $\phi(\mathbf{x},t)$ is the electric potential, measured in volts $\text{V}$, 
- $\mathbf{J}_p(\mathbf{x},t)$ is the primary current density due to neuronal activity, measured in amperes per squared meter $\frac{\text{A}}{\text{m}^2}$,
- $\mu_0$ is the permeability of free space, measured in henry per meter $\frac{\text{H}}{\text{m}}$, 
- $\mathbf{B}(\mathbf{x},t)$ is the magnetic field, measured in tesla $\text{T}$. 

EEG measures the electric potential $\phi$ at electrode positions $\mathbf{x}_\text{sensors}$ relative to a reference electric potential at an electrode position $A$, i.e., voltages: $$V(\mathbf{x}_\text{sensors}, t)=\phi(\mathbf{x}_\text{sensors}, t) - \phi(A, t)$$![[eeg_recording.png]]