Take for example 
$$
	V_{ud}V_{ub}^{*} + V_{cd} V_{cb}^{*} + V_{td} V_{tb}^{*} = 0,
$$
Now, divide by $V_{cd}V_{cb}^{*}$, to get
$$
	1 + \frac{V_{ud}V_{ub}^{*}}{V_{cd}V_{c b}^{*}} + \frac{V_{td}V_{tb}^{*}}{V_{cd}V_{c b}^{*}}= 0,
$$
which can also be rewritten as 
$$
	1 - (\bar{\rho} + i \bar{\eta}) - (1-\bar{\rho} - i\bar{\eta}) =0,
$$
where we defined 
$$
	\bar{\rho} + i \bar{\eta} \equiv - \frac{V_{ud}V_{ub}^{*}}{V_{cd}V_{cb}^{*}}.
$$
The equation states that the three numbers form a triangle with vertices 
$$
	1,\quad 0,\quad \bar{\rho} + i \bar{\eta}.
$$
At leading order, we have 
$$
	\bar{\rho} + i \bar{\eta} = (\rho + i \eta)\left( 1 - \frac{\lambda^{2}}{2}+\dots \right),
$$
where $\rho$ and $\eta$ come from the [[CKM Parametrization and Geometry#Wolfenstein parametrization|Wolfenstein parametrization]].

**Observation:** If we look at triangles involving other matrix elements, they not have terms of the same order in $\lambda$, so they need to much more precision in order to be measured.
### Area and the Jarlskog invariant

Take two sides of the original triangle. The area of the triangle made by two complex numbers $z,w$ is given by $\frac{1}{2}\mathrm{Im}(z w^{*})$. Taking to sides of the unnormalized triangle, the area is 
$$
	A = \frac{1}{2} |\mathrm{Im}[V_{ud} V_{ub}^{*}V_{cd}V_{c b}^{*}]| \equiv \frac{\lvert J \rvert}{2},
$$
where we defined the **Jarlskog invariant** 
$$
	J \equiv \mathrm{Im}[V_{ud}V_{cd} V_{ub}^{*}V_{c b}^{*}].
$$
In fact, all the possible unitarity triangles have the same area.
We also have the relation 
$$
	\mathrm{Im}(V_{ij}V_{kl}V_{il}^{*}V_{kj}^{*}) = J \sum_{m,n}\epsilon_{ikm}\epsilon_{j l n}
$$

We defined $\bar{\rho},\bar{\eta}$ after normalizing the original triangle. This shrunk the area by a factor $\lvert V_{cd}V_{c b}^{*} \rvert^{2}$. Since the area of the normalized triangle is also $\lvert  \frac{\bar{\eta}}{2}\rvert$, we get the relation 
$$
	J = \lvert V_{cd} V_{c b}^{*} \rvert^{2} \bar{\eta}, 
$$
up to an orientation-dependent sign.

>[!math]- Derivation of the $J$ relation
>Since I can always define of the products as real, I have 
>$$
>\mathrm{Im}(V_{ki}V_{kj}^{*})_{k=1} + \mathrm{Im}(V_{ki V_{kj}^{*}}) = 0,
>$$
>from which I easily conclude.

## CP violation

In general, we have CP violation **if and only if no allowed rephasing of the fields makes all CKM elements real**.

For three generations this is equivalent to 
$$
	J \neq 0.
$$
In the standard parametrization, the Jarlskog invariant translates to 
$$
	J = c_{12} c_{23}c_{13}^{2}s_{12}s_{23}s_{13} \sin\delta.
$$
Thus, if any of the angles vanished, then there would be no CP violation
## Invariant expressions

The observables we built were not invariant under $U(3)$ transformations. This is because we already diagonalized the Yukawa matrices. There is another way  to describe physical CP violation, and this is done through **invariants**. 

Since, under a flavor transformations, the Yukawa matrices transform as (we use the spurion technique)
$$
	Y_{u} \to U_{L}Y_{u}V^{\dagger}_{u_{R}},\quad Y_{d}\to U_{L} Y_{d} V_{d_{R}}^{\dagger},
$$
from which we can build the matrices 
$$
	H_{u} = Y_{u}Y_{u}^{\dagger},\quad H_{d} = Y_{d}Y_{d}^{\dagger}.
$$
Now, quantities such as 
$$
	\mathrm{Tr}[H_{u},H_{d}]^{n},\quad \det[H_{u},H_{d}]
$$
are invariant. In particular, the determinant is CP-odd, and is a direct measure of physical CP violation.

We also have the **Jarlskog relation**:
$$	\det[Y_{u}Y_{u}^{\dagger},Y_{d}Y_{d}^{\dagger}] = 2iJ \prod_{i < j}(m_{u_{i}^{2}} - m_{u_{j}^{2}})(m_{d_{i}}^{2}-m_{d_{j}}^{2}).
$$
This relation shows that  **CP violation $\iff$ $J \neq 0$ and no quarks are degenerate**.