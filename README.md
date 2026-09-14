# Turbulent Airfoil Flow Simulation | ANSYS Fluent

## Overview

A 2D CFD study of turbulent flow over a NACA 0012 airfoil using ANSYS Fluent.
The simulation investigates the aerodynamic behavior of the airfoil at an angle
of attack of 10° and evaluates its performance through surface pressure,
lift, and drag characteristics.

The project is based on a canonical turbulent airfoil-flow problem from
Cornell University's engineering simulation coursework, with emphasis on
CFD setup, turbulence modeling, post-processing, and validation against
experimental data.

## Problem Definition

The flow around a NACA 0012 airfoil is simulated at an angle of attack of 10°.
The resulting flow field and aerodynamic quantities are analyzed and compared
with experimental data.

### Operating Conditions

| Parameter | Value |
|---|---:|
| Airfoil | NACA 0012 |
| Chord length | 1 m |
| Angle of attack | 10° |
| Free-stream velocity | 51.45 m/s |
| Density | 1.1767 kg/m³ |
| Reynolds number | 6 × 10⁶ |

## Objectives

- Set up a 2D turbulent external-flow simulation in ANSYS Fluent.
- Analyze the velocity and pressure fields around the airfoil.
- Obtain the surface pressure coefficient distribution.
- Determine the lift and drag coefficients.
- Compare the numerical results with experimental data provided by NASA.

## CFD Methodology

The simulation follows a standard external-aerodynamics CFD workflow:

1. NACA 0012 geometry preparation
2. Computational-domain and mesh generation
3. Definition of fluid properties and boundary conditions
4. Turbulence-model selection
5. Numerical solution of the governing equations using ANSYS Fluent
6. Convergence monitoring
7. Post-processing of the flow field and aerodynamic quantities
8. Comparison with experimental data

### Solver Setup

| Setting | Description |
|---|---|
| Solver | ANSYS Fluent |
| Dimension | 2D |
| Flow | Turbulent |
| Analysis | Steady-state |
| Turbulence model | To be added |
| Pressure-velocity coupling | To be added |
| Discretization schemes | To be added |

## Computational Mesh

The computational domain was discretized with increased mesh resolution
around the airfoil to capture the flow gradients and near-wall behavior.

### Mesh Overview

![Computational Mesh](mesh/mesh_overview.png)

### Near-Airfoil Mesh

![Near-Airfoil Mesh](mesh/mesh_near_airfoil.png)

## Boundary Conditions

The computational domain was configured to represent the specified
free-stream conditions around the airfoil.

| Boundary | Condition |
|---|---|
| Inlet | To be added |
| Outlet | To be added |
| Airfoil surface | No-slip wall |
| Far-field / other boundaries | To be added |

## Results

### Velocity Distribution

The velocity field around the NACA 0012 airfoil is examined to identify
flow acceleration, deceleration, and the development of the wake.

![Velocity Contour](results/velocity_contour.png)

### Pressure Distribution

The pressure field illustrates the pressure variation around the airfoil
resulting from the external flow.

![Pressure Contour](results/pressure_contour.png)

### Surface Pressure Coefficient

The surface pressure coefficient distribution is extracted along the
airfoil surface and compared with experimental measurements.

![Pressure Coefficient Distribution](results/cp_distribution.png)

## Aerodynamic Performance

The aerodynamic performance of the airfoil is evaluated using the lift
and drag coefficients obtained from the CFD solution.

| Quantity | CFD | Experimental |
|---|---:|---:|
| Lift coefficient, $C_L$ | To be added | To be added |
| Drag coefficient, $C_D$ | To be added | To be added |

## Validation

The numerical solution is compared with experimental data provided by NASA.

The validation focuses on:

- Surface pressure coefficient distribution
- Lift coefficient
- Drag coefficient

### CFD vs Experimental Pressure Distribution

![Pressure Coefficient Validation](validation/cp_validation.png)

### Lift and Drag Comparison

![Aerodynamic Coefficient Comparison](validation/coefficient_comparison.png)

## Key Observations

- The pressure and velocity fields around the NACA 0012 airfoil were
  obtained from the CFD solution.
- The surface pressure distribution was evaluated to characterize the
  aerodynamic loading.
- Lift and drag coefficients were extracted from the numerical solution.
- CFD predictions were compared with experimental data to assess the
  accuracy of the simulation.

## Skills Demonstrated

- Computational Fluid Dynamics (CFD)
- ANSYS Fluent
- External Aerodynamics
- Turbulence Modeling
- Mesh Generation
- Boundary Condition Setup
- CFD Post-processing
- Aerodynamic Force Analysis
- Numerical Validation

## Software

- ANSYS Fluent
- ANSYS Meshing

## Reference

Cornell University, ENGR2000X — A Hands-on Introduction to Engineering
Simulations, Module 5: Turbulence.

Experimental data used for validation: NASA experimental data for the
NACA 0012 airfoil.
