2025-02-07 13:35

Sources: 

Tags:

**Gauss' law** (electrostatics) states that the electric flux through a closed surface is proportional to the total charge enclosed within that surface. Formally:
$$\nabla \cdot \mathbf{E} = \frac{\rho}{\varepsilon_0}$$
where:
- $\mathbf{E}(\mathbf{x},t)$ is the electric field, measured in volts per meter $\frac{\text{V}}{\text{m}}$, 
- $\mathbf{x}$ represents the position vector in three-dimensional space, typically expressed as $\mathbf{x}=(x,y,z)$, measured in meters $\text{m}$,
- $t$ is time, measured in seconds $\text{s}$,
- $\nabla$ is the nabla symbol that denotes the three-dimensional gradient operator,
- $\nabla \cdot$ denotes the divergence operator, which measures the net flux of a field out of an infinitesimal volume, and which when applied to $\mathbf{E}$ is: $$\nabla\cdot\mathbf{E}=\frac{\partial}{\partial x}E_x + \frac{\partial}{\partial y}E_y + \frac{\partial}{\partial z}E_z,$$ measured in volts per meter squared $\frac{\text{V}}{\text{m}^2}$,
- $\rho(\mathbf{x}, t)$ is the charge density, measured in coulombs per cubic meter $\frac{\text{C}}{\text{m}^3}$,
- $\varepsilon_0$ is the permittivity of free space, measured in farads per meter $(8.85 \times 10^{-12}\frac{\text{F}}{\text{m}})$.

Alternatively, in integral form: $$\oint_S \mathbf{E} \cdot d\mathbf{A} = \frac{Q_\text{enc}}{\varepsilon_0}$$ where:
- $S$ represents a closed surface,
- $\oint_S$ represents a surface integral, 
- $d\mathbf{A}$ is a differential surface element that represents an infinitesimally small patch of the surface $S$,
- $Q_\text{env}$ is the total charge enclosed by the Gaussian surface, measured in coulombs, $\text{C}$.