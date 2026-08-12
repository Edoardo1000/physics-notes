 We see that the [[Custodial Symmetry#Effective theory|effective Lagrangian]] is a nonlinear sigma-model, identical to the **chiral Lagrangian**.
The effective theory breaks down when loop contributions become comparable to tree-level amplitudes, which happens at a scale 
$$
	E \sim \frac{4\pi v}{\sqrt{ N_{\pi} }},
$$
and *nonperturbative effects* become relevant.

Now, we know that the Higgs sector of the Standard Model is the **UV completion** of this effective theory, and the cutoff scale disappears. In particular, in the Standard Model the Higgs is *weakly interacting* above this scale.

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
If Higgs is the Goldstone mode of some *symmetry breaking*, what might be original group?

The Standard Model has $SO(4)$ **custodial symmetry**. Moreover, we have the Higgs doublet which contains four bosons. Now, the symmetry breaking $SO(5)\to SO(4)$ produces exactly four Goldstones, which is what we need.
So we might suppose that this is the right choice for the symmetry group.

We thus write our quadruplet $\{ H_{1},H_{2},H_{3},H_{4} \}$ as 
$$
	\Sigma = e^{ i H^{a}t^{a}/f }\Sigma_{0} = \left( \sin \frac{H}{f} \hat{H},\ \cos \frac{H}{f} \right)
$$
with $$f>v,\quad \Sigma_{0} = (0 \ 0 \ 0 \ 0 \ 1),\quad \hat{H}_{i} = \frac{H_{i}}{H}, \quad H = \sqrt{ \sum H_{i}^{2} }.$$
**Geometric interpretation:** This vector lies on the 4-sphere $S^{4} = SO(5) / SO(4)$. Each direction on the sphere corresponds to the four Goldstone modes $H_{i}$.
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

## Interactions with fermions
In the minimal composite Higgs, we have the symmetry breaking $SO(5) \to SO(4)$, and the Goldstone bosons had shift symmetry, why implies no mass, and no potential for $H$. However, *the Standard Model explicitly breaks $SO(5)$ symmetry*, and **a potential is allowed**.

In order to understand what the potential might be, the effective Lagrangian obtained by integrating out the composite sector has the form 
$$
	\mathcal{L}_{eff} = \bar{\psi} \not\!{q} \Pi(q^{2},H)\psi,
$$
and symmetry implies that $\Pi$ must have the form 
$$
	\Pi(q^{2},H) = \Pi_{UV}(q^{2}) + \Pi_{IR}(q^{2})\sin ^{2} \frac{H}{f},
$$
where 
- $\Pi_{UV}$ is the Higgs-independent part;
- $\Pi_{IR}$ is the coefficient of the Higgs-dependent term.

From this, using the quantum effective action, we get the *Coleman-Weinberg potential* 
$$
\begin{align}
	V(H)  & \sim \int \frac{d^{4}q}{(2\pi)^{4}} \log\left(\Pi_{UV}(q^{2}) + \Pi_{IR} (q^{2})\sin ^{2} \frac{H}{f} \right)  \\
	 &  \sim \mathrm{const}. + \alpha_{1} \sin ^{2} \frac{H}{f} + \alpha_{2} \sin ^{4 } \frac{H}{f} + \dots.
\end{align}
$$
This implies that the potential is of the form $V\left( \sin ^{2} \frac{H}{f} \right)$. Because of this, **the potential cannot give a nonzero VEV $v << f$**. Indeed, the minima are located at multiples of $\pi f$, which is too big.
Our problem is that, from the measurements of $a$, we know $f$ must be much less than $f$.

However, *fermion loops* might come to the rescue. The interactions can be
- **chiral-preserving**: $$
	[i \bar{\psi}_{L}\not\!{D}\psi_{L} \ \Pi_{L}(q^{2}) + i \bar{\psi}_{R}\not\!{D}\psi_{R} \ \Pi_{R}(q^{2})]\cos \frac{H}{f};
$$
- **mixing:**
  $$
  	\psi_{L} \not\!{D} \psi_{L} \Pi_{LR}(q^{2}) \cos \frac{H}{f}.
  $$
As a result, now the potential becomes 
$$
	V(H) = \alpha \cos \frac{H}{f} - \beta \sin ^{2} \frac{H}{f}.
$$
If we minimize the potential, we find 
$$
	\xi = \sin ^{2} \frac{H}{f} = 1 - \cos ^{2} \frac{H}{f} = 1 - \left( \frac{\alpha}{2\beta} \right)^{2}.
$$
In order to have $\xi\ll 1$, we must have $\alpha \sim 2\beta$, which is a **fine tuning**. So it appears we cannot get rid of it, **we still have the naturalness problem**.

 We have the problem of *IR corrections*: 
$$
	\Delta = \frac{\delta m^{2}}{m^{2}} \leftrightarrow \Lambda \leq 4\pi v \frac{1}{\Delta}.
$$
# UV-completion
*Take a look at [[Techicolor]].*
