2025-02-07 15:14

Sources: 

Tags:

The **Cauchy momentum equation** describes how the velocity of a fluid or deformable solid changes over time due to forces acting on it. It is a statement of [[Newton's second law]] applied to continuous material. In Eulerian form, it states: $$\frac{\partial}{\partial t}\mathbf{u} + (\mathbf{u} \cdot\nabla)\mathbf{u}=\frac{1}{\rho}\nabla \cdot \boldsymbol{\sigma} + \mathbf{f}$$ where:
- $t$ is time, measured in seconds, $\text{s}$,
- $\frac{\partial}{\partial t}$ represents the partial derivative operator with respect to time $t$,
- $\mathbf{u}(\mathbf{x},t)$ is the flow velocity vector field, measured in meters per second, $\frac{\text{m}}{\text{s}}$,
- $\mathbf{x}$ represents the position vector in three-dimensional space, typically expressed as $\mathbf{x}=(x,y,z)$, measured in meters, $\text{m}$,
- $\nabla$ is the nabla symbol which denotes the three-dimensional gradient operator,
- $\rho(\mathbf{x}, t)$ is the density at a given point of the continuum, measured in kilograms per meter cubed, $\frac{\text{kg}}{\text{m}^3}$ ,
- $\boldsymbol{\sigma}(\mathbf{x}, t)$ is the stress tensor, measured in pascals, $\text{Pa}$,
-  $\nabla \cdot$ denotes the divergence operator, which when applied to $\boldsymbol{\sigma}$ is: $$\nabla\cdot\boldsymbol{\sigma}=
\begin{bmatrix}
\frac{\partial}{\partial x} \sigma_{xx} + \frac{\partial}{\partial y} \sigma_{yx} + \frac{\partial}{\partial z} \sigma_{zx}  \\ 
\frac{\partial}{\partial x} \sigma_{xy} + \frac{\partial}{\partial y} \sigma_{yy} + \frac{\partial}{\partial z} \sigma_{zy} \\ 
\frac{\partial}{\partial x} \sigma_{xz} + \frac{\partial}{\partial y} \sigma_{yz} + \frac{\partial}{\partial z} \sigma_{zz}
\end{bmatrix},$$ measured in pascals per cubic meter, $\frac{\text{Pa}}{\text{m}^3}$,
- $\mathbf{f}(\mathbf{x}, t)$ is a vector containing all accelerations caused by body forces