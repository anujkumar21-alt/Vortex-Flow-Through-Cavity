# CFD Investigation: Shear-Driven Open Cavity Flow (Re = 100 - 3000)

Parametric numerical investigation of 2D laminar shear-driven flow over a recessed rectangular cavity using ANSYS Fluent across Reynolds numbers Re = 100, 200, 400, 600, 800, 1000, and 3000.

## Problem Overview & Geometry
- Domain: Channel flow passing over an open recessed square cavity slot
- Cavity Dimensions: 1 cm width x 1 cm depth (Aspect Ratio W/D = 1.0)
- Solver: ANSYS Fluent (Coupled Scheme, Second-Order Upwind discretization)
- Convergence Target: Scaled residuals < 10^-6

## Parametric Vortex Dynamics & Findings
Tracks the evolution of shear layer penetration, internal recirculation strength, and primary vortex core migration across Reynolds numbers:

- Re = 100:  Cavity geometric center | Weak, diffusion-dominated viscous recirculation
- Re = 200:  Near cavity center      | Stable, well-formed circular primary vortex
- Re = 400:  Shifting downstream     | Growing convective entrainment and circulation
- Re = 600:  Mid-right region        | Transition to inertia-dominated internal rotation
- Re = 800:  Downstream shifted      | High boundary shear and increased core vorticity
- Re = 1000: Lower-right quadrant    | Deep shear layer dip, intensified cavity swirl
- Re = 3000: Compressed on right wall| Strong downstream wall impingement & peak vorticity

### Key Conclusion
As the Reynolds number increases from 100 to 3000, convective momentum transfer across the cavity opening strengthens substantially. Higher inertial forces drive deeper shear layer deflection, continuously increasing the internal circulation velocity and vorticity while displacing the primary vortex core toward the downstream impingement boundary.

## Repository Contents
- Shear_Driven_Cavity_Report.pdf: Full technical report detailing governing physics, parametric regimes, and flow field contour grids.
- Cavity_Open_Shear_Flow.wbpz: Archived ANSYS Workbench project (mesh, boundary conditions, and solved case/data files).
