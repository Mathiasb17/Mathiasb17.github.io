# Fluid simulation
## Procedural
## Physics Based
### SPH
#### Kernels
##### Default
###### Formula
Use this kernel for pretty much everything you need. However, for pressure and viscosity forces, prefer the spiky and visc kernels.

Kernel :

$$ W_{poly6}(\vec{x}, h) = \frac{315}{64 \pi h^9} 
\begin{cases} 
  (h^2 - ||x||^2)^2 if ||x|| < h
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
