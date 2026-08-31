
> [!info]- Notation Conventions
> ![[Thermal Correlators#^q-def]]

*See also* [[Thermal Correlators]].

# Definition

- *Conformal block decomposition of 1-point functions* 
Unlike in the case of flat space, they neither vanish nor are fixed by conformal symmetry. They admit a **conformal block decomposition**: 
$$
	Z(q,y)\langle \phi(x) \rangle _{q,y} = r^{-\Delta_{\phi}}\sum_{\mathcal{O},a} \lambda^{a}_{\phi \mathcal{O}\mathcal{O}} g^{\Delta_{\phi},a}_{\Delta,l}(q,y,s),
$$
with $(r,\theta,\phi)$ spherical coordinates, $s = \sin ^{2}\theta$. The sum runs all over primaries $\mathcal{O}$ and tensor structures labeled by $a$.  
	The $\lambda^{a}_{\phi \mathcal{O}\mathcal{O}}$ are said **OPE coefficients**.
	The $g^{\Delta_{\phi},a}_{\Delta,l}$ are said **conformal blocks**. ^thermal-1pt-block



# Conformal block expansions

Inversion formulas are useful only if we have sufficient control over conformal blocks.

The formulas follow from the **Casimir differential equation** 
$$
	C_{\Delta_{\phi}}\,g_{\Delta,\ell}^{\Delta_{\phi,a}}(q,y,s)=-2\Bigl(\Delta(\Delta-3)+\ell(\ell+1)\Bigr)g_{\Delta,\ell}^{\Delta_{\phi},a}(q,y,s)\,,
$$
^casimir-eq

### Small $q$ expansion

For low temperatures, we expand the blocks as 
$$
	g^{\Delta_{\phi},a}_{\Delta,\ell}(q,u,s)= q^{\Delta}\sum_{n_{1}=0}^{\infty} q^{n_{1}}f_{n_{1}}(u,s),
$$
$$
	f_{n_{1}}(u,s) = \sum_{n_{2},n_{3}}A_{(n_{1},n_{2},n_{3})}u^{n_{2}}s ^{n_{3}}, \quad 0\leq n_{2}\leq n_{1}+\ell, \, 0\leq n_{3}\leq n_{2},
$$
where 
$$
	u = y + \frac{1}{y} - 2.
$$
The coefficients $A$ are fixed uniquely by solving the equation order by order in $q$.

A **Mathematica code** for this expansion is available at https://gitlab.com/russofrancesco1995/thermal_blocks.

### Large $\Delta$ expansion

We find that 
$$
	g^{\Delta_{\phi},a}_{\Delta,\ell}(q,y,s) = q^{\Delta} F^{\Delta_{\phi},a}_{\Delta,\ell}(q,y,s), \quad F(q,y,s) = \sum_{n=0}^{\infty}F^{(n)}(q,y,s)\Delta^{-n}.
$$
Again, solve the equation order by order in $\Delta^{-1}$, more details in https://arxiv.org/abs/2506.21671/.

