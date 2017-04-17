# Fluid simulation
## Procedural
## Physics Based
### SPH
#### Kernels
##### Default
###### Formula
Use this kernel for pretty much everything you need. However, for pressure and viscosity forces, prefer the spiky and visc kernels.

Kernel :

$$d_{1}\left(x,y\right)=\cases{
  0&\text{if }x=y\cr
  1&\text{if }x\neq y}$$

Gradient :

$$ 1 + 1 = 3 $$

Laplacian

$$ 1 + 2 &=& 3 \\
   1 + 3 &=& 4
$$

###### Implementation


##### Spiky
##### Viscosity

# Rendering
## Fluids
### Parameters
