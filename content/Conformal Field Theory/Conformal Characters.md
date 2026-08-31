
# Verma modules

Since we have conformal symmetry, the family of an operator is built in the following way:
- Start with a **primary** operator $\mathcal{O}(0)$ which creates the state $\ket{\Delta}$ when acting on the vacuum.
- Build the **descendants** by acting on the state with $P_{\mu}$.
The **Verma module** is the space spanned by  
$$
	\ket{\Delta} ,\quad P_{\mu}\ket{\Delta} \quad P_{\mu}P_{\nu}\ket{\Delta} 
$$

For the conformal group $SO(3,2)$, the characters on the parabolic Verma modules are given by 
$$
	\chi_{\Delta,l}(q,y) = \mathrm{Tr}_{V_{\Delta,l}}(q^{D}y^{M})= \frac{q^{\Delta}y^{-l}(1-y^{2l+1})}{(1-q)(1-y)(1-qy)\left( 1-\frac{q}{y} \right)}.
$$
They satisfy the orthogonality relations 
$$
	\int_{\gamma-i\infty}^{\gamma + i \infty}d\beta \int_{-\pi}^{\pi} d\mu \omega(\beta,\mu) \chi_{\Delta_{1},l_{1}}(\beta,\mu)\chi_{3-\Delta_{2},l_{2}}(\beta,\mu) = 2\pi i \delta(\Delta_{1}-\Delta_{2}) \delta_{l_{1},l_{2}},
$$
with the measure 
$$
	\omega(\beta,\mu) = \left( \frac{8}{\sqrt{ \pi }} \sinh \frac{\beta}{2} \sin \frac{\mu}{2} \sinh \frac{\beta+i\mu}{2} \sinh \frac{\beta-i\mu}{2}\right)^{2}
$$