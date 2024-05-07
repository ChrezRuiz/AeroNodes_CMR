---
tags:
  - Engine_Condition_Indicator
---
### Definition
- critical limiting factor of jet engine operation
- crucial to monitor to avoid turbine overheat and damage

### Types:
- ![Turbine Inlet Temperature (TIT)](./Turbine%20Inlet%20Temperature%20(TIT).md)
- ![Turbine Outlet Temperature (TOT)](./Turbine%20Outlet%20Temperature%20(TOT).md)
- ![Interstage Turbine Temperature (ITT)](./Interstage%20Turbine%20Temperature%20(ITT).md)
---
### Ram Effect Consideration
*adequate consideration to fluid motion effects to parameters is required for accurate indication*
*Recall:* $\frac{T_{t}}{T_{s}}$ ratio with $M$ 
$$\frac{T_{t}}{T_{s}}=1+\left[\frac{\gamma -1}{2}(M^{2})\right]$$
Such that, temperature rise due to ram effects can be calculated, and the actual temperature can also be determined. Depending on the [K-type Thermocouple](./K-type%20Thermocouple.md), it can identify either. 

--- 
### EGT Limits
- Internal Temperature Affects Engine lifetime
- Modern engines are designed to start and maintain at lowest possible temperatures
	- immediate start of high temperatures reduces service life
	- low starting temperature allows cooling air to pass

---
### System Components
- [K-type Thermocouple](./K-type%20Thermocouple.md)
- Circuit Leads
- Variable Calibrating Sensor
- [d'Arsonval Meter](./d'Arsonval%20Meter.md) (Analog)
- EICAS (Digital)

---
### System Operation (Temperature)
- each [K-type Thermocouple](./K-type%20Thermocouple.md) (or any thermocouple) may have single or multiple hot junctions. When connected in a closed-loop, the conductors change resistance at a set rate when heated, affecting average current produced.
- when heated, free electrons move from hot to cold junctions then back. Thus, creating a current.
- Electron theory and hot-cold junction ends
	- electrons flow from hot to cold then hot due to the current pressure, creating a loop
	- if: heat is applied on both junctions
		- then: current is produced on both ends
		- effect: current is cancelled out = no current flow = no reading
- for Ram effect consideration (fluid motion), refer to [Turbine Engine Exhaust Gas Temperature (EGT) > Ram Effect Consideration](Turbine%20Engine%20Exhaust%20Gas%20Temperature%20(EGT).md#Ram%20Effect%20Consideration)

---

