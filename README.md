# Switched Reluctance Motor (SRM) Flux Surface Visualization

This repository provides a Python script to visualize the magnetic flux surface of a switched reluctance motor (SRM) based on rotor angle (in radians) and current (in amperes). The flux data is loaded from a MATLAB `.mat` file, and the surface is interpolated and plotted in 3D using `matplotlib`.

## Features
- Loads flux data (`Psi`), rotor angle (`teta`), and current (`I`) from a MATLAB `.mat` file.
- Converts rotor angle from degrees to radians for visualization, scaled from 0 to \(2\pi\).
- Interpolates and plots the flux surface as a function of rotor angle and current.
- Automatically handles cases where current is 0 by setting corresponding flux values to 0.
- Provides a 3D plot of the interpolated surface using a viridis colormap.

## Requirements
- Python 3.x
- Required packages:
  - `numpy`
  - `scipy`
  - `matplotlib`

You can install the dependencies using `pip`:
```bash
pip install numpy scipy matplotlib
