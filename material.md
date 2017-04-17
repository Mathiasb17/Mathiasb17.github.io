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

$$ W_{poly6}(\vec{x}, h) = \frac{315}{64 \pi h^9} 
\begin{cases} 
  (h^2 - ||x||^2)^2 if ||x|| < h \\
  0 else
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
