In addition to its gauge symmetries, the Standard Model possesses some *extra global symmetries*. They do not arise because of some deeper reasons, but because they are **accidental symmetries**, meaning that the terms appearing in the effective Lagrangian which break them are *irrelevant*.

A classical analogue is that of the **multipole expansion**:
- the monopole potential has $SO(3)$ symmetry,
- the dipole potential has $SO(2)$ symmetry,
- higher monopoles have still smaller symmetry groups.
The reasoning with effective field theories is basically the same; higher order terms have *fewer and fewer symmetries*.

# Flavor symmetry
Each fermion in the Standard Model comes in *three copies*. For example, for the electron, we have the triplet $\{ e,\mu,\tau \}$.
The [[Glashow-Weinberg-Salam Model|gauge sector]] of the Lagrangian is invariant under mixing between these flavors:
$$
	\psi^{i} \to U^{i}_{j} \psi^{j},\quad U\in U(3).
$$
Since there are five different fermion families, the flavor symmetry group is 
$$
	U(3)^{5} \approx U(1)^{5} \times SU(3)^{5}.
$$
However, **Yukawa interaction** explictitly breaks flavor symmetry down to 
$$
	U(1)_{B} \times U(1)_{e} \times U(1)_{\mu} \times U(1)_{\tau},
$$
where $B$ is a quantum number called **baryon number**.

- For the quantum numbers, see [[Baryon and Lepton Number]]
- The explicit breaking of this symmetry is described by the [[Quark Mass Basis and CKM Matrix|CKM matrix]].

# Custodial symmetry
From the [[Higgs Boson Interactions#1. The Higgs Potential and Self-Interactions|Lagrangian]] of the Higgs sector, the symmetry group is
$$
	SO(4) \sim SU(2)_{L} \times SU(2)_{R}.
$$
>[!math]- Derivation: symmetry group of the Higgs sector
>The potential is a function of $H^{\dagger}H$. If we write the Higgs doublet as
>$$
>H = \begin{pmatrix} \phi_{1} + i \phi_{2} \\ \phi_{3} + i \phi_{4} \end{pmatrix},
>$$
>we see that
>$$
>H^{\dagger}H = \phi_{1}^{2} + \phi_{2}^{2} + \phi_{3}^{2} + \phi_{4} ^{2},
>$$
>from this, the $SO(4)$ symmetry is clear.

To write more explicitly how the left and right groups act on the doublet, we can use the matrix 
$$
	\mathcal{H} \equiv (H^{c} \ H),
$$
which transforms as 
$$
	\mathcal{H} \to V_{L} \mathcal{H} V_{R}^{\dagger}.
$$
**Embedding hypercharge:** If we look at the action of $T^{3}_{R}$ on $\mathcal{H}$, we see that it behaves exactly as hypercharge (pay attention to the sign change due to the dagger on the right), so we have 
$$
	Y = T^{3}_{R},
$$
and we can define a covariant derivative 
$$
	D_{\mu}\mathcal{H} = \partial_{\mu}\mathcal{H} - ig W_{\mu}^{a}T_{L}^{a}\mathcal{H} + i g' B_{\mu}\mathcal{H}T^{3}_{R}.
$$
Note that the $g'$ in the Lagrangian part will not be invariant under $SO(4)$.
*Custodial symmetry is explicitly broken by hypercharge and the Yukawa interaction.*

Using this parametrization, we can build a [[Sigma Model for Higgs]] to describe spontaneous symmetry breaking.


