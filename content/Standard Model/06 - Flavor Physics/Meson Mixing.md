In this case, the amplitude is CP invariant, but the **initial state** is not. This happens because I cannot diagonalize $H$ and $CP$ simultaneously.

Consider a meson $M^{0},\bar{M}^{0}$. The two states are eigenstates of the flavor operator, which indicates one of the quantum numbers of the particles (such as strangeness):
$$
	F \ket{M^{0}} = \ket{M^{0}} ,\quad F\ket{\bar{M}^{0}} = - \ket{\bar{M}^{0}}.
$$
The particle dynamics is governed by an effective Hamiltonian 
$$
	H_{\mathrm{eff}} = M - \frac{i}{2} \Gamma,
$$
with both $M, \Gamma$, both hermitian. Moreover, suppose we chose phases so that CP symmetry acts as 
$$
	CP\ket{M^{0}} = \ket{\bar{M}^{0}} . 
$$
**Note:** from now on we assume *CPT symmetry*. Because of this, the diagonal elements of the Hamiltonian are equal.
The mass eigenstates are the eigenstates of the Hamiltonian:
$$
	\ket{M_{L,H}} = p\ket{M^{0}}  \pm q\ket{\bar{M}^{0}} .
$$
Where the labels stand heavy and light mesons. 
We have that **the state is CP invariant $\iff \left| \frac{q}{p} \right| =1$**.

After a short calculation, we find
$$
	\left( \frac{q}{p} \right)^{2} = \frac{M_{12}^{*} - \frac{i}{2} \Gamma_{12}^{*} }{M_{12} - \frac{i}{2}\Gamma_{12}}.
$$
Taking, the modulus square, we find the relation 
$$
	\left\lvert  \frac{q}{p}  \right\rvert = 1 \iff \mathrm{Im}(M_{12} \Gamma_{12}^{*})=0
$$

### Kaon decay

Consider the case of the kaons $K^{0},\bar{K}^{0}$. For simplicity, let's first suppose that the interaction corresponding to kaon decay is CP invariant, which does not imply that that the complete effective Hamiltonian is also CP invariant.

Now, suppose that we started from a kaon in one of its physical states
$$
	\ket{ K_{S,L}} \equiv p \ket{K^{0}}+ q \ket{\bar{K}^{0}},
$$
which evolves in time just by a phase factor, and where the labels "long" and "short" are usually used for this particle. We ask ourselves what are the particles our kaon decays into.

Since we supposed CP invariant decay interactions, the only possible decays are 
$$
	K_{1} \to \pi + \pi,\quad K_{2} \to \pi + \pi + \pi,
$$
where we defined the CP eigenstates
$$
	\ket{K_{1}} = \frac{1}{\sqrt{ 2 }}(\ket{K^{0}} + \ket{\bar{K}^{0}} ),\quad \ket{K_{2}} = \frac{1}{\sqrt{ 2 }}(\ket{K^{0}} - \ket{\bar{K}^{0}} ).
$$
If $p \simeq q$, the physical states are slightly different from the CP eigenstates, and we define $\epsilon_{K}$ by
$$
	\ket{K_{S}} \simeq \frac{\ket{K_{1}} + \epsilon_{K}\ket{K_{2}} }{\sqrt{ 1 + \lvert  \epsilon_{K}\rvert ^{2} }}, \quad \ket{K_{L}} \simeq \frac{\ket{K_{2}} + \epsilon_{K}\ket{K_{1}}}{\sqrt{ 1 + \lvert \epsilon_{K} \rvert ^{2} }}.
$$
Due to this mixing it is possible to have CP violating decays. In particular, the long-lived particle $K_{L}$ can decay in two pions, and the amplitude is given by 
$$
	A(K_{L}\to \pi \pi) \simeq \epsilon_{K} A(K_{1}\to \pi \pi).
$$
**Note:** $K_{L}$ is called long because it decays primarily in three pions, and since $m_{K} \approx 3m_{\pi}$, this decays is suppressed by the phase space factor.

We define the experimental observables
$$
	\frac{\bra{\pi^{0} \pi^{0}} H \ket{K_{L}}}{\bra{\pi^{0} \pi^{0}} H \ket{K_{S}} } \equiv \eta_{00} = \epsilon_{K} - 2 \epsilon'_{K}, \quad \frac{\bra{\pi^{+}\pi^{-}} H \ket{K_{L}} }{\bra{\pi^{+}\pi^{-}} H \ket{K_{S}} } \equiv \eta_{+ -} = \epsilon_{K} + \epsilon_{K}',
$$
where the $\epsilon_{K}'$ has been added to take into account possible [[Direct CP Violation|direct CP violation]] effects. If these were zero, then $\eta_{00}$ and $\eta_{+-}$ would be equal.


### Time-dependent mixing

The same phenomenon can have a different manifestation, depending on which particles we start from. In particular, suppose that instead of starting from a mass eigenstate we have a flavor eigenstate at $t=0$. 

Now, the state evolves in time. If at $t=0$ we had a meson in the state $\ket{M^{0}}$, then its state at time $t$ would be 
$$
	\ket{M^{0}(t)} = g_{+}(t)\ket{M^{0}} + \frac{q}{p}g_{-}(t)\ket{\bar{M}^{0}},
$$
where we defined 
$$
	g_{+}(t) = e^{ -(im+\Gamma/2) t }\cos\left( \frac{\Delta mt}{2} \right),\quad g_{-}(t) = -i e^{ -(im + \Gamma/2)t }\sin\left( \frac{\Delta mt}{2} \right),\quad m = \frac{m_{L} + m_{H}}{2},\quad \Delta m = m_{H} - m_{L}.
$$
Likewise, if we started from $\bar{M}^{0}$, the state would be 
$$
	\ket{\bar{M}^{0}(t)} = g_{+}\ket{\bar{M}^{0}} + \frac{p}{q}g_{-}(t)\ket{M^{0}}.
$$
Suppose that the particles each decay in different final products. Then there is no interference. Measuring the particle type at time $t$, we have 
$$
	P(M^{0}\to \bar{M}^{0};t) = \left\lvert  \frac{q}{p}  \right\rvert^{2},\quad P(\bar{M}^{0}\to M^{0};t) = \left\lvert  \frac{p}{q}  \right\rvert ^{2},
$$
which are different if there is CP violation.

# Calculation of $M_{12}$,

at one-loop level, the box diagram is the responsible for the mixing. The matrix element 
$$
	M_{12} = \bra{M^{0}} H \ket{\bar{M}^{0}},
$$
is subject to the [[GIM Mechanism]], and is therefore suppressed.

# Examples
### Kaon mixing
In order to violate flavor and trigger the process $M^{0}\leftrightarrow \bar{M}^{0}$, we need a corresponding *Feynman diagram*. In fact, there is a box diagram involving the **charged current**. This diagram gives an amplitude
$$
	A \sim \left( \sum_{K} V_{ki} V_{kl}^{*} \right)^{2}.
$$
We can measure
$$
	\epsilon_{k} \sim \mathrm{Im}(M_{12}) \sim \mathrm{Im}(V_{ts}^{*}V_{td})^{2} + \dots = 2 \mathrm{Im}(V_{ts}^{*}V_{td})\mathrm{Re}(V_{ts}^{*}V_{td}).
$$
We have 
$$
	V_{ts}^{*} V_{td} \sim - A^{2} \lambda^{5}(1 - \bar{\rho} - i\bar{\eta}),
$$
from which 
$$
	\epsilon_{k} \propto (1-\bar{\rho}) \bar{\eta},
$$
which is the equation of an **hyperbola**. From this we get $\eta$.

If we calculate the element $M_{12}$, the amplitude is subject to the [[GIM Mechanism]]. The most relevant term is the one for the charm ($\xi_{t}$ is small), so that we have 
$$
	M_{12} \simeq G_{F}^{2} m_{c}^{2} \xi_{c}^{2}.
$$
In the Wolfenstein parametrization, the imaginary contribution comes from the top term instead. The physical statement is that $\mathrm{Im}(\xi_{c}\xi_{t}^{*})\neq 0$.
### B meson mixing
*This is not a CP phase measurement, it only measures the mixing amplitude.*
$$
B^0 = \bar{b}d
$$
The Hamiltonian eigenstates have a **mass difference** $\Delta m = m_{H} - m_{L}$.
The mass difference can be measured by their oscillations, in particular, we have 
$$
\begin{align}
	P(B^{0}\to B^{0};t)  & = \frac{e^{ -\Gamma t }}{2}[1+\cos(\Delta m \; t)], \\
	P(B^{0}\to \bar{B}^{0};t) & = \frac{e^{ -\Gamma t }}{2}[1-\cos(\Delta m \;  t)].
\end{align}
$$
In this case the mass difference measures $(V_{tb}^{*}V_{td})^{2}$.  With this measurement, we  find  
$$
	(1-\bar{\rho})^{2} + \bar{\eta}^{2},
$$
which is a **circumference with center 1**.