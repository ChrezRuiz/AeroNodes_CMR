Provides an algorithm of identifying factor coefficients, which are unitless, considering a set of variables affecting the experiment. 

The theorem itself can be explored by imagining at the basic color wheels. Other sources may provide alternating letters to identify a variable, but the principle remains the same.

### Step 1: Basic Units of the Known Universe $(k)$ 
- *Primary Colors*
- *Identify:* the number of basic units to be used, usually 3 (mass, length, & time). Such that no other units can go below the listed.

### Step 2: Variables Affecting the Field of Study $(N)$ 
- *Secondary Colors*
- *Identify:* variables can be imagined as secondary colors, as each is derived from a combination of some or all the $k$s.
- For the field of Aeronautics involving propellers, these are usually 6:
	1. Force
	2. Diameter
	3. Velocity
	4. Angular Velocity
	5. Fluid Viscosity 
	6. Fluid Density

### Step 3: Identify $\pi$ Functions
- *Equation for Tertiary Colors*
- An understanding of the principles is needed to obtain the equations. 
- *Identify:* variables that exist in all coefficients, then the variable that the coefficient is based on. 
- *where:* a coefficient of force and viscosity is affected by Velocity, Density, and the shape of the object (Diameter), but $C_F$ is based on the effect of Force, while the latter is based on the effect of $\mu$.
- The number of equations possible can be determined by:$$k-N$$
- For the field of Aeronautics involving propellers, these are usually 3:
	- $\pi_{1}=f_1(V,\rho,D,F)=C_F$ 
	- $\pi_{2}=f_{2}(V,\rho,D,\mu)=C_{\mu}=\frac{1}{RN}$  
	- $\pi_{3}=f_3(V,\rho,D,w)=C_{w}=\frac{1}{J}$ 

### Step 4: Solve for $\pi$ Functions
- *Obtaining Tertiary Colors*
- The goal is to cancel out all units. 
- *Perform:* assignment of exponent on each variable, except the non-common variable. Rewrite in units format and simplify. *Take* exponents of each basic unit and identify the value of each assigned exponent such that the sum of which is 0.
- For the field of Aeronautics involving propellers, for $\pi_{1}$:
	- $\pi_{1}=(lt^{-1})^{a}(ml^{-3})^{b}(l)^{c}(mlt^{-2})$  
		- $m=b+1=0,\therefore b=-1$
		- $t=-a-2=0,\therefore a=-2$ 
		- $l=0=a-3b+c+1=-2-3(2)+c+1, \therefore c=-2$ 

### Step 5: Substitute and Solve
- *Perform:* Substitution, thus, positioning each variable where each basic unit would be cancelled out. Creating a coefficient or unitless variable.
- For the field of Aeronautics involving propellers, for $\pi_{1}$:
	- $\pi_{1}=(V^{-2})(\rho^{-1})(D^{-2})(F)=\frac{F}{(V^{2})(\rho)(D^{2})}=C_{F}$ 