# Aerodynamics of Transport Vehicles - Politecnico di Milano

This repository contains the CFD analysis project for the "Aerodynamics of Transport Vehicles" course at Politecnico di Milano. The study investigates the aerodynamic impact of different rear wing attachment configurations on a Tesla Model S.

**Team:** Co-developed by Alberto Rivero, Alejandro Rivera, Mikel Segovia, and Francisco Javier Martín.

### Project Overview & Methodology

* **3D Modeling & CAD:** Modified a Tesla Model S geometry using CATIA® to integrate a custom rear wing combining NACA 4412 and Selig 1223 airfoils with endplates.
* **Mesh Generation:** Generated high-quality hybrid meshes using OpenFOAM's `blockMesh` and `snappyHexMesh` utilities. Conducted a rigorous mesh independence study and evaluated boundary layer resolution ($y^+$ assessment) to balance numerical accuracy and computational cost.
* **CFD Simulation Setup:** Performed incompressible RANS simulations using the OpenFOAM® `SimpleFoam` solver. The $k-\omega$ SST turbulence model was selected to accurately capture boundary layer physics and far-field robustness.
* **Configurations Analyzed:** Evaluated a baseline model against three distinct spoiler mounting strategies: "Below" (suction surface), "Back" (pressure surface, behind trailing edge), and "Front" (pressure surface, ahead of leading edge).
* **Post-processing & Visualization:** Utilized ParaView for advanced flow field visualization. Analyzed mean pressure coefficients ($C_p$) on the wing and car body, evaluated wake formations, and identified complex 3D vortex structures using the Q-criterion.
* **Aerodynamic Performance:** Compared downforce ($C_L$), drag ($C_D$), and aerodynamic efficiency across all setups. The findings successfully correlated aerodynamic forces with theoretical vehicle dynamics, such as cornering velocity limits.
