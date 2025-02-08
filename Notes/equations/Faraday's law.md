2025-02-07 14:24

Sources: 

Tags:

**Faraday's law** states that a changing magnetic field over time induces an electric field. Formally:
$$\nabla \times \mathbf{E} = -\frac{\partial}{\partial t} \mathbf{B}$$
where:
- $\mathbf{E}(\mathbf{x},t)$ is the electric field, measured in volts per meter $\frac{\text{V}}{\text{m}}$,
- $\mathbf{x}$ represents the position vector in three-dimensional space, typically expressed as $\mathbf{x}=(x,y,z)$, measured in meters $\text{m}$,
- $t$ is time, measured in seconds $\text{s}$,
- $\nabla$ is the nabla symbol which denotes the three-dimensional gradient operator,
- $\nabla \times$ denotes the curl operator, which measures the rotation of a field in space, and which when applied to $\mathbf{E}$ is: $$\nabla \times \mathbf{E}=\left(\frac{\partial}{\partial y}E_z - \frac{\partial}{\partial z}E_y\right)\mathbf{i} + \left(\frac{\partial}{\partial z}E_x - \frac{\partial}{\partial x}E_z\right)\mathbf{j} + \left(\frac{\partial}{\partial x}E_y - \frac{\partial}{\partial y}E_x\right)\mathbf{k},$$ measured in volts per meter squared $\frac{\text{V}}{\text{m}^2}$,
- $\frac{\partial}{\partial t}$ denotes the partial derivative operator with respect to time $t$,
- $\mathbf{B}(\mathbf{x},t)$ is the magnetic field (or magnetic flux density), measured in tesla $\text{T} = \frac{\text{Wb}}{\text{m}^2} = \frac{\text{N}}{\text{A}\cdot\text{m}}$. 

Alternatively, in integral form: $$\oint_C \mathbf{E} \cdot d\mathbf{s} = -\frac{d}{dt}\int_S \mathbf{B}\cdot d\mathbf{A}$$ where:
- $C$ represents a closed loop or contour in space,
- $\oint_C$ represents a line integral around the closed path $C$, measuring the total circulation of the electric field along the loop,
- $d\mathbf{s}$ is a differential line element that represents an infinitesimally small segment along the loop $C$,
- $\frac{d}{dt}$ represents the time derivative operator, indicating how a quantity changes over time,
- $S$ is a surface whose boundary is the closed loop $C$,
- $\int_S$ represents a surface integral, which sums the contribution of the field $\mathbf{B}$ over the entire surface $S$, 
- $d\mathbf{A}$ is a differential surface element, representing an infinitesimally small patch of the surface $S$.