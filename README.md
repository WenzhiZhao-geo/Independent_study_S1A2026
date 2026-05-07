# Independent_study_S1A2026

This repository contains the code and numerical experiments developed as part of the course **Independent_study_S1A2026**. The notebooks document the learning outcomes of the course and focus on solving time dependent partial differential equations using different numerical methods.

## Overview

The project investigates numerical solutions for heat diffusion and wave propagation problems. The main objective is to compare several computational approaches, including finite difference methods, finite element methods, implicit and explicit time integration schemes, Crank–Nicolson schemes, and pseudospectral methods.

## Contents

The work is organized into four Jupyter Notebook exercises:

### 1. Exercise 1A — Transient Heat Diffusion Toward a Curved Geothermal Profile

This notebook solves a one dimensional transient heat diffusion problem in a crustal column with radiogenic heat production. The temperature field evolves from an initial condition toward a curved steady state geothermal profile.

The problem includes fixed temperature boundary conditions at the top and bottom of the domain. Different numerical methods are implemented and compared to evaluate accuracy, stability, and convergence behavior.

### 2. Exercise 1B — Half Space Gaussian Shear Heating Diffusion

This notebook studies one dimensional heat diffusion in a half space with Gaussian shear heating concentrated near a symmetry plane. The model represents localized heat production caused by shear deformation.

A logarithmically refined grid is used near the shear zone to better resolve the strong temperature gradients. The numerical results are compared across several methods, including explicit, implicit, Crank–Nicolson, FEM-based, and pseudospectral approaches.

### 3. Exercise 2A — One Dimensional Acoustic Source–Receiver Exercise

This notebook solves a one dimensional homogeneous acoustic wave propagation problem. A localized source generates waves that are recorded at a receiver location.

The computed receiver trace is benchmarked against a Green function reference solution. The exercise focuses on the numerical behavior of wave propagation schemes, including accuracy, dispersion, and stability.

### 4. Exercise 2B — Two Dimensional SH Wave Source–Receiver Exercise

This notebook extends the wave propagation problem to two dimensions. It solves a homogeneous SH wave equation on a rectangular grid with a localized source and receiver.

The receiver trace is compared with a two dimensional Green function reference. This exercise demonstrates how numerical methods perform in higher dimensional wave simulations and highlights computational cost, spatial resolution, and error behavior.

## Numerical Methods Used

The notebooks include implementations of:

- Explicit finite difference methods
- Implicit finite difference methods
- Crank–Nicolson schemes
- Finite element methods with consistent and lumped mass matrices
- Backward/implicit FEM schemes
- Pseudospectral cosine or sine transform methods
- Error and residual analysis using L2 error and final residual comparisons

## Purpose

The purpose of this repository is to document the learning process and computational results from **Independent_study_S1A2026**. The exercises show how different numerical discretization and time-stepping methods can be applied to physical problems involving thermal diffusion and acoustic or elastic wave propagation.

Through these notebooks, the project compares numerical accuracy, stability constraints, computational efficiency, and agreement with analytical or reference solutions.

## Files

```text
01_Exercise1A.ipynb   Transient heat diffusion toward a curved geothermal profile
02_Exercise1B.ipynb   Half space Gaussian shear heating diffusion
03_Exercise2A.ipynb   1D acoustic wave source–receiver exercise
04_Exercise2B.ipynb   2D SH wave source–receiver exercise

## Dependencies

This project uses Python and several standard scientific computing packages. The required packages are listed in `requirements.txt`.

Main dependencies:

```text
python 3.11 or later
numpy
pandas
scipy
matplotlib
jupyterlab
notebook
ipykernel
pillow
