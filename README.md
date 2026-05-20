[README.md](https://github.com/user-attachments/files/28076481/README.md)
# ParaView-Project# ParaView Work Sample: Pendulum Dynamics Scientific Visualization

## Overview
This work sample demonstrates a complete scientific visualization workflow using **Python + ParaView**.  
The project generates a simulated damped pendulum dataset, exports it in ParaView-readable formats, and visualizes the motion, velocity, and energy behavior of the system.

This sample is designed to show:
- Scientific data generation
- ParaView visualization workflow
- Physics-based reasoning
- Data interpretation
- Technical communication
- Ability to prepare reproducible datasets and documentation

## Project Summary
The pendulum is modeled using numerical time-stepping. For each time step, the dataset records:

- Time
- Position: `x`, `y`, `z`
- Angle in degrees
- Velocity vector: `vx`, `vy`
- Speed
- Potential energy per kg
- Kinetic energy per kg
- Total energy per kg

The included `.vtk` file can be opened directly in ParaView.

## Files
```text
data/
  pendulum_dynamics.csv       Raw table data
  pendulum_trajectory.vtk     ParaView-ready trajectory file

scripts/
  generate_pendulum_dataset.py  Python script used to generate the dataset

paraview/
  paraview_steps.md           Step-by-step ParaView visualization guide

docs/
  project_summary.md          Short writeup for applications
```

## How to Open in ParaView
1. Open ParaView.
2. Click **File → Open**.
3. Select `data/pendulum_trajectory.vtk`.
4. Click **Apply**.
5. Change the coloring from `Solid Color` to `speed`.
6. Use **Tube Filter** to make the trajectory visually thicker.
7. Add **Glyph Filter** and select `velocity` as the vector field to display arrows.
8. Use color mapping to compare speed and total energy along the path.

## What This Demonstrates
This project shows that I can move from a physical model to structured data, then transform that data into an interpretable visualization. The final visualization allows users to observe where the pendulum reaches maximum speed, how energy changes over time, and how damping gradually reduces motion.

## Tools Used
- Python
- CSV
- VTK
- ParaView
- Scientific visualization
- Simulation modeling
