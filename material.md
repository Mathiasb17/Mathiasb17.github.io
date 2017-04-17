# Fluid simulation
## Procedural
## Physics Based
### SPH
#### Kernels
##### Default
###### Formula
Use this kernel for pretty much everything you need. However, for pressure and viscosity forces, prefer the spiky and visc kernels.

Kernel :

$$
  f(n) =
\begin{cases}
n/2,  & \text{if $n$ is even} \\
3n+1, & \text{if $n$ is odd}
\end{cases}
$$

Gradient :

Laplacian

###### Implementation


##### Spiky
##### Viscosity

# Rendering
## Fluids
### Parameters
