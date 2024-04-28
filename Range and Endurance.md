- The total distance (Range) and time (Endurance) traversed by an aircraft given one load of fuel.
### Basic Principle:
*Range is the amount of displacement that an aircraft design is capable of.* 
$$R=V_{\infty}dt$$
*Endurance is the amount of time an aircraft design is capable of staying aloft.*
$$E=dt$$ ^d41af2

*Therefore,* **Range** is a product of **Endurance** and **[Velocity](./Velocity.md)**.

Both are inversely proportional.
$$v=\frac{ds}{dt}=\frac{\text{Range}}{\text{Endurance}}$$

---
### Variables:
*Range and Endurance is limited by the factor of fuel amount and consumption of the [Aircraft Powerplant](./Aircraft%20Powerplant.md) due to its capabilities and aircraft [Aerodynamics](./Aerodynamics.md)* 
- $W_{0} = \text{Gross Weight}$ 
- $W_{f} = \text{Fuel Weight}$ 
- $W_{1} = \text{Weight w/o Fuel}$ 

---
### Principles:
#### General:
- $\uparrow \text{Range}$ 
	- *Power utilized for distance and lift, thus less efficiency due to necessity to provide for both.*
	- $\uparrow V, \uparrow P_{req}$
- $\uparrow\text{Endurance}$ 
	- *Power utilized for lift, thus, focus on providing lifting force increases efficiency.*
	- $\downarrow V,\downarrow P_{req}$
#### Engine-Specific:
- ##### Propeller-Driven
	*Refer to Equations below for further analysis*
	- *For Range:*
		1. Largest Possible Propeller Efficiency
		2. Lowest Possible PSFC
		3. Largest $W_{F}$
		4. Flight @ $\frac{L}{D}_{max}$ 
	- *For Endurance:*
		1. $\eta_{max}$ 
		2. $c_{min}$
		3. Largest $W_{F}$
		4. Flight @ $\frac{C_{L}^\frac{3}{2}}{C_D}$ 
		5. Flight @ SL, due to $\rho$ consideration.
- ##### Jet Engine
	- *For Range:*
		1. Flight @ $\frac{C_{L}^\frac{1}{2}}{C_{D}}_{max}$ 
	- *For Endurance:*
		1. Max Endurance @ $T_{R-min}$ 
		2. Max Endurance @ $\frac{C_{L}}{C_{D}}_{max}$ 
		3. Flight @ $\frac{C_{L}}{C_{D}}$ 
---
### Equations:
#### Weight Variable Change $(\dot{-W_{f}})$
*Not an official terminology.* 
- It describes the change in weight per time as one variable.
- The *weight of the aircraft* changes as fuel is consumed, thus is **equal** to the *weight of the fuel*
- $$\frac{dW}{dt}=\frac{dW_{f}}{dt}=\frac{-W_{f}}{t}=\dot{-W_{f}}$$
#### Specific Fuel Consumption (SFC)
- Describes the weight consumption per [Thrust](./Thrust.md), providing a factor unit.
- general equations:  ^7948b3
	- Thrust Specific Fuel Consumption:  ^d4b21f
		- *For Jet Engines or engines rated by Velocity ([Jet Engine](./Jet%20Engine.md))*  
		- $$\text{TSFC}=c_T=\frac{\dot{-W_{f}}}{T}$$
		- $$DA:\frac{\frac{N}{s}}{N}=\frac{N}{N(s)}=\frac{1}{s}$$ 

	- Power Specific Fuel Consumption:  ^800921
		- *For [Propeller](Propeller.md)-driven Engines or engines rated by Brake Power*
		- $$\text{PSFC}=c=\frac{-\dot{W_{f}}}{P}$$
		- $$DA:\frac{\frac{N}{s}}{\frac{Nm}{s}}=\frac{Ns}{Nsm}=\frac{1}{m}$$
	- Equation *for piston engine-propeller using Velocity:* $$\text{TSFC}=c_{t}=\frac{cV_{\infty}}{\eta_{pr}}$$

#### Breguet's Range and Endurance Equation
- ##### Propellers ^540682
	- *Range*
		- refer first to Endurance, obtain equation for $dt$ because $$R=ds=V_{\infty}dt$$
		- in this case, $$R=V\left(\frac{1}{c}\right)\left(\frac{C_{L}}{C_{D}}\right)\left(\frac{1}{V}\right)\int^{W_{0}}_{W_{1}}\frac{dW}{W}$$
		- Simplify, cancelling out $V$: $$R=\left(\frac{1}{c}\right)\left(\frac{C_{L}}{C_{D}}\right)\int^{W_{0}}_{W_{1}}\frac{dW}{W}$$
		- Integrate, $$R=\left(\frac{1}{c}\right)\left(\frac{C_{L}}{C_{D}}\right)\left(ln\frac{W_{0}}{W_{1}}\right)$$
	- *Endurance* 
		- for propellers, we can use PSFC because of power-base $$\text{if }c=\frac{\dot{W_{F}}}{P}=\frac{\int^{W_{0}}_{W_{1}}\frac{dW}{dt}}{P}$$
		- transposing to isolate $dt$  $$\therefore E=\int^{W_{0}}_{W_{1}}dt=\int^{W_{0}}_{W_{1}}\frac{dW}{c(P)}$$
		- expand [Power](Power.md), to obtain basic aircraft performance variables $$\therefore E=\int^{W_{0}}_{W_{1}}\frac{dW}{c(T)(V)}$$
		- expand [Thrust](./Thrust.md) to obtain relationship with Weight. *Remember this equation as $dt$* $$\therefore E=\int^{W_{0}}_{W_{1}}\left(\frac{C_{L}}{C_{D}}\right)\left(\frac{dW}{c(V)(W)}\right)=\frac{1}{c}\left(\frac{C_{L}}{C_{D}}\right)\left(\frac{1}{V}\right)\int^{W_{0}}_{W_{1}}\frac{dW}{W}=dt$$
		- expand Velocity to extract Weight Factor $$\text{if } V=\sqrt\frac{2W}{\rho sC_{L}}$$ $$\therefore E=\frac{1}{c}\left(\frac{C_{L}}{C_{D}}\right)\left(\sqrt\frac{\rho s C_{L}}{2W}\right)\int^{W_{0}}_{W_{1}}\frac{dW}{W}$$
		- extract W from velocity equation to combine and integrate with $\frac{dW}{W}$, W in Velocity becomes $\frac{1}{\sqrt{W}}=\frac{1}{W^{\frac{1}{2}}}$ , which can be multiplied to $\frac{dW}{W}$  $$\therefore E=\frac{1}{c}\left(\frac{C_{L}^\frac{3}{2}}{C_{D}}\right)\left(\sqrt\frac{\rho s}{2}\right)\int^{W_{0}}_{W_{1}}\frac{dW}{W^\frac{3}{2}}$$
		- integrate $$\therefore E=\frac{1}{c}\left(\frac{C_{L}^\frac{3}{2}}{C_{D}}\right)\left(\sqrt\frac{\rho s}{2}\right)\frac{-2}{[\sqrt{W}]^{W_{0}}_{W_{1}}}$$
- ##### Jet Engines ^dfd8ef
	- *Range*
		-  Obtain $dt$ from Endurance, and Multiply $V$ due to $R=V_{\infty}dt$  $$R=ds=V_{\infty}dt=V\left[\frac{1}{c_{T}}\left(\frac{C_{L}}{C_{D}}\right)\left(\int^{W_{0}}_{W_{1}}\frac{dW}{W}\right)\right]$$
		- based from Velocity equation derived from Lift equation $$\text{if } V=\sqrt\frac{2W}{\rho sC_{L}}$$
		- Substitute Velocity, $$\therefore R=\sqrt\frac{2W}{\rho sC_{L}}\left[\frac{1}{c_{T}}\left(\frac{C_{L}}{C_{D}}\right)\left(\int^{W_{0}}_{W_{1}}\frac{dW}{W}\right)\right]$$
		- Extract and combine $C_{L}$ and $W$ from the Velocity equation $$\therefore R=\sqrt\frac{2}{\rho s}\left[\frac{1}{c_{T}}\left(\frac{C_{L}^\frac{1}{2}}{C_{D}}\right)\left(\int^{W_{0}}_{W_{1}}\frac{dW}{W^\frac{1}{2}}\right)\right]$$
		- Integrate, $$\therefore R=\sqrt\frac{2}{\rho s}\left[\frac{1}{c_{T}}\left(\frac{C_{L}^\frac{1}{2}}{C_{D}}\right)\left(2[\sqrt{W}]^{W_{0}}_{W_1}\right)\right]$$
	- *Endurance*
		- for propellers, we can use TSFC because of thrust-base $$\text{if }c_{T}=\frac{\dot{W_{f}}}{T}=\frac{\frac{dW}{dt}}{T}$$
		- transposing to isolate $dt$  $$E=dt=\int \frac{dW}{c_{t}T}$$
		- Isolating integral and substituting [Thrust](./Thrust.md#^f63895) equation, then integrating $$E=dt=\int_{W_{1}}^{W_{0}}\frac{dW}{c_{t}T}=\frac{1}{c_{T}}\left(\frac{C_{L}}{C_{D}}\right)\left(ln\frac{W_{0}}{W_{1}}\right)$$

#### Range and Endurance for Battery-Power Aircraft
- Range Equation: $$E_{max}=(Rt)^{1-n}\left(\frac{\eta_{tot}VC}{\left(\frac{1}{\sqrt{\rho S}}\right)\left(C_{D0}^{\frac{1}{4}}\right)\left(\frac{2W}{\sqrt{k}}\right)^\frac{3}{2}}\right)^{n}\left(\sqrt{\frac{2W}{\rho S}\sqrt{\frac{k}{C_{D0}}}}\right)\left(3.6k\right)$$
- Endurance Equation: $$E_{max}=(Rt)^{1-n}\left(\frac{\eta_{tot}VC}{\left(\frac{1}{\sqrt{\rho S}}\right)\left(C_{D0}^{\frac{1}{4}}\right)\left(\frac{2W}{\sqrt{k}}\right)^\frac{3}{2}}\right)^{n}h$$