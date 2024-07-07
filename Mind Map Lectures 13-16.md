### Mechanism and Machine Design Mind Map

#### **Lecture 13: Material Strength and Stiffness**
- **Strength**
  - Capacity to withstand great force/pressure
- **Stiffness**
  - Rigidity, resistance to deformation
- **Load Classification**
  - **With respect to time**: Static, Impact, Cyclic
  - **With respect to area**: Concentrated, Distributed
  - **With respect to location and method**: Shear, Normal, Bending, Combined, Torsion
- **Support Reactions**
  - Types: Cable, Roller, Pin, Fixed support
- **Axial Loading**
  - **Stress Types**: 
    - **Normal Stress**: \(\sigma = \frac{P}{A}\)
    - **Shear Stress**: \(\tau = \frac{V}{A}\)
    - **Torsional Stress**: \(\tau = \frac{T \cdot r}{J}\)
  - **Stress-Strain Diagram**
    - **Ductile Materials**: Yield strength (\(\sigma_y\)), Ultimate strength (\(\sigma_u\)), Necking, Fracture
    - **Brittle Materials**: Modulus of Elasticity (\(E\)), Ultimate strength
- **Torsional Loads on Circular Shafts**
  - **Elastic Torsion Formulas**:
    - \(\tau = \frac{T \cdot r}{J}\)
    - \(\theta = \frac{T \cdot L}{J \cdot G}\)
  - **Torsional Failure Modes**
    - Ductile: Shear failure
    - Brittle: Tensile failure along 45° planes
- **Examples**:
  - **Example 1**: Determine the shear stress at Pin A and C
    - **Solution**: 
      \[
      \tau = \frac{V}{A}
      \]

#### **Lecture 14: Shear Force and Bending Moment Diagrams**
- **Shear Force and Bending Moment Diagrams**
  - Calculation of reaction forces
  - **Example 1**:
    - **Problem**: Draw the shear force and bending moment diagram for the beam shown.
    - **Solution**:
      - Calculate the reaction forces \(A_y= 5.75 \, \text{kN}\) and \(C_y= 34.25 \, \text{kN}\).
      - Draw the shear force diagram:
        - \(V(x)\) from 0 to 5 m: \(V = 5.75 \, \text{kN}\)
        - \(V(x)\) from 5 to 10 m: \(V = -9.25 \, \text{kN}\)
      - Draw the bending moment diagram:
        - \(M(x)\) from 0 to 5 m: \(M = 5.75x\)
        - \(M(x)\) from 5 to 10 m: \(M = 80 - 9.25(x-5)\)
- **Bending/Normal Stress in a Beam**
  - **Normal Stress**: \(\sigma = \frac{M \cdot y}{I}\)
  - **Section Modulus**: \(S = \frac{I}{c}\)
- **Design of Prismatic Beams for Bending**
  - Normal stress, section modulus
- **Deformation of Beams Under Transverse Loading**
  - **Elastic Curve Equation**:
    - \(\frac{d^2 y}{dx^2} = \frac{M}{EI}\)
  - **Beam Deflection and Slope**:
    - \(\delta_{max} = \frac{P \cdot L^3}{48 \cdot E \cdot I}\) (Simply supported beam, center load)
    - \(\theta = \frac{P \cdot L^2}{16 \cdot E \cdot I}\) (Cantilever beam, end load)
- **Examples**:
  - **Example 2**: Determine the centroid of a beam with the given cross-section.
    - **Solution**:
      - Divide the cross-section into simpler shapes.
      - Calculate the area and centroid of each shape.
      - Use the formula for the centroid: \( \bar{y} = \frac{\sum A_i y_i}{\sum A_i} \).
  - **Example 3**: Determine the maximum stress in compression and tension for a beam with the given load and cross-section.
    - **Solution**:
      \[
      \sigma = \frac{M \cdot c}{I}
      \]
  - **Example 4**: Determine the maximum allowable value of \( w \) for a beam with the given load and material properties.
    - **Solution**:
      \[
      w = \frac{\sigma_{allow}}{(L \cdot b)}
      \]
  - **Example 5**: Determine the equation of deflection for the simply supported beam with the load distribution shown, using the superposition method.
    - **Solution**:
      \[
      \delta(x) = \sum \delta_i(x)
      \]

#### **Lecture 15: Mohr’s Circle**
- **Mohr’s Circle**
  - **Principal Stresses**:
    - \(\sigma_{1,2} = \frac{\sigma_x + \sigma_y}{2} \pm \sqrt{\left(\frac{\sigma_x - \sigma_y}{2}\right)^2 + \tau_{xy}^2}\)
  - **Angle of Principal Planes**:
    - \(\tan 2\theta_p = \frac{2\tau_{xy}}{\sigma_x - \sigma_y}\)
- **Examples**:
  - **Example 1**:
    - **Problem**: Given stress values, draw Mohr’s Circle and find principal stresses.
    - **Solution**:
      - Plot points \((\sigma_x, \tau_{xy})\) and \((\sigma_y, -\tau_{xy})\).
      - Find the center \(C = \left(\frac{\sigma_x + \sigma_y}{2}, 0\right)\).
      - Calculate the radius \(R = \sqrt{\left(\frac{\sigma_x - \sigma_y}{2}\right)^2 + \tau_{xy}^2}\).
      - Principal stresses: \(\sigma_1 = C + R\), \(\sigma_2 = C - R\).

#### **Lecture 16: Failures Resulting from Static Loading**
- **Static Load Failures**
  - Definitions and types of failure
- **Static Strength**
  - Design considerations
  - Published strength values
- **Stress Concentration**
  - **Stress Concentration Factors**:
    - \(K_t = \frac{\sigma_{max}}{\sigma_{nom}}\)
    - \(K_{ts} = \frac{\tau_{max}}{\tau_{nom}}\)
  - Causes: Geometric discontinuities, material irregularities, surface cracks
- **Ductile Failure Theory Example**
  - Given parameters and calculation of factor of safety
  - **Mohr’s Circle Application**
    - Use for calculating combined stress states
  - **Von Mises Stress Calculation**:
    - \(\sigma_e = \sqrt{\sigma_1^2 - \sigma_1\sigma_2 + \sigma_2^2}\)

#### **Example Problems and Solutions**
- **Example 1**: Determine the shear stress at Pin A and C
  - **Solution**: 
    \[
    \tau = \frac{V}{A}
    \]
- **Example 2**: Draw the shear force and bending moment diagram for a given beam.
  - **Solution**:
    - Calculate the reaction forces \(A_y= 5.75 \, \text{kN}\) and \(C_y= 34.25 \, \text{kN}\).
    - Draw the shear force diagram:
      - \(V(x)\) from 0 to 5 m: \(V = 5.75 \, \text{kN}\)
      - \(V(x)\) from 5 to 10 m: \(V = -9.25 \, \text{kN}\)
    - Draw the bending moment diagram:
      - \(M(x)\) from 0 to 5 m: \(M = 5.75x\)
      - \(M(x)\) from 5 to 10 m: \(M = 80 - 9.25(x-5)\)
- **Example 3**: Determine the centroid of a given beam cross-section.
  - **Solution**:
    - Divide the cross-section into simpler shapes.
    - Calculate the area and centroid of each shape.
    - Use the formula for the centroid: \( \bar{y} = \frac{\sum A_i y_i}{\sum A_i} \).
- **Example 4**: Determine the maximum stress in compression and tension for a beam with the given load and cross-section.
  - **Solution**:
    \[
    \sigma = \frac{M \cdot c}{I}
    \]
- **Example 5**: Determine the maximum allowable value of \( w \) for a beam with the given load and material properties.
  - **Solution**:
    \[
    w = \frac{\sigma_{allow}}{(L \cdot b)}
    \]
- **Example 6**: Determine the equation of deflection for the simply supported beam with the load distribution shown, using the superposition method.
 

 - **Solution**:
    \[
    \delta(x) = \sum \delta_i(x)
    \]
- **Example 7**: Given stress values, draw Mohr’s Circle and find principal stresses.
  - **Solution**:
    - Plot points \((\sigma_x, \tau_{xy})\) and \((\sigma_y, -\tau_{xy})\).
    - Find the center \(C = \left(\frac{\sigma_x + \sigma_y}{2}, 0\right)\).
    - Calculate the radius \(R = \sqrt{\left(\frac{\sigma_x - \sigma_y}{2}\right)^2 + \tau_{xy}^2}\).
    - Principal stresses: \(\sigma_1 = C + R\), \(\sigma_2 = C - R\).

### Visualization of Topics
- **Main Concepts**: Strength, Stiffness, Load Classification, Support Reactions, Stress-Strain Behavior, Torsional Loads
- **Diagrams and Equations**: Shear Force, Bending Moment, Elastic Curve, Mohr’s Circle
- **Failure Analysis**: Static Load, Stress Concentration, Ductile and Brittle Failures
- **Practical Applications**: Beams, Shafts, Machine Elements

### References to Shigley's Mechanical Engineering Design 9th Edition
- **Lecture 13**: Chapters 2, 3, and 4
- **Lecture 14**: Chapters 3 and 4
- **Lecture 15**: Chapter 3
- **Lecture 16**: Chapters 3 and 4

---

This mind map integrates the lectures' key concepts, examples, solutions, and references to Shigley's Mechanical Engineering Design 9th Edition for a comprehensive understanding of the topics.
