# Volumetric Measurements - Stanford Bunny

3D Point Cloud Analysis & Volumetric Measurement Pipeline using the Stanford Bunny dataset.

## Notebooks

### 1. Main Pipeline
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Moooooonk/Volumetric-measurements/blob/master/volumetric.ipynb)

- Point Cloud Loading & 3D Visualization (Plotly)
- Mesh Reconstruction (Convex Hull, Marching Cubes)
- 3D Gaussian Splatting (3DGS)
- Volume Measurement (Divergence Theorem, Signed Tetrahedra, Monte Carlo, Voxelization)
- Comparison & Analysis

### 2. Reference-Based Experiments
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Moooooonk/Volumetric-measurements/blob/master/volumetric_experiments.ipynb)

- Icosphere Resolution vs Volume Accuracy (Level 1-5)
- Green's Theorem 2D Cross-Section Area
- Slice-Based Volume (Smoothing Splines + Green's Equations)
- Truncated Cone Approximation
- Planar Capping for Non-Watertight Meshes
- Mesh Resolution Convergence Study
- Bland-Altman Analysis & Statistical Metrics (TEM, CV, ICC)

## Setup

1. Upload `bunny.tar.gz` to Google Drive (`MyDrive/Volumetric_measurements/`)
2. Click the "Open in Colab" badge above
3. The notebook will automatically mount Drive and extract data

## Methods

| Method | Type | Reference |
|--------|------|-----------|
| Divergence Theorem | Surface Integral (Exact) | Park M.G. |
| Signed Tetrahedra | Geometric (Exact) | - |
| Slice-Based (Green's Eq.) | Cross-Section Integration | Park D.H. (DIMA) |
| Truncated Cone | Frustum Approximation | Park D.H. (DIMA) |
| Monte Carlo | Stochastic | - |
| Voxelization | Discrete | - |
| 3D Gaussian Splatting | Density Field | Kerbl et al. |
