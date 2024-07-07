### **Mechanism and Machine Design Mind Map with Detailed References**

#### **Lecture 20: Shaft Design**
- **Key Terms**: Shaft, Key, Pulley, Sheave, Gear
- **Shaft Design**:
  - **Layout**: Draw shaft layout.
  - **Calculations**:
    - **Equation 7.12**:
      \[
      T = \frac{\pi}{16} \cdot \tau \cdot d^3
      \]
    - **Torque Summation**:
      \[
      \sum \text{Torque}_{cw} = 11 \cos(20^\circ) \cdot \left(\frac{0.6}{2}\right) - F_B \cos(25^\circ) \cdot \left(\frac{0.3}{2}\right) = 0 \implies F_B = 22.81 \text{kN}
      \]
  - **Example Problem**:
    - **Given**:
      - Radius: 18mm
      - Rotation: 600 rpm
      - Power: 30kW
    - **Key Calculation**:
      \[
      \text{Key Length} = \frac{T}{\tau \cdot r \cdot s} \cdot \text{Safety Factor}
      \]
      - Key: 10mm square, yield strength 455MPa, safety factor 2.8
- **Critical Speeds**:
  - **Formula**:
    \[
    \text{Critical Speed} = \frac{30}{\pi d} \sqrt{\frac{E I}{m}}
    \]
  - Unstable speeds and deflections.
  - Design for critical speeds twice the operating speed.
- **Influence Coefficient**:
  - **Transverse Deflection**:
    \[
    \delta_i = \frac{F_j L^3}{3 E I}
    \]
    - Deflection at location \(i\) due to unit load at location \(j\).
- **Reference**:
  - **Shigley's Mechanical Engineering Design**
    - **Chapter 7: Shafts and Shaft Components**
      - Section 7-3: Shaft Layout
      - Section 7-4: Shaft Design for Stress
      - Section 7-6: Critical Speeds for Shafts

#### **Lecture 21: Gears & Spur Gear**
- **Applications**: 
  - Reduce speed
  - Increase torque
  - Transmit power
- **Types of Gears**: 
  - Pinion
  - Spur Gears
- **Spur Gear Nomenclature**:
  - **Pitch Line Velocity (V)**:
    \[
    V = \frac{\pi d N}{60}
    \]
  - Speed (rpm)
  - Pressure angle
- **Design Equations**:
  - **Lewis Bending Equation**:
    \[
    \sigma = \frac{W_t}{F} \cdot \frac{1}{\left(\frac{b}{m} \cdot Y\right)}
    \]
  - **Bending Stress**:
    - **English Units**:
      \[
      \sigma = \frac{W_t K_o K_m K_v}{F} \cdot \frac{1}{\left(\frac{b}{m} \cdot Y\right)}
      \]
    - **SI Units**:
      \[
      \sigma = \frac{W_t K_o K_m K_v}{F} \cdot \frac{1}{\left(\frac{b}{m} \cdot Y\right)}
      \]
  - **Dynamic Factor**:
    - **English Units**:
      \[
      K_v = \left(1 + \frac{V}{1000}\right)^{-1}
      \]
    - **SI Units**:
      \[
      K_v = \left(1 + \frac{V}{60}\right)^{-1}
      \]
  - **Contact Stress**:
    \[
    \sigma_c = \sqrt{\frac{W_t K_o K_m K_v}{d_p F} \cdot \left(\frac{1 + \mu^2}{E}\right)}
    \]
- **Gear Design Procedure**:
  - Identify input speed, output speed, and power.
  - Choose gear material.
  - Specify diametral pitch/module, face width.
  - Compute stress (bending and contact) and iterate design for optimization.
- **Examples**:
  - **Example 1**:
    - **Given**: Steel spur pinion, module 3 mm, 22 teeth, 20° pressure angle, transmits 11 kW at 1200 rpm, face width 50 mm.
    - **Bending Stress Calculation**:
      \[
      \sigma = \frac{W_t}{F} \cdot \frac{1}{\left(\frac{b}{m} \cdot Y\right)}
      \]
  - **Example 2**:
    - **Given**: Speed reducer, module 4 mm, 22-tooth steel pinion, 60-tooth cast-iron gear, transmits 11 kW at 1200 rpm, face width 50 mm.
    - **Contact Stress Calculation**:
      \[
      \sigma_c = \sqrt{\frac{W_t K_o K_m K_v}{d_p F} \cdot \left(\frac{1 + \mu^2}{E}\right)}
      \]
- **Reference**:
  - **Shigley's Mechanical Engineering Design**
    - **Chapter 14: Spur and Helical Gears**
      - Section 14-1: The Lewis Bending Equation
      - Section 14-3: AGMA Stress Equations
      - Section 14-4: AGMA Strength Equations
      - Section 14-7: Dynamic Factor
      - Section 14-18: Analysis

#### **Lecture 22: Finite Element Analysis (FEA)**
- **Introduction to FEA**:
  - Application in machine design.
  - Example with FEA software (SolidWorks).
- **Background**:
  - Basics and theory of FEA.
  - Use of FEA in optimizing designs.
- **Practical Example**:
  - Step-by-step example using SolidWorks for FEA.
- **Reference**:
  - **Shigley's Mechanical Engineering Design**
    - **Chapter 19: Finite-Element Analysis**
      - Section 19-1: The Finite-Element Method
      - Section 19-3: The Finite-Element Solution Process
      - Section 19-4: Mesh Generation
      - Section 19-5: Load Application
      - Section 19-6: Boundary Conditions
      - Section 19-7: Modeling Techniques

This detailed mind map includes the specific chapters and sections from "Shigley's Mechanical Engineering Design" relevant to each lecture, providing a comprehensive guide for your studies. If you need further details or specific sections, feel free to ask!
