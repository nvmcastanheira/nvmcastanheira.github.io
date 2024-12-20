---
title: "Numerical Libraries"
permalink: /numerical-libraries/
layout: single
---

Below I display ready-to-use software for a variety of solvers/numerical-methods. Most of these are NOT optimized, and are simply ready to deploy with documentation. 

## Nth-derivative Calculations Using Cauchy's Integral Formula (CauchDev)

Nth-order numerical differentiation (without automatic  methods) has issues with numerical stability when attempted with typical finite-different schemes. There are methods to contravene this (e.g: taking a first-order derivative a multitude of times on the input array), but this requires a very granular input. A nice alternative is provided in CauchDev: a contour integral is taken about a circle centered at each point in the array. This directly calculates the numerical derivative by Cauchy's integral formula (citation needed). 

The only required assumption is a continuous underlying function (which is true of the convolution of real-valued functions (citation needed)). [CauchDev]{google.com} provides an implementation of the above in Python. 
