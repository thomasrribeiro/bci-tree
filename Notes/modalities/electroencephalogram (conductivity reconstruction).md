2025-02-10 10:47

Sources: 

Tags:

**Electroencephalogram conductivity reconstruction** is a *proposed* [[passive sensing]] technique that measures [[electrophysiological brain activity]] by reconstructing changes in conductivity due to primary current sources from electric potential recordings on the scalp obtained using [[electroencephalogram]].

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

The proposed modality sets $\mathbf{J}_p=0$, simplifying the system of equations $(7)$ and reconstructs for $\sigma(\mathbf{x}, t)$ in a manner similar to [[electroencephalogram (source reconstruction)]]. It is hypothesized that $\sigma(\mathbf{x}, t)$ will vary locally in time according to primary current sources, and that the newly formed problem of scalar field reconstruction will have a smaller solution space compared to the vector field reconstruction of $\mathbf{J}_p(\mathbf{x},t)$, easing the ill-posedeness of the inverse problem. 