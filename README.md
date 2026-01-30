
---

## Topics Covered

### Core Gmsh Concepts
- Geometry creation (Built-in kernel & OpenCASCADE)
- Points, curves, surfaces, volumes
- Physical groups for solver interpretation
- 1st-order vs 2nd-order (quadratic) elements
- Mesh quality metrics (Jacobian, SCIN, Gamma, SIG)

### Meshing Techniques
- Unstructured triangular/tetra meshes
- Structured and **transfinite meshing**
- Quad-dominant and recombined meshes
- Volumetric (3D) meshing
- Shell meshing concepts (solver-side thickness)

### Mesh Control
- Global and local mesh sizing
- **Mesh Fields**:
  - Distance
  - Threshold
  - Box
  - Cylinder
  - MathEval
  - Min / Max field combinations
- Curvature-based mesh refinement
- Background meshes

### Advanced Topics
- Compound surfaces for poor CAD
- STL import and topology restoration
- Periodic meshing for cyclic geometries
- Anisotropic meshes (metric tensors)
- Mesh partitioning for parallel solvers (METIS)
- Homology checks for mesh validity

---

## Impeller-Specific Work

- 2D and 3D meshing of impeller geometry
- Transfinite meshing of blades and edges
- Mesh refinement at hub, base, and blade tips
- Cylindrical and distance-based mesh fields
- Structured meshing of **1/8th impeller sector**
- Periodic meshing for cyclic symmetry
- Practical limitations of mesh transformations in Gmsh
- Comparison with ANSYS ICEM for mesh transformation

---

## Tools Used

- **Gmsh**
- FreeCAD (CAD preparation)
- Elmer / Calculix (solver considerations)
- ANSYS ICEM (mesh transformation comparison)

---

## Key Learnings

- Mesh quality matters more than mesh density
- Transfinite meshing is powerful but limited without topology control
- Mesh fields are essential for impeller meshing
- Periodic meshing is the correct way to handle cyclic geometries in Gmsh
- CAD quality directly affects mesh robustness
- Not all mesh operations belong in Gmsh — knowing tool limits matters

---

## Status

🚧 Ongoing  
This repository will continue to evolve with:
- Cleaner impeller CAD
- Improved structured meshing
- Solver-ready CFD meshes
- Automation scripts

---

## Notes

This repo is **learning-focused**, not a polished product.
Expect experimentation, iteration, and documented failures — because that’s how real engineering work happens.




---

## Key Contributions

- Engineering interpretation of each Gmsh tutorial
- Application of **mesh fields (cylindrical, distance, threshold)** to impeller geometry
- Structured meshing of impeller blades using **transfinite curves and surfaces**
- Evaluation of **periodic meshing vs geometric mesh transformation**
- Identification of practical limitations in Gmsh meshing workflows

---

## Impeller Meshing Example

![Impeller Mesh](images/impeller_mesh.png)

---

## Tools

- Gmsh  
- FreeCAD  
- Elmer / Calculix  
- ANSYS ICEM (comparison)

---

## Status

Ongoing technical study.  
This repository prioritizes **methodology and reproducibility** over polished results.
