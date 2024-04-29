### Definition
- the velocity achievable can be derived using the equation discussed prior, particularly the thrust equation at steady, level, unaccelerated flight, ![Thrust](./Thrust.md#^f63895) where velocity can be extracted from dynamic pressure $(q)$![Dynamic Pressure (q)](./Dynamic%20Pressure%20(q).md#^5ed2e9)
- if finding: Max Value
	- use: Thrust Available $(T_{a})$
- if finding Min Value
	- use: Thrust Required $(T_{r})$ 

---
### Principles
*to increase maximum velocity:*
1. Increase [Thrust to Weight Ratio](Thrust%20to%20Weight%20Ratio.md) $\left(\frac{T_{A}}{W}\right)_{max}$ 
2. Increasing the [S)](Wing%20Loading%20(W/S).md) 
3. Decreasing [Zero-Lift Drag Coefficient](Zero-Lift%20Drag%20Coefficient.md) $C_{D_{0}}$ 

---
### Equations
- #### General Equation
	- Thrust is equal to drag, thus can be equated $$T_{a}=D=qs[C_{d_{0}}+k(C_{l})^{2}]$$
	- $C_{l}$ can be substituted to its basic form to obtain $q$ which is factored by $V$ $$\text{where }C_{l}=\frac{W}{qs}\therefore T_{a}=qs\left[C_{d_{0}}+k\left(\frac{W^{2}}{q^{2}s^{2}}\right)\right]$$
	- multiply both sides by q to create quadratic equation, which allows q to be obtained $$ q \left[T_{a}=qs\left[C_{d_{0}}-k\left(\frac{W^{2}}{q^{2}s^{2}}\right)\right]\right] \rightarrow q^{2}sC_{d_{0}}-qT_{a}+\frac{kW^{2}}{s}=0$$
	- use the quadratic formula to find the value of $q$ ![Quadratic Formula](./Quadratic%20Formula.md#^01b5a4)
	- therefore, $$q=\frac{T_{a}\pm \sqrt{T_{a}^{2}-4(sC_{d_{0}})(\frac{kW^{2}}{2})}}{2sC_{d_0}}$$
	- *recall:* ![Dynamic Pressure (q)](./Dynamic%20Pressure%20(q).md#^5ed2e9)
	- which can then be equated to $$V=\sqrt{\frac{T_{a}\pm \sqrt{T_{a}^{2}-4(sC_{d_{0}})(\frac{kW^{2}}{2})}}{qsC_{d_0}}}$$
- #### Equation considering Wing Loading
	- Wing loading consideration is important in understanding the limits of the airframe and the structure of the aircraft $$V_{max}=\sqrt{\frac{\left(\frac{T_{A}}{W}\right)_{max}\left(\frac{W}{S}\right)+\frac{W}{S}\sqrt{\left(\frac{T_{A}}{W}\right)^{2}-(4C_{D_{0}}k)}}{\rho_{\infty}C_{D_{0}}}}$$
