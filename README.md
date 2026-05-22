# Engine-Mount-Optimization

![Status](https://img.shields.io/badge/Status-Completed-success)
![CAD](https://img.shields.io/badge/CAD-CATIA_V5-blue)
![CAE](https://img.shields.io/badge/FEA-ANSYS_Workbench-orange)
![Doc](https://img.shields.io/badge/Report-LaTeX-008080)

## 🚀 Overview
This repository showcases the structural engineering, parametric modeling, and Finite Element Analysis (FEA) of an engine mount bracket for a sounding rocket, designed to house the **AeroTech M1939W** solid rocket motor (98 mm diameter).

Rather than just presenting a final part, this project documents an **iterative engineering journey**. The objective was to find the perfect balance between aggressive mass reduction and dynamic structural stability under severe launch loads (6750 N). 

## 🔄 The Design Evolution
The engineering process went through three critical phases, each analyzed using ANSYS Static Structural:

1. **Iteration 1 (Solid Tube & Trusses):** Highly conservative. Great stress distribution, but heavier than necessary.
2. **Iteration 2 (Open Truss Skeleton):** Maximum mass reduction. Visually striking and numerically safe in static analysis, but rejected due to the high risk of lateral buckling and lack of vibrational containment for the motor casing.
3. **The Final Product (Slotted Tube):** The optimal solution. By reintroducing the central tube but cutting longitudinal slits, the design achieved incredible lightness while maintaining the "backbone" required to prevent buckling and secure the motor.

## 📊 Final Product Snapshot
The final iteration proves that intelligent geometric optimization can yield a flight-ready component.

* **Final Mass:** 1.35 kg
* **Max Total Deformation:** 0.063 mm (Extremely rigid)
* **Max von Mises Stress:** 94.31 MPa
* **Factor of Safety (FoS):** ~2.96 (Target was >1.5)

### 🗺️ Deformation & Stress Analysis (Final Iteration)
![Deformation Plot](Media/deformation_support_2.png)
*(Total Deformation plot of the final slotted-tube design, demonstrating near-zero displacement under a 6750 N compressive load).*

## 📂 Repository Structure
* `/CAD_Models`: Native (.CATPart) and universal (.STP) geometry files.
* `/Simulations`: ANSYS Workbench project setups and reports.
* `/Media`: High-resolution FEA plots and videos.
* `/Report`: Full Technical Report compiled in LaTeX.

## 📄 Dive into the Engineering
How did the mesh behave? What were the exact boundary conditions, material properties, and mathematical decisions behind the dynamic load factor? The complete methodology and the detailed breakdown of the three iterations are documented in the academic report.
