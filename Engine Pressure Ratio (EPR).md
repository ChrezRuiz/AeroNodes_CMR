---
tags:
  - Engine_Thrust_Indicator
---
### Definition
- EPR is a thrust indicating system and a back-up system for [%RPM Indicator (Compressor Speed)](./%25RPM%20Indicator%20(Compressor%20Speed).md) on engines using N<sub>1</sub> as their primary performance parameter
- The ratio between discharge pressure and inlet pressure, or turbine discharge pressure and compressor inlet pressure
- *Principle:*
		- The pressure buildup causes potential energy, which is then transformed into kinetic energy. Thus, the higher the compression ratio, the higher the discharge pressure, the more thrust.
		- [Thrust](./Thrust.md) produced for turbofan engines can be calculated through pressure data at the **engine inlet** and **high-pressure turbine discharge** (nozzle)
### *Recall:* ![Thrust > Engine Thrust Equation](./Thrust.md#Engine%20Thrust%20Equation) ![Bernoulli's Equation > General Equation](./Bernoulli's%20Equation.md#General%20Equation)![Bernoulli's Equation > Basic Continuity Equation](./Bernoulli's%20Equation.md#Basic%20Continuity%20Equation)
- *Thus:* Pressure data acquisition at both the inlet and outlet can be used to calculate the velocity at both regions and to calculate both factors of the thrust equation

---
### EPR Equation
$$\text{EPR}=\frac{P_{t_{e}}}{P_{t_{i}}}\text{ or }IEPR=\frac{P_{t_{e}}+P_{\text{bypass}}}{P_{t_{i}}} $$
where:
- $\text{EPR = Engine Pressure Ratio}$
- $\text{IEPR = Integrated Pressure Ratio}$ 
- $P_{t_{e}}=\text{Discharge Pressure}$
- $P_{t_{i}}=\text{Inlet Pressure}$
- $P_{\text{bypass}}=\text{Bypass Air Pressure}$ 

---
### Modern Systems
- Differential pressure transducer analyzes pressure at each probe to indicate data in the cockpit
- Modern systems compensate for airspeed and altitude effects *(Recall [Density](./Density.md))* 

### Turbine Discharge Pressure
![Turbine Discharge Pressure (TPR)](./Turbine%20Discharge%20Pressure%20(TPR).md)