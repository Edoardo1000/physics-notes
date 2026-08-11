When the *path integral measure* is not invariant under a classical symmetry transformation, we are witnessing an **anomaly**.
Suppose we have a transfomation which changes the **fermion** path integral measure:
$$
	\psi\to U\psi = e^{ i\alpha^{a}T^{a} } \quad D\bar{\psi}\psi \to e^{ i \int d^{4}x \;\alpha^{a}\mathcal{A}^{a}(x) },
$$
then the *Ward identities* become 
$$
	\langle \partial_{\mu} J_{\mu}^{a}(x) \rangle = \mathcal{A}^{a}(x)
$$
# Triangle diagrams
Triangle diagrams such as the **pion decay** one have to be regularized. Now, the problem with *dimensional regularization* is that **the fifth gamma matrix** cannot be defined for $D=4-2\epsilon$. Moreover, for $D=5$ the fifth gamma is one of the other matrices, I do not have chiral fermions.

The trick is to define the index $\mu = \bar{\mu} + \hat{\mu}$, with $\hat{\mu}\sim \epsilon$.
In the calculation with the regulator there will be terms $\gamma_{\hat{\mu}}\gamma_{5}$, which have to disappear.

The final result is that 
$$
	\mathcal{A}^{a}(x) = -\frac{1}{32\pi^{2}} \epsilon_{\mu \nu \rho \sigma} F_{\mu \nu}^{b}F_{\rho \sigma}^{c}\mathrm{Tr}[T^{a}\{ T^{b},T^{c} \}].
$$
# Vector-like representations
A **vector-like representation** satisfies 
$$
	T^{*} = -S^{\dagger} T S,
$$
which means that the representation is *isomorphic to its conjugate*. In this case, I must have 
$$
	\mathrm{Tr}[T_{a}\{ T_{b},T_{c} \}] = 0
$$
The following groups have only real representations:
- $SO(2n+1)$
- $SO(4n)$
- $Sp(2n)$
- $G_2,F_4,E_7,E_8$ (exceptional Lie groups)

The following groups, gave $d^{abc}=0$, and thus no anomalies:
- $SO(4n+2), (n\geq 2)$
- $E_6$