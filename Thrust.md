- <span style="background:rgba(5, 117, 197, 0.2)">The amount of [Force](Force.md) that the [Powerplant](./Powerplant.md) of the aircraft is able to output</span>, or the needed amount for an aircraft to achieve a set performance
- Each engine varies in thrust output and propulsive efficiency
	- For Reciprocating Engine-Propeller Combination : *Low Thrust, High Propulsive Efficiency, rated for endurance and efficiency*
	- For Turbojet Engines/[Jet Engine](./Jet%20Engine.md) : *High Thrust, Less Propulsive Efficiency, rated for Range*
	- For [Rocket Engine](Rocket%20Engine.md) : *Tremendous Thrust, Poor Propulsive Efficiency, rated for Longest Range and Speed*

---
### Engine Thrust Equation:

$$
F = \dot{m}(V_i-V_{e}) +A_1(P_i-P_e)
$$
where:
- $V_{i}$ and $P_{i}$ are Inlet Velocity and Pressure
- $V_{e}$ and $P_e$ are Exhaust Velocity and Pressure

--- 
### Aerodynamic Thrust Equation:
$$T=\frac{L}{\frac{C_{L}}{C_{D}}}$$
$$\therefore T\text{ @ Steady, Level, Unaccelerated Flight}=\frac{L}{\frac{C_{L}}{C_{D}}}=\frac{W}{\frac{C_{L}}{C_{D}}}$$ ^f63895
---
### Propulsive Efficiency
![Pasted image 20240421190357.png](./Engineering%20Concepts%20&%20Subjects/Aerodynamics/Chapter%206%20-%20Aircraft%20Performance/Photos/Pasted%20image%2020240421190357.png)
*Propulsive Efficiency of Different Engines (Yin, 2016)*
#### Principle:
- [Propellers](./Propellers.md) have the highest efficiency among other engines, but degrade at Mach 1.
- [Turbojets](Turbojets.md) have strong velocity capabilities with ability to surpass Mach 1, thus longer range, but lower efficiency. 
- High [Bypass](Bypass.md) Turbojet engines have better efficiency compared to pure turbojets.
#### Expound: 
- [Propellers](./Propellers.md) 
	- *utilizes*: airfoils spun to generate thrust through "[Lift (L)](./Lift%20(L).md)" effects, but not equal to it. 
	- *instead*: thrust is the resultant force parallel to the longitudinal axis of the cone or aircraft caused by Thrust, Drag, and other aerodynamic effects.
	- *thus,* due to modifiable propeller radius, capturing more mass air, based on the *Thrust Equation* airfoil characteristics, increases the thrust output with less fuel consumption based on engine efficiency
	- *however,* stalling speeds exist for airfoil profiles, thus efficiency drops after reaching sonic speeds
- [Turbojets](Turbojets.md) 
	- *utilizes* the velocity of the air for thrust creation, thus the use of air inlet, compression, and combustion
	- *thus,* due to its principle, larger fuel is required to combust to achieve high speeds without the need for airfoils as the main propulsive mechanism
	- *however,* this coincidentally reduces efficiency while negating the issue of airfoil stall for Propellers
- Bypass turbojet engines
	- *utilizes* a large mass flow engine through a large inlet area, but only combusts a percentage of the input air, then relying on mass continuity to increase the velocity of the bypass air
	- *thus,* due to utilization of both mass flow and velocity, the efficiency is increased without immediate diminishing effect similar to propellers, nor the necessity to increase combustion requirements due to its design to combust only primary air
#### Efficiency Equations
- ##### General Efficiency Equation:
	- $$\eta_{p}=\frac{\text{Power Ouput}}{\text{Brake Horsepower}}$$
	- where Brake Power is the Indicated Power adjusted with Engine Efficiency Factor $\eta_{mech}(I_{p})$   
- ##### Propeller Efficiency Equation when Only $V_e$  & $V_i$ 
	- $$\eta_p=\frac{2}{1+\frac{V_{e}}{V_{i}}}$$
- ##### Propeller Efficiency Equation when Induced Velocity is given/found
	- $$\frac{1}{1+(\frac{W}{V_{0}})}$$

###### REFERENCES
- Yin, F. (2016). Modeling and Characteristics of a Novel Multi-fuel Hybrid Engine for Future Aircraft. [Dissertation (TU Delft), Delft University of Technology]. https://doi.org/10.4233/uuid:344b7d9c-f54c-483687ca-28582231a3d3