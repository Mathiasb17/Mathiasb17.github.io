---
layout: post
title: "GPU SPH Fluid Solver"
comments: true
description: "A CUDA parralelized fluid solver"
keywords: "SPH, CUDA, Fluids, CFD"
---

I'm currently developping a GPU parallelized Smoothed Particle Hydrodynamics (SPH) fluid simulator. I used CUDA to parallelize 
rountines such as neighbors updating, density and internal forces computing.

Also I discretize solid boundaries with spheres and compute adhesion forces on fluid particles.

The overall simulation runs between 1100 and 1200 FPS with ~18k particles on a Nvidia GTX 970 graphic card. (but displays ~800 on the video, the video capture slows down the computations)

<iframe width="560" height="315" src="https://www.youtube.com/embed/_DdHN8qApns" frameborder="0" allowfullscreen></iframe>

You can find the source code [here](https://github.com/Mathiasb17/sph_boundary_particles)

The simulator was written accordingly to the following papers :

* [SPH star](https://cg.informatik.uni-freiburg.de/publications/2014_EG_SPH_STAR.pdf)
* [Boundaries paper](https://cg.informatik.uni-freiburg.de/publications/2013_CASA_elasticSolids.pdf)

I plan to add the following features :

* Implicit Incompressible SPH (currently i'm using an equation of state, and that sucks)
* Two way coupling
* Better surface tension models
* Breaking waves
* Real-time surface reconstruction using GVDB
* Maybe real-time rendering using nvidia optics !?
