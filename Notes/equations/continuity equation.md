2025-02-07 16:06

Sources: 

Tags:

The **continuity equation** is a mathematical expression of mass conservation, stating that the rate of change of mass in a given region is equal to the net mass flux entering or leaving that region. Formally: $$\frac{\partial}{\partial t}\rho + \nabla \cdot(\rho \mathbf{u})=s$$ where:
- $t$ is time, measured in seconds $\text{s}$,
- $\frac{\partial}{\partial t}$ represents the partial derivative operator with respect to time $t$,
- $\rho(\mathbf{x}, t)$ is the density at a given point of the continuum, measured in kilograms per meter cubed $\frac{\text{kg}}{\text{m}^3}$,
- $\mathbf{x}$ represents the position vector in three-dimensional space, typically expressed as $\mathbf{x}=(x,y,z)$, measured in meters $\text{m}$,
- $\mathbf{u}(\mathbf{x},t)$ is a vector field, measured in meters per second $\frac{\text{m}}{\text{s}}$, describing the movement of some quantity $q$,
- $s(\mathbf{x},t)$ is the generation of the quantity $q$ described by $\mathbf{u}(\mathbf{x},t)$ per unit volume per unit time; with terms that generate $q$ (i.e. $\sigma>0$) or remove $q$ (i.e. $\sigma <0$) being referred to as sources and sinks, respectively,
- $\nabla$ is the nabla symbol which denotes the three-dimensional gradient operator,
-  $\nabla \cdot$ denotes the divergence operator, which when applied to $\rho\mathbf{u}$ is: $$\nabla\cdot(\rho\mathbf{u})=\frac{\partial}{\partial x}(\rho u_x) + \frac{\partial}{\partial y}(\rho u_y) + \frac{\partial}{\partial z}(\rho u_z),$$ measured in kilograms per cubic meter per second $\frac{\text{kg}}{\text{m}^3 \cdot \text{s}}$.