---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
redirect_from: 
  - /projects
---

[`SeriesAcceleration.jl`](https://github.com/Atomtomat/SeriesAcceleration.jl): Functonality for improved sum calculations, i.e. obtaining a closer approximation of the limit of an infinte series, than through plain summation.


[`EquivalenceClassesConstructor.jl`](https://github.com/Atomtomate/EquivalenceClassesConstructor.jl): Construction of a minimal set of representatives from a given set, under a number of equivalence relations. A mapping back to the original set is also computed. This can, for example, be used 


[`Dispersions.jl`](https://github.com/Atomtomate/Dispersions.jl): This is a small utility code that helps with the computation of quantities on Bravais lattices. Notable is the functionality to calculate on a reduced lattice, with representatives generated from `EquivalenceClassesConstructor.jl`. One important group of functions exported are convolutions and autocorrelations, which are computed using Fast Fourier Transforms (FFTs).


[`jED.jl`](https://github.com/Atomtomate/jED.jl): This Julia code can calculate the exact solution of a lattice model (currently implemented: Anderson Impurity Model, Hubbard Model) by finding all eigenvalues in a basis for the corresponding Hilbert space. While sufficiently fast to be usable in production, the main purpose of this code is to by eadily accasible for students. Therefore clarity of the code has been 


[`LadderDGA.jl`](https://github.com/Atomtomate/LadderDGA): This Julia code calculates an improved solution (in terms of Green's functions) for the Hubbard model on arbitrary (implemented in another project `Dispersions.jl`) lattice, starting from a Dynamical Mean Field (DMFT) input.
The DMFT solution can, for example, be calculated using `jED.jl` or my [CTQMC code](https://github.com/Atomtomate/DMFT). Subsequently, a two-particle Green's function needs to be computed (The DMFT solution and the two-particle Green's function can, for example, obtained from [`pomerol`](https://github.com/pomerol-ed/pomerol)).
The input for `LadderDGA.jl` is then prepared by [`VertexPostprocessing.jl`](https://github.com/Atomtomate/VertexPostprocessing.jl), which can also take symmetry considerations from `EquivalenceClassesConstructor.jl` into account.


[`MFDecoupling.jl`](https://github.com/Atomtomate/MFDecoupling.jl): A co-authored wrapper around a differential equation solver package, that computes the time evolution on an Anderson Impurity Chain.


[`LuttingerWard_from_ML`](https://github.com/Atomtomate/LuttingerWard_from_ML): This is a co-authored project which aims to explore the feasibility of training neural networks to learn details about the Luttinger Ward functional. Using `jED.jl`, pairs of Green's functions and self-energies are generated and given as training/test data to different network architectures. 


[`PyTorchTutorial`](https://github.com/Atomtomate/PyTorchTutorial): Small tutorial with examples and explanations for the basics of machine learning and PyTorch.