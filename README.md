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
- Elmer  (solver considerations)
- ANSYS ICEM (mesh transformation comparison)

---

## Key Learnings

- Mesh quality matters more than mesh density
- Transfinite meshing is powerful but limited without topology control
- Mesh fields are essential for impeller meshing
- Periodic meshing is the correct way to handle cyclic geometries in Gmsh
- CAD quality directly affects mesh robustness

---

## Key Contributions

- Engineering interpretation of each Gmsh tutorial
- Application of **mesh fields (cylindrical, distance, threshold)** to impeller geometry
- Structured meshing of impeller blades using **transfinite curves and surfaces**
- Evaluation of **periodic meshing vs geometric mesh transformation**
- Identification of practical limitations in Gmsh meshing workflows

---

## Impeller Meshing Example

<img width="1600" height="957" alt="image" src="https://github.com/user-attachments/assets/3c25c5cc-664f-4502-b02f-98b51febd6c4" />


---

## Tools

- Gmsh  
- FreeCAD  
- Elmer 
- ANSYS ICEM (comparison)

---

