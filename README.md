# ✈️ Transonic Aerodynamic Wing Design Project

**Course**: MSc Aerospace Dynamics, Cranfield University  
**Supervisors**: Dr Simon Prince and Dr Davide Di Pasquale
**Tools Used**: VGK, VGK_2D, VFP, XFOIL  

---

## 📖 Overview

This project focuses on the **design, optimisation, and analysis** of a **transonic wing** for a long-haul commercial airliner. Using computational tools such as VGK, VGK_2D, and VFP, the study aimed to improve aerodynamic efficiency, reduce wave drag, and ensure safety margins under cruise conditions.

---

## 🏆 Key Objectives

1. **Airfoil Design**:
   - Create airfoil profiles for the root, crank, and tip sections of the wing.
   - Optimise profiles for minimum drag and sufficient lift at transonic conditions.
2. **Wing Design**:
   - Integrate airfoil sections into a finite wing geometry.
   - Analyse the effect of twist, sweep, and dihedral on performance.
3. **Performance Analysis**:
   - Evaluate cruise performance using VGK_2D and VFP solvers.
   - Compare spanwise load distributions with ideal elliptical lift.

---

## 🔍 Test Cases

| **Test Case**           | **Description**                                                                 | **Key Parameters**                |
|-------------------------|---------------------------------------------------------------------------------|-----------------------------------|
| **Root Airfoil Design** | Optimise for front-loading with no shock design for cruise conditions.          | `CL = 0.4266`, `t/c = 15%`        |
| **Crank Airfoil Design**| Design a supercritical airfoil for max lift at 30% semispan.                    | `CL = 0.7023`, `t/c = 12.65%`     |
| **Tip Airfoil Design**  | Optimize for rear-loading with weak shock to reduce tip loading.                | `CL = 0.5893`, `t/c = 7%`         |
| **Wing Analysis**       | Analyze overall wing performance at cruise Mach (M = 0.8).                     | `CL = 0.4971`, `CD = 0.0157`      |

---

## 📊 Key Results

### Root Airfoil (VGK_2D)
- **Design**: No-shock airfoil with maximum thickness at 15% chord.  
- **Performance**: Low drag, suitable buffet margin for cruise.  
- **Coefficients**:  
  - Lift Coefficient (`CL`): 0.4266  
  - Korn Factor (`Kn`): 0.88  

### Crank Airfoil (VGK_2D)
- **Design**: Supercritical airfoil with rear loading for higher lift.  
- **Performance**: High lift and acceptable wave drag.  
- **Coefficients**:  
  - Lift Coefficient (`CL`): 0.7023  
  - Korn Factor (`Kn`): 0.876  

### Tip Airfoil (VGK_2D)
- **Design**: Thin supercritical airfoil with weak shocks for structural integrity.  
- **Performance**: Acceptable lift with reduced tip loading.  
- **Coefficients**:  
  - Lift Coefficient (`CL`): 0.5893  
  - Korn Factor (`Kn`): 0.87  

### Overall Wing (VFP)
- **Design**: Final geometry integrates root, crank, and tip sections with twist and sweep for transonic performance.  
- **Performance**: High aerodynamic efficiency and near-elliptical lift distribution.  
- **Coefficients**:  
  - Lift-to-Drag Ratio (`L/D`): 31.73  
  - Moment Coefficient (`CM`): -0.746  

---

## 🛠️ Tools and Technologies

| **Tool**        | **Purpose**                                         |
|------------------|-----------------------------------------------------|
| **VGK**         | Inverse design of airfoil profiles.                 |
| **VGK_2D**      | Analysis of aerodynamic coefficients for airfoils.  |
| **VFP**         | Design and analysis of finite wing geometries.      |
| **XFOIL**       | Airfoil thickness modification.                     |

---

## 📌 Key Contributions

1. **Airfoil Optimisation**: Successfully designed and analysed airfoils for the root, crank, and tip sections, ensuring performance and structural integrity.  
2. **Wing Geometry**: Created a final wing design integrating airfoil sections with optimal twist, sweep, and dihedral angles for cruise efficiency.  
3. **Performance Validation**: Validated aerodynamic characteristics through computational tools, achieving a near-elliptical lift distribution and high aerodynamic efficiency.  

---

## 📈 Data Summary

| **Variable**    | **Value**               | **SI Unit** |
|------------------|-------------------------|-------------|
| Cruise Mach      | 0.8                     | -           |
| Altitude         | 38,000                  | ft          |
| Root CL          | 0.4266                  | -           |
| Crank CL         | 0.7023                  | -           |
| Tip CL           | 0.5893                  | -           |
| Wing L/D         | 31.73                   | -           |

---

## 🔍 Visualizations

1. **Wing Geometry**  
   ![Wing Geometry](./images/wing-geometry.png)

2. **Pressure Coefficients**  
   ![Pressure Distribution](./images/pressure-distribution.png)

3. **Spanwise Loading**  
   ![Spanwise Load](./images/spanwise-load.png)

---

## 📫 Contact

For further information, feel free to reach out:  
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/namitarajendrapatil)  
[![Email](https://img.shields.io/badge/-Gmail-red?style=flat&logo=gmail)](mailto:namitapatil1995@gmail.com)  

---

*This project was completed as part of the MSc Aerospace Dynamics course at Cranfield University.*
