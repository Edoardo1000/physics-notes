---
tags:
  - topic/standard-model
---
If we consider all the fermion flavors, the [[Electroweak Mass Generation#Fermion Mass Generation|Yukawa couplings]] are in fact *matrices*, which do not need to be diagonal, and different flavors are mixed.

 If we try to diagonalize the matrices $Y_{e},Y_{u},Y_{d}$, we discover that $Y_{u},Y_{d}$ cannot be diagonalized at the same time, meaning that some mixing must occur.

However, since it's better to work with a diagonal mass matrix, we can move the mixing terms in the *charged current Lagrangian* and get 
$$
	\mathcal{L}_{cc} \supseteq \bar{u}_{L} V_{\mathrm{CKM}} \gamma_{\mu} d_{L} + \mathrm{h.c.},
$$
where $V_{\mathrm{CKM}}$ is called the **CKM matrix**.
**Note:** the neutral current is unchanged only at *tree level*.

>[!math]- Derivation: CKM matrix
>The transformations we can perform that leave the Lagrangian unchanged apart from the Yukawa sector are 
>$$
> Q \to V_{Q}Q,\quad u_{R} \to V_{u} u_{R},\quad d_{R} \to V_{d}d_{R}. 
> $$
>We diagonalize the Yukawa matrices, and we write
>$$
> Y_{u} = U_{u_{L}}^{\dagger} \hat{Y}U_{u_{R}}, \quad Y_{d} = U_{d_{L}}^{\dagger} \hat{Y}_{d} U_{d_{R}}.
> $$
>If we choose $V_{Q} = U_{d_{L}}^{\dagger}, V_{d} = U_{d_{R}}^{\dagger}, V_{u} = U_{u_{R}}^{\dagger}$,
>we are left with the diagonal mass matrix $\hat{Y}_{d}$, and the nondiagonal part 
>$$
>\bar{Q}V\hat{Y}_{u}u_{R}H^{c}.
>$$
>At this point, we can no longer change the fields, and we are thus forced to have states which mix. However, we can move this ugly matrix to the weak interaction. 
>This is done by the transformation
>$$
> u_{L} \to Vu_{L},
>$$ 
>and keeping $d_{L}$ fixed. This way, the mass matrices are now diagonal. However, this is not a symmetry of the Lagrangian, and the charged current interaction becomes
>$$
> \bar{u}_{L} V_{\mathrm{CKM}}\gamma_{\mu}d_{L}, 
> $$
>with $V_{\mathrm{CKM}} \equiv V^{\dagger}$.

The final group of symmetries is thus 
$$
	G_{\mathrm{SM}} = U(1)_{B} \times U(1)_{e} \times U(1)_{\mu} \times U(1)_{\tau}.
$$
---
#### See also
- **[[CKM Parametrization and Geometry]]**
- **[[Flavor Measurements and CP Violation]]**