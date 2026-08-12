---
tags:
  - topic/standard-model
---
The generation of [[Electroweak Mass Generation|vector boson masses]] in the Standard Model uses the Higgs doublet via the [[Higgs Mechanism|Higgs mechanism]].
However, we can describe the mass generation using an effective theory which:
- makes [[Global Symmetries of the Standard Model|custodial symmetry]] more transparent;
- makes clear where the masses come from;
- can be used to study Beyond Standard Model physics.
# Spontaneous symmetry breaking
In this formulation, the Higgs field acquires a VEV 
$$
	\langle \mathcal{H} \rangle = \frac{v}{\sqrt{ 2 }} I,
$$
which causes the symmetry breaking
$$
SU(2)_{L} \times SU(2)_{R} \to SU(2)_{V},
$$
where $SU(2)_{V}$ corresponds to the diagonal subgroup of the custodial symmetry group.
# Effective theory for the Goldstone modes
We can write
$$
	\mathcal{H} = \frac{v+h}{\sqrt{ 2 }}U, \quad U = e^{ i \sigma^{a} \pi^{a}/2v },
$$
where $U$ describes the goldstone modes of the Higgs and transforms exactly as $\mathcal{H}$.
The [[Higgs Boson Interactions|Higgs sector Lagrangian]] can also be written in the following form:
$$
\begin{align}
	\mathcal{L}_{\mathrm{Higgs}}  & = \frac{1}{2} \mathrm{Tr}[D_{\mu}\mathcal{H}^{\dagger} D^{\mu}\mathcal{H}] - \lambda (\mathrm{Tr}[\mathcal{H}^{\dagger} \mathcal{H}]-v^{2})^{2}, \\
	 & = \frac{(v+h)^{2}}{4}\mathrm{Tr}[D_{\mu}U^{\dagger} D^{\mu}U] + \frac{1}{2} (\partial h)^{2} - V(h).
\end{align}
$$
We can then focus only on the Goldstone modes, thereby getting the *sigma model Lagrangian* 
$$
	\mathcal{L}_{\sigma} = \frac{v^{2}}{4}\mathrm{Tr}[D_{\mu}U^{\dagger} D^{\mu}U].
$$
With this model, I can explicitly calculate the masses gained by the vector bosons (the calculation is the same as for the Higgs doublet, just set $U=1$).
