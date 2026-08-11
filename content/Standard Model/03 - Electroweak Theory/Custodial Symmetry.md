From the [[Higgs Boson Interactions#1. The Higgs Potential and Self-Interactions|Lagrangian]] of the Higgs sector, the symmetry group appears to be 
$$
	G_{H} = SO(4) \sim SU(2)_{L} \times SU(2)_{R}.
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
We also observe that **hypercharge** can be embedded in this symmetry group by identifying 
$$
	Y = T^{3}_{R}.
$$
### Spontaneous breaking
The Higgs field acquires a VEV 
$$
	\langle \mathcal{H} \rangle = \frac{v}{\sqrt{ 2 }} I,
$$
which causes the symmetry breaking $SU(2)_{L} \times SU(2)_{R} \to SU(2)_{V}$.


### Effective theory for the Goldstone modes
By writing 
$$
	\mathcal{H} = \frac{v+h}{\sqrt{ 2 }}U, \quad U = e^{ i \sigma^{a} \pi^{a}/2v }
$$
we can get an effective action which describes the *vector boson mass generation*. 
Them matrix is subject to the transformation 
$$
	\mathcal{H}\to V_{L}\mathcal{H}V_{R},\quad V_{L / R} \in SU(2).
$$
We go from the Higgs Lagrangian 
$$
	\mathcal{L}_{\mathrm{Higgs}} = \frac{1}{2} \mathrm{Tr}[D_{\mu}\mathcal{H}^{\dagger} D^{\mu}\mathcal{H}] - \lambda (\mathrm{Tr}[\mathcal{H}^{\dagger} \mathcal{H}]-v^{2})^{2},
$$
to the effective Lagrangian 
$$
	\mathcal{L}_{\mathrm{eff}} = \frac{(v+h)^{2}}{4}\mathrm{Tr}[D_{\mu}U D^{\mu}U] + \frac{1}{2} (\partial h)^{2} - V(h),
$$
which is very similar to the pion Lagrangian, this might give hints about the [[Composite Higgs]] model.

### Explicit breaking
In fact, only the generator $T^{3}_{R}$ is gauged. $g'$ **explicitly breaks the symmetry**. If $g'$ were zero, $W$ and $Z$ would have the same masses.

In the effective Lagrangian, I can write 
$$
	\mathcal{L} = \frac{v^{2}}{4}\mathrm{Tr}[D_{\mu}U^{\dagger} D^{\mu}U] + \epsilon \frac{v^{2}}{4} \mathrm{Tr}[D_{\mu}U^{\dagger} U \sigma_{3}]^{2},
$$
from which  we have 
$$
	m_{Z}^{2} \to m_{Z}^{2}(1-2\epsilon) \implies \rho=1+2\epsilon.
$$
Thus, this term in the effective action is what parametrizes the breaking of custodial symmetry. We have bounds on $\epsilon$.

If the breaking comes from higher-dimension operators of BSM physics, the Lagrangian should be 
$$
	\mathcal{L} = \frac{1}{\Lambda^{2}}\mathrm{Tr}[D_{\mu}\mathcal{H}^{\dagger} \mathcal{H} \sigma_{3}],
$$
from which we deduce $\epsilon \sim \frac{v^{2}}{\Lambda^{2}}$.

