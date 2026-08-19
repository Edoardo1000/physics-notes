Consider the process 
$$
	n\to p + e + \bar{\nu}_{e},
$$
which is described by the effective Lagrangian 
$$
	\mathcal{L} = \frac{G_{F}}{\sqrt{ 2 }}(\bar{p} \gamma^{\mu}(1-\alpha\gamma_{5})n)(\bar{e}\gamma_{\mu}(1-\gamma_{5})\nu_{e}),
$$
where $G_{F}$ is known as **Fermi's constant**, and $\alpha$ is a dimensionless number, which would be $1$ if the neutron were an elementary particle. The interaction is also known as **Fermi interaction**.

The Lagrangian is an effective description of electroweak interactions from the [[Glashow-Weinberg-Salam Model]], after integrating out the $W$ bosons. Since the neutron and the proton are QCD bounds states, and QCD at low energy is nonperturbative, the parameter $\alpha$ needs to be found experimentally.
By matching, we find that 
$$
	G_{F} = \frac{\sqrt{ 2 }}{8} \frac{g^{2}}{m_{W}^{2}}.
$$
**Note:** Since the neutron is a composite particle, and $G_{F}$ describes Fermi interaction at the level of fundamental particles, it is reasonable to expect that $\alpha\neq 1$. However, one might wonder why the expression is not the more general $\beta - \alpha \gamma_{5}$, with a coefficient also in the vector part of the interaction. This is due to isospin symmetry.

>[!math]- Derivation: coefficient of the vector part
>
>At the quark level, the interaction is dictated by the current (see also [[Gauge Boson Mixing and Currents]])
>$$
>	J_{\mathrm{weak}}^{\mu} = \bar{u}\gamma^{\mu}(1-\gamma_{5})d = \bar{u} \gamma^{\mu}d - \bar{u} \gamma^{\mu}\gamma_{5}d \equiv V^{\mu} - A^{\mu}.
>$$
>To compute the amplitude, we need the matrix element 
>$$
>	\bra{p(p')} V^{\mu}(0)\ket{n(p)} = \bar{u}_{p}(p')\left[ f_{1}(q^{2})\gamma^{\mu}+ f_{2}(q^{2}) \frac{\sigma^{\mu \nu}}{2m} q_{\nu} + f_{3}(q^{2}) \frac{\sigma^{\mu \nu}}{2m} q_{\nu} \right]u_{n}(p),
>$$
>with $q=p'-p$. The equation comes from requiring Lorentz covariance, and the functions $f_{i}(q^{2})$ are known as form factors. The matrix element of the axial current has an analogous expression: 
>$$
>\bra{p(p')} A^{\mu}(0)\ket{n(p)} = \bar{u}_{p}(p')\left[ g_{1}(q^{2})\gamma^{\mu}\gamma_{5}+ g_{2}(q^{2}) \frac{\sigma^{\mu \nu}}{2m} q_{\nu}\gamma_{5} + g_{3}(q^{2}) \frac{\sigma^{\mu \nu}}{2m} q_{\nu} \gamma_{5}\right]u_{n}(p).
>$$
>In neutron decay, we have $\lvert q \rvert\ll m_{N}$, so we can approximate 
>$$
>	J_{\mathrm{weak}}^{\mu} \simeq \bar{u}_{p}[f_{1}(0)\gamma^{\mu} - g_{1}(0)\gamma^{\mu}\gamma_{5}]u_{n}.
>$$
>Now, in the limit $m_{u} \approx m_{d}$, we have isospin symmetry $SU(2)_{V}$
>$$
>	\begin{pmatrix}
>	u \\ d
>	\end{pmatrix} 
>	\to
>	e^{ i\theta_{a} \sigma^{a}/2 } 
>	\begin{pmatrix}
>	u \\ d
>	\end{pmatrix},
>$$
>with conserved current 
>$$
>	V^{\mu}_{a} = \bar{q} \gamma^{\mu} \frac{\sigma_{a}}{2}q.
>$$
>Now, define the conserved charge 
>$$
>	Q_{+} = \int d^{3}x V_{+}^{0},\quad V_{+} \equiv V_{1} + i V_{2} = \bar{u} \gamma^{\mu}d.
>$$
>This charge acts on all states in the Hilbert space, and since we know that the proton and the neutron form a isospin doublet, we have 
>$$
>	Q_{+}\ket{n} = \ket{p} \implies \bra{p(p')} Q_{+}\ket{n(p)}  = 2E_{\mathbf{p}}(2\pi)^{3}\delta(\mathbf{p'}-\mathbf{p}),
>$$
>where we used covariant normalization of state vectors. In turn, expanding the charge, we have 
>$$
>	\begin{align}
>	\bra{p(p')} Q_{+} \ket{n(p)} & = \int d^{3}x e^{ i (\mathbf{p'}-\mathbf{p})\cdot \mathbf{x} }\bra{p(p')} V^{0}_{+}(0)\ket{n(p)}  \\
>	 & \simeq (2\pi)^{3}\delta(\mathbf{p'}-\mathbf{p}) f_{1}(0)\bar{u}_{p}\gamma^{0}u_{n} \\
>	 & = 2E_{\mathbf{p}} (2\pi)^{3} \delta(\mathbf{p'}-\mathbf{p}) f_{1}(0).
>	\end{align}
>$$
>Here we used the fact that translation symmetry implies 
>$$
>	V_{+}^{\mu}(x) = e^{ i P\cdot x }V_{+}^{\mu}(0)e^{ -i P \cdot x },
>$$
>and that in the limit $m_{p} = m_{n},$ we have the identity ${u}(\mathbf{p})^{\dagger}u(\mathbf{p})=2E_{\mathbf{p}}$. Thus, we found 
>$$
>	f_{1}(0) = 1,
>$$
>which implies that the coefficient in the effective action is exactly $1$.
 # Wu experiment

Consider the decay of a polarized proton, with polarization $\vec{P}$. 
In the experiment, we cannot measure neutrinos, and we only see the outgoing electron, while the proton is basically at rest.
The squared amplitude, after summing over electron and neutrino polarizations, is 
$$
\begin{align}
	\sum_{\sigma}{\lvert A \rvert }^{2} & = 32m^{2}[E_{e}E_{\nu}(1 + 3\alpha^{2}) + \vec{p}_{e} \cdot \vec{p}_{\nu}(1-\alpha^{2}) \\
	& + 2 \vec{P} \cdot ((\mathrm{Re}\alpha - \lvert \alpha \rvert ^{2})E_{e}\vec{p}_{\nu} + (\mathrm{Re}\alpha + \lvert \alpha \rvert ^{2})E_{\nu}\vec{p}_{e}) - 2 \mathrm{Im}\alpha \vec{P} \cdot (\vec{p}_{e}\wedge \vec{p}_{\nu})].
\end{align}
$$
The parameter we can really measure is $E_{\nu}\vec{p}_{e}$.
If we integrate over the neutrino direction, use conservation of energy, and measure the asymmetry, we are able to find 
$$
	\alpha \approx 1.27.
$$