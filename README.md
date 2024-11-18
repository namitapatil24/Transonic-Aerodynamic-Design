# Transonic Aerodynamic Wing Design Project

**Course**: MSc Aerospace Dynamics, Cranfield University  
**Supervisors**: Dr Simon Prince and Dr Davide Di Pasquale  
**Tools Used**: VGK, VGK_2D, VFP, XFOIL  

---

## 📖 Overview


This project applies advanced low fidelity computational techniques (VGK, VGK_2D, and VFP) to design, optimize, and analyze a transonic wing planform composed of root, crank, and tip airfoils. The study aims to maximize aerodynamic performance, reduce drag, and ensure safe operational margins.

The design of transonic wings for long-haul commercial airliners is critical to balancing aerodynamic efficiency and operational safety. Transonic flow regimes present unique challenges due to the formation of shock waves on the airfoil surfaces, which can lead to **wave drag**, **flow separation**, and **buffet onset**. 

To address these challenges, supercritical airfoils are employed to delay drag divergence and maintain favorable lift-to-drag ratios. These airfoils feature:
- **Flattened upper surfaces** to minimize shock strength.
- **Aft cambering** to enhance rear loading for lift production.
- **Optimized leading-edge radii** to manage flow acceleration and curvature.


---

## 🏆 Key Objectives

1. **Airfoil Design**:
   - Develop optimized profiles for root, crank, and tip sections.
   - Minimize drag while maintaining sufficient lift.
2. **Wing Design**:
   - Integrate airfoils into a finite wing geometry.
   - Optimize spanwise lift distribution using twist, sweep, and dihedral.
3. **Performance Evaluation**:
   - Analyze aerodynamic efficiency and validate against design criteria.

---
## 🔍 Methodology

1. **Airfoil Design**:  
   - Used **VGK** to create root, crank, and tip airfoils optimized for transonic flow conditions.  
   - Performed iterative refinements with **XFOIL** to adjust thickness, camber, and leading-edge radii for wave drag reduction.  

2. **Mesh Generation**:  
   - Developed structured grids for airfoil sections using VGK_2D, ensuring adequate resolution near shock regions.  
   - Validated mesh quality through sensitivity analysis to ensure accurate predictions.  

3. **Finite Wing Analysis**:  
   - Integrated airfoil sections into a 3D wing planform using **VFP** with optimized sweep, twist, and dihedral angles.  
   - Simulated wing performance at transonic cruise conditions (`M = 0.8`) to assess aerodynamic coefficients and spanwise load distributions.  

4. **Post-Processing**:  
   - Analyzed Cp distributions, spanwise load variations, and drag breakdown to evaluate aerodynamic efficiency.  
   - Compared results with ideal lift distribution and documented findings in the final report.  
 


---



## 📊 Data Summary and Explanation

| **Variable**    | **Value**               | **SI Unit** | **Explanation**                                                                 |
|------------------|-------------------------|-------------|---------------------------------------------------------------------------------|
| **Cruise Mach**  | 0.8                     | -           | Transonic cruise condition; freestream Mach number.                             |
| **Altitude**     | 38,000                  | ft          | Typical cruising altitude for long-haul flights.                                |
| **Root CL**      | 0.4266                  | -           | Lift coefficient of root airfoil; designed for structural support and efficiency.|
| **Crank CL**     | 0.7023                  | -           | Maximum lift coefficient at 30% span; provides majority of lift.                |
| **Tip CL**       | 0.5893                  | -           | Reduced lift at the tip to minimize induced drag and structural stress.          |
| **Wing L/D**     | 31.73                   | -           | High aerodynamic efficiency for cruise.                                         |

### Observations:
1. **Root Airfoil**: Designed with no rear loading to avoid high drag moments and minimize structural stresses. It ensures stability and trim requirements.
2. **Crank Airfoil**: Positioned for maximum lift generation. Rear loading enhances lift production while maintaining acceptable drag divergence margins.
3. **Tip Airfoil**: Thin and rear-loaded to reduce tip loading and avoid tip stall, crucial for preserving aileron authority during flight.
4. **Wing Performance**: The near-elliptical lift distribution minimizes induced drag, achieving an impressive lift-to-drag ratio of 31.73.

---

## 🔍 Key Findings and Observations

1. **Aerodynamic Challenges in Transonic Flow**:
   - Shock formation on the upper surface leads to **wave drag** and flow separation. By delaying drag divergence using supercritical designs, these effects are mitigated.
   - Buffet onset is managed by maintaining a sufficient **buffet margin** (~0.05 Mach).

2. **Airfoil Design Optimization**:
   - The **Root Airfoil** avoids strong shocks, promoting smooth flow for structural reliability.
   - The **Crank Airfoil** achieves maximum lift while controlling wave drag with a supercritical shape.
   - The **Tip Airfoil** minimizes loading to ensure structural integrity and operational safety.

3. **Wing Design Integration**:
   - Incorporating twist, sweep, and dihedral enhances aerodynamic efficiency and stability.
   - The twist schedule (Root: +2°, Crank: +1°, Tip: -2°) ensures ideal spanwise lift distribution and prevents tip stall.

4. **Performance Validation**:
   - The **Lift-to-Drag Ratio (L/D)** of 31.73 demonstrates excellent efficiency.
   - The **Spanwise Load Distribution** closely matches the ideal elliptical profile, minimizing induced drag.

---

## 🧪 Test Cases

| **Test Case**           | **Description**                                                                 | **Key Parameters**                |
|-------------------------|---------------------------------------------------------------------------------|-----------------------------------|
| **Root Airfoil Design** | Optimize for front-loading with no shock design for cruise conditions.          | `CL = 0.4266`, `t/c = 15%`        |
| **Crank Airfoil Design**| Design a supercritical airfoil for max lift at 30% semispan.                    | `CL = 0.7023`, `t/c = 12.65%`     |
| **Tip Airfoil Design**  | Optimize for rear-loading with weak shock to reduce tip loading.                | `CL = 0.5893`, `t/c = 7%`         |
| **Wing Analysis**       | Analyze overall wing performance at cruise Mach (M = 0.8).                     | `CL = 0.4971`, `CD = 0.0157`      |

---

## ⚡ Key Contributions

1. **Airfoil Design and Optimization**:
   - Designed and analyzed airfoil profiles tailored for specific wing sections.
   - Addressed transonic challenges using supercritical airfoil principles.
2. **Finite Wing Integration**:
   - Integrated optimized airfoils into a wing planform with a 35° sweep.
   - Incorporated twist and dihedral for enhanced aerodynamic performance.
3. **Performance Validation**:
   - Achieved near-elliptical spanwise lift distribution, reducing induced drag.
   - Validated high aerodynamic efficiency and safe operational margins.

---

## 🔍 Visualizations

1. **Wing Geometry**  
   ![Wing Geometry](./images/wing-geometry.png)

2. **Pressure Coefficients**  
   ![Pressure Distribution](./images/pressure-distribution.png)

3. **Spanwise Loading**  
   ![Spanwise Load](./images/spanwise-load.png)

---

## 🛠️ Tools and Technologies

| **Tool**        | **Purpose**                                         |
|------------------|-----------------------------------------------------|
| **VGK**         | Inverse design of airfoil profiles.                 |
| **VGK_2D**      | Analysis of aerodynamic coefficients for airfoils.  |
| **VFP**         | Design and analysis of finite wing geometries.      |
| **XFOIL**       | Airfoil thickness modification.                     |

---
## 🚀 Future Scope

1. **Advanced Turbulence Modeling**:
   - Implement high-fidelity turbulence models (e.g., LES or DDES) to capture flow unsteadiness and shock-boundary layer interactions more accurately.

2. **Transient Simulations**:
   - Conduct unsteady simulations to analyze buffet onset and dynamic loading conditions during cruise and off-design operations.

3. **Structural Analysis**:
   - Extend the study to include aeroelastic and structural integrity analyses for real-world operational scenarios.

4. **Optimization Techniques**:
   - Incorporate multi-disciplinary optimization algorithms to balance aerodynamic performance with structural and manufacturing constraints.

---

## 📫 Contact

For further information, feel free to reach out:  
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/namita-rajendra-patil/)  
[![Email](https://img.shields.io/badge/-Gmail-red?style=flat&logo=gmail)](mailto:namitapatil1995@gmail.com)  

---

*This project was completed as part of the MSc Aerospace Dynamics course at Cranfield University.*
