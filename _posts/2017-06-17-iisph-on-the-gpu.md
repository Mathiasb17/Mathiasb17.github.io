---
layout: post
title: "IISPH On the GPU"
comments: true
description: "A cuda parallelized IISPH solver"
keywords: "sph, iisph, CUDA"
---

A few weeks ago i posted about my gpu implementation of an [EOS SPH solver](http://bromat.fr/2017/gpu-sph-fluid-solver/).

I just finished my implementation of an IISPH solver, parallelized with CUDA.

<iframe width="560" height="315" src="https://www.youtube.com/embed/Him-FXRogDk" frameborder="0" allowfullscreen></iframe>

You can find the code [here](https://github.com/Mathiasb17/sph_opengl)

My plan for this git repository is to gather a maximum of particle based fluid simulation methods, and to distribute it
as a free and open source library.

Enjoy !
