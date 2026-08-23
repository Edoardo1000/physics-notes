 We see that the [[Sigma Model for Higgs#Effective theory|effective Lagrangian]] is a nonlinear sigma-model, identical to the chiral Lagrangian.
The effective theory breaks down when loop contributions become comparable to tree-level amplitudes, which happens at a scale 
$$
	E \sim \frac{4\pi v}{\sqrt{ N_{\pi} }},
$$
and nonperturbative effects become relevant.

Now, we know that the Higgs sector of the Standard Model is the UV completion of this effective theory, and the cutoff scale disappears. In particular, in the Standard Model the Higgs is weakly interacting above this scale.

Now suppose we wanted to *UV-complete the effective theory in some other way*. Looking at the interaction between the Goldstone modes and the Higgs boson, the possible terms are
$$
	\mathcal{L}_{h} = \frac{v^{2}}{4}\mathrm{Tr}[D_{\mu}U^{\dagger} D^{\mu}U]\left( 1 + 2a \frac{h}{v} + b \frac{h^{2}}{v^{2}}+ \dots \right)+\bar{q}_{L}YUq_{R}\left( 1 + c \frac{h}{v} + \dots \right).
$$
The standard model has $a = 1, \ b=1$. Calculating now the scattering amplitude between Goldstones, we find
$$
	A(\pi \pi\to \pi \pi) = \frac{1}{v^{2}}\left[ s + t - a^{2}\left( \frac{s^{2}}{s-m^{2}}+\frac{t^{2}}{t-m^{2}}  \right) \right]= \frac{s+t}{v^{2}}(1-a^{2}) + O\left( \frac{m^{2}}{E^{2}} \right).
$$
We can then read the new cutoff of the theory:
$$
	\Lambda \sim \frac{4\pi v}{\sqrt{ 1 - a^{2} }}.
$$
A measurement of the value of $a$ would then give us an estimate of the *new physics scale*.

Usually, before reaching the limit, **resonances become relevant**.

## Minimal composite Higgs
If Higgs is the Goldstone mode of some symmetry breaking, what might be original group?

The Standard Model has $SO(4)$ **custodial symmetry**. Moreover, we have the Higgs doublet which contains four bosons. Now, the symmetry breaking $SO(5)\to SO(4)$ produces exactly four Goldstones, which is what we need.
So we might suppose that this is the right choice for the symmetry group.

We thus write our quadruplet $\{ H_{1},H_{2},H_{3},H_{4} \}$ as 
$$
	\Sigma = e^{ i H^{a}t^{a}/f }\Sigma_{0} = \left( \sin \frac{H}{f} \hat{H},\ \cos \frac{H}{f} \right)
$$
with $$f>v,\quad \Sigma_{0} = (0 \ 0 \ 0 \ 0 \ 1),\quad \hat{H}_{i} = \frac{H_{i}}{H}, \quad H = \sqrt{ \sum H_{i}^{2} }.$$
**Geometric interpretation:** This vector lies on the 4-sphere $S^{4} = SO(5) / SO(4)$. Each direction orthogonal to the vector corresponds to the four Goldstone modes $H_{i}$.

Pay attention that we have two different $SO(4)$ groups:
- the $SO(4) \supset SU(2)_{L} \times U(1)_{Y}$ of the Standard Model;
- the stabilizer of $\Sigma$, for fixed $H_{i}$.
For general $H$, their intersection is only $U(1)_{\mathrm{em}}$.

We can do a gauge transformation and bring $\Sigma$ to the unitary gauge: 
$$
	\Sigma = \left( 0,\ 0,\ 0,\ \sin \frac{H}{f},\ \cos \frac{H}{f} \right).
$$
>[!warning]- Notation: embedding of the Standard Model in $SO(5)$
>We need to embed $SU(2) \times U(1)_{Y}$ inside the larger $SO(5)$ group.
>A possible way to do that is using the matrices 
>$$
>	(T^{a}_{L,R})_{I,J} = -\frac{i}{2}\left[ \frac{1}{2}\epsilon^{abc}(\delta^{a}_{I}\delta^{c}_{J}-\delta^{b}_{J}\delta^{c}_{I}) \pm (\delta^{a}_{I}\delta^{4}_{J}-\delta^{a}_{J}\delta^{4}_{I}) \right].
>$$
### Symmetry breaking
Our vector acquires a VEV $\langle \Sigma \rangle$. The Goldstone modes get eaten by the vector bosons, and the mass they acquire depends on the value of $\frac{\langle H\rangle}{f}$.
In particular, we obtain the relation 
$$
	v^{2}  = f^{2} \sin ^{2} \frac{\langle H \rangle }{f}.
$$
>[!math]- Derivation: Relation between $v$ and $\frac{\langle H \rangle}{f}$
>The interaction Lagrangian is obtained by minimal coupling:
>$$
>\mathcal{L} = \frac{1}{4} f^{2} \mathrm{Tr}[D_{\mu}\Sigma ^{\dagger}D^{\mu}\Sigma] \supset \frac{f^{2}}{4} g^{2} \sum_{a,b=1}^{3} W_{\mu}^{a}W_{\mu}^{b} \Sigma ^{\dagger} t^{a} t^{b} \Sigma =  \frac{f^{2}}{4} \frac{g^{2}}{2} \sin ^{2} \frac{H}{f} W_{\mu}^{a}W_{\mu}^{a}.
>$$
>We now expand the sine, writing $H = \langle H \rangle + h$, we have at leading order (the next order is used for interactions)
>$$
>\mathcal{L} \supset \frac{f^{2}}{4} \frac{g^{2}}{2}\sin ^{2} \frac{\langle H \rangle }{f} W_{\mu}^{a}W_{\mu}^{a}.
>$$
>Comparing with the expression for $m_W^2$ we get the desired result.

The interaction Lagrangian, writing $H = \langle H \rangle + h$ and $\xi \equiv \frac{v^{2}}{f^{2}}$, gives 
$$
	\mathcal{L}\supset \frac{1}{2} \frac{g^{2}v^{2}}{4} W_{\mu}^{a}W_{\mu}^{a}\left( 1 + \frac{2h}{v}\sqrt{ 1-\xi } + \frac{h^{2}}{v^{2}}(1 - 2\xi) \right),
$$
from which we find 
$$
	a = \sqrt{ 1-\xi },\quad b = 1-2\xi,\quad \Lambda = 4\pi f.
$$
Thus, we see that the cutoff scale grows with $f$.

## Precision tests
*Also look at [[Extensions of the Standard Model]].*

We can calculate corrections coming from these operators

# Symmetry-breaking potential

Since $H$ acquires a VEV, we would like to know which potential generates it. Moreover, from the Coleman-Weinberg potential we get 
$$
	m_{h}^{2} = \frac{d^{2}V_{\mathrm{eff}}}{dH^{2}}
$$
First, we observe that if $SO(5)$ were an exact symmetry, all possible vacua would be degenerate and all modes would be massless. However, we know that weak interactions and interactions with fermions explicitly break $SO(5)$ symmetry, and the Goldstone acquires a mass.

We will write the electroweak gauge vectors in compact form as 
$$
	A_{\mu} \equiv g W_{\mu}^{a} T^{a} + g' B_{\mu}T^{3}_{R}.
$$

To get the potential, suppose we have a generic quadratic effective action 
$$
	S_{EFT}^{(2)}[A,\Sigma] = \frac{1}{2} \int \frac{d^{4}q}{(2\pi)^{4}} A_{\mu}^{a}(-q)\Pi^{\mu \nu}_{ab}(q)A^{b}_{\nu}(q).
$$
A generic effective action can always be written in this form (for most sensible theories), and the kernel is transverse: 
$$
	q_{\mu}\Pi^{\mu \nu}_{ab} = 0 \implies \Pi^{\mu \nu}_{ab} = P^{\mu \nu}_{T} \Pi_{ab}(q,\Sigma),\quad P_{T}^{\mu \nu}= g^{\mu \nu} - \frac{q^{\mu}q^{\nu}}{q^{2}}.
$$

>[!math]- Derivation: form of the effective action
>Suppose the UV theory is composed of some particles which we collectively denote by $\chi$. The partition function is given by (we omit the $J$s since we do not need them here) 
>$$
>	Z = \int \mathcal{D}\chi \;\mathcal{D}A \;e^{ -S[\chi] - J^{\mu}_{a}A^{a}_{\mu} },
>$$
>where we supposed minimal coupling between the new particles and $A$. Now, the integral can be reorganized so that we can separate the heavy modes $\chi_{\mathrm{heavy}}$ from the Goldstone modes $\Sigma$. Thus, we have 
>$$
>	Z = \int \mathcal{D}\chi_{\mathrm{heavy}} \;\mathcal{D}\Sigma\; \mathcal{D}A \; e^{ -S[\chi,\Sigma]-J^{\mu}_{a}A_{\mu}^{a} }. 
>$$
>Now define 
>$$
>	e^{ -S_{EFT}[A,\Sigma] } = \int \mathcal{D}\chi_{\mathrm{heavy}} \; e^{ -S[\chi_{\mathrm{heavy}},\Sigma] - J^{\mu}_{a}A_{\mu}^{a} } = Z_{0}[\Sigma]\langle e^{ - J_{a}^{\mu}A_{\mu}^{a} } \rangle_{0,\Sigma} ,
>$$
>where we defined $Z_{0}[\Sigma]$ to be the partition function with gauge fields set to zero. From this, we get 
>$$
>	S_{EFT}[A,\Sigma] = -\log Z_{0}[\Sigma] - \log \langle e^{ - J^{\mu}_{a}A_{\mu}^{a} } \rangle_{0,\Sigma}. 
>$$
>We can now use the cumulant expansion 
>$$
>	\log \langle e^{ X } \rangle = \langle X \rangle _{c} + \frac{1}{2} \langle X^{2} \rangle _{c} + \frac{1}{3!}\langle X^{3} \rangle _{c}+\dots,
>$$
>and the fact that $\langle J^{\mu}_{a} \rangle=0$ due to Lorentz invariance, to finally get our result, with 
>$$
>	\Pi^{\mu \nu}_{ab}(q,\Sigma) = \langle J^{\mu}_{a}J^{\nu}_{b} \rangle _{c,0,\Sigma}.
>$$
>Moreover, since the current is usually conserved, it follows that $\Pi$ is transverse.

*Remark:* It should not be confused with the quantum effective action,  since the full $S_{EFT}$ is not generated by 1PI diagrams. It is instead the *connected* generating function, so a more appropriate name would be $W$.

*Remark:* In general, an effective action is nonlocal, so the usual thing to do would be to find.

Using the spurion technique, we can find how $\Pi$ depends on $\Sigma$, and the result is that 
$$
	\Pi(q^{2})=\Pi_{UV}(q^{2}) + \Pi_{IR}(q^{2})\sin ^{2} \frac{H}{f}.
$$
Here, $\Pi_{UV}$ and $\Pi_{IR}$ are matrices, the indices $ab$ have been suppressed. They are called this way because:
- $\Pi_{UV}$ is independent of the vacuum orientation, and survives at high momentum;
- $\Pi_{IR}$ distinguishes the broken vacuum direction, and in suppressed at high momentum.

>[!math]- Derivation: dependence of $\Pi$ on $H$
>To use the spurion technique, let's  pretend that our gauge fields transform under $SO(5)$ as 
>$$
>	A_{\mu} \to g_{5} A_{\mu} g_{5},\quad g_{5}\in SO(5),
>$$
>while $\Sigma$ transforms as $\Sigma\to g_{5}\Sigma$.
>Now, supposing the original theory is invariant under this symmetry, the only two possible quadratic invariants are 
>$$
>	I_{0} \equiv \mathrm{Tr}(A_{\mu}A_{\nu}),\qquad (A_{\mu}\Sigma)^{T}(A_{\nu}\Sigma).
>$$
>Thus, the two-point function has the general form
>$$
>	W^{(2)} = \frac{1}{2} P_{T}^{\mu \nu}[\Pi_{0}(q^{2})\mathrm{Tr}(A_{\mu}A_{\nu})+ \Pi_{1}(q^{2})(A_{\mu}\Sigma)^{T}(A_{\nu}\Sigma)].
>$$
>Now, we expand $A_{\mu}$, and write $\Sigma$ in the unitary gauge. In this case we have 
>$$
>	A_{\mu} \Sigma = \sin \frac{H}{f} A_{\mu} e_{4},
>$$
>with $e_{4}$ the fourth basis vector in the canonical basis, from which we immediately get the expression for $\Pi$ we were looking for.

## Obtaining the potential

The action we obtained is $S_{EFT}[A,\Sigma]$, to get the Coleman-Weinberg potential we need to use the [[Quantum Effective Action]]. Since in this case we are interested in the case $\langle A \rangle=0$, we can do the expansion 
$$
	H = \bar{H}+h,\quad A = a,
$$
with $h$ and $a$ small.
We have the partition function (we wrote everything directly in terms of $H$) 
$$
	Z[J] = \int \mathcal{D}A \; \mathcal{D}H\; e^{ -(S_{SM}[A])+S_{EFT}[A,H] },
$$
and we perform the Legendre transform 
$$
	\Gamma[\bar{H}] = -W[J] - J \cdot \bar{H}.
$$
Now, after adding the kinetic term for $A$ to $\Pi$, its inverse propagator is
$$
	K_{A}(q,h) = K_{A}^{(0)}(q) + \Pi_{IR}\sin ^{2} \frac{h}{f},
$$
and at one-loop level we have 
$$
	V_{\mathrm{gauge}}(h) \sim \frac{3}{2} \int \frac{d^{4}q}{(2\pi )^{4}} \log \det K_{A}(q,h),
$$
where the factor of $3$ counts the physical vector polarizations.

For fermions, the reasoning is the same, except this time we have a minus sign: 
$$
	V_{\mathrm{fer mions}}(h) \sim -2N_{c} \int \frac{d^{4}q}{(2\pi)^{4}} \log \det K_{f}(q,h).
$$
Because of the $\sin ^{2} \frac{H}{f}$ dependence, a purely bosonic contribution gives minima of the potential $v = \pi k f \geq f$, which is a problem. Thus, we need the minus sign coming from fermion loops. 

Possible interactions, written in momentum space, are:
- **chiral-preserving**: $[i \bar{\psi}_{L}\not\!{p}\psi_{L} \ \Pi_{L}(q^{2}) + i \bar{\psi}_{R}\not\!{p}\psi_{R} \ \Pi_{R}(q^{2})]$, where the form factors are even in $H$ due to gauge invariance; 
- **mixing:** $\psi_{L}\not\!{p} \psi_{L} \Pi_{LR}(q^{2})$. In this case, the form factor is odd in $H$, since $\psi_{L}\psi_{R}$ is not automatically a gauge singlet.

With this interactions, the fermionic kernel has determinant 
$$
	\det K_{f}(H) \propto p^{2} \Pi_{L}\Pi_{R} + \lvert \Pi_{LR} \rvert ^{2}.
$$
 As a result, the Coleman-Weinberg can produce terms of the form
$$
	V(H) = \alpha \cos \frac{H}{f} - \beta \sin ^{2} \frac{H}{f}.
$$
If we minimize the potential, we find 
$$
	\xi = \sin ^{2} \frac{H}{f} = 1 - \cos ^{2} \frac{H}{f} = 1 - \left( \frac{\alpha}{2\beta} \right)^{2}.
$$
In order to have $\xi\ll 1$, we must have $\alpha \sim 2\beta$, which is a **fine tuning**. A generic potential would have instead $v \sim h$.

In fact, the problem we solved was the strong dependence of the Higgs mass on UV physics.
In fact, the Coleman-Weinberg potential is suppressed by the scale of strong resonances $m_{*}$, since 
$$
	V(H) \sim \int \frac{d^{4}q}{(2\pi)^{4}} \log\left[ 1 + F(q^{2})\sin ^{2} \frac{H}{f} \right],\quad F \sim \frac{\Pi_{IR}}{\Pi_{UV}},
$$
and at scales $q\gg m_*$ the dynamics should not care about the Goldstone orientation, and therefore $F$ tends to zero.

The problem we have is in fact an **IR** one, it is not solved by formulating a particular UV-complete theory.

# UV-completion
*Take a look at [[Techicolor]].*

# How to give mass to fermions

In the Standard Model, quark masses come from the [[Electroweak Mass Generation#Fermion Mass Generation|Yukawa interaction]]. In a composite-Higgs model, $H$ is not fundamental, so the question of how it interacts with fermions is nontrivial. 

If $H$ is represented by some operator $\mathcal{O}_{H}$, then the first guess might be 
$$
	\mathcal{L}_{UV} \supset \frac{c}{\Lambda_{UV}^{\Delta_{H}-1}}\bar{q}_{L}q_{R}\mathcal{O}_{H},\quad \Delta_{H} \equiv [\mathcal{O}_{H}].
$$
For example, if the Higgs is a fermion bilinear, 
$$
	\mathcal{O}_{H} \sim \bar{\Psi} \Psi,
$$
then $\Delta_{H} \simeq 3$, and the interaction has $\Lambda_{UV}^{2}$.

However, a problem arises: at the scale $m_{*}$, do the matching 
$$
	\mathcal{O}_{H} \sim g_{*} m_{*}^{\Delta_{H}-1} H,
$$
from which we get an effective Yukawa interaction 
$$
	y_{q} \sim c g_{*} \left( \frac{m_{*}}{\Lambda_{UV}} \right)^{\Delta_{H}-1}.
$$
The problem is that we have $\Lambda_{UV} \gg m_{*}$ from experiments. If $\Delta_{H} = 3$, this cannot predict the top Yukawa coupling.

The first attempt would be to have $\Delta_{H} \simeq 1$, and this can happen in strongly couple theories. However, if this were true, then the singlet $\mathcal{O}_{H}^{\dagger} \mathcal{O}_{H}$ would have approximately dimension 2, which means the coefficient is very sensitive to UV physics.

So we have the competition **large Yukawa vs natural Higgs mass**.
### Alternative: partial compositeness

Instead of coupling the quarks directly to the Higgs, we might try to couple them to the strong sector: 
$$
	\mathcal{L}_{\mathrm{mix}} = \lambda_{L} \bar{q}_{L} \mathcal{O}_{R} + \lambda_{R} \bar{t}_{R} \mathcal{O}_{L} + \mathrm{h.c.},
$$
with $\mathcal{O}_{R,L}$ fermionic operators with the appropriate quantum numbers. This is called **partial compositeness**, the quarks do not get mass by the Higgs, but by mixing with the strong sector.

At the resonance level, the Lagrangian is 
$$
	\mathcal{L} \supset \Delta \bar{q}_{\mathrm{el}} \chi + m_{*} \bar{\chi} \chi,
$$
where $\chi$ is a composite fermion. Because of this, the mass matrix is schematically 
$$
	\begin{pmatrix}
	0 & \Delta \\ \Delta & m_{*},
	\end{pmatrix},
$$
and after diagonalization the light state is 
$$
	q_{SM} = \cos\theta q_{\mathrm{el}} + \sin\theta \chi_{\mathrm{comp}},
$$
with $\tan\theta \sim \frac{\Delta}{m_{*}}$  and there is also a heavy state 
$$
	Q_{\mathrm{heavy}} = -\sin\theta q_{\mathrm{el}} + \cos\theta \chi_{\mathrm{comp}}.
$$
Now, inside the strong sector, composite fermions couple to  to the Higgs, 
$$
	\mathcal{L}_{\mathrm{strong}} \supset g_{*} \bar{\chi}_{L} H \chi_{R},
$$
from which, after expanding, we find 
$$
	y_{q} \sim g_{*} \sin\theta_{L}\sin\theta_{R}.
$$