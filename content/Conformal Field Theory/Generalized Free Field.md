
**Definition:** A GFF is a non-local CFT operator constructed from a completely unconstrained Fock space, typically arising as the boundary dual to a massive free scalar in AdS.

## Thermal Partition Function
Because it lacks a local equation of motion (no null states), the single-particle Hilbert space is a full Verma module. The multi-particle partition function is the Plethystic exponential of the single-particle character:
$$
Z_{\mathrm{GFF}} = \prod_{(\Delta, m)} \frac{1}{1 - q^\Delta y^m}
$$
We also have 
$$
	\log{{Z}}_{\mathrm{GFF}}(q,y)=-\sum_{\Delta,m}\log(1-q^{\Delta}y^{m})=\sum_{n=1}^{\infty}{\frac{(q^{\Delta}y^{m})^{n}}{n}}=\sum_{n=1}^{\infty}{\frac{1}{n}}\sum_{\Delta,m}q^{n\Delta}y^{n m}\ .
$$
The second sum is the character of the Verma module, so we can write 
$$
	\log Z_{\mathrm{GFF}}(q,y) = \sum_{n=1}^{\infty}\frac{1}{n} \frac{q^{n \Delta}g^{n}}{(1-q^{n})(1-q^{n}y^{n})\left( 1-\frac{q^{n}}{y^{n}} \right)}.
$$

(It is also useful to add another **fugacity** $g$ that keeps track of the particle number). 

*See also the general framework in [[Thermal Correlators]].*
*For the conformal characters, see [[Conformal Characters]]*.
