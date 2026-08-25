In this case, the amplitude is CP invariant, but the **initial state** is not. This happens because *I cannot diagonalize $H$ and $CP$ simultaneously*.

Consider a meson $M^{0},\bar{M}^{0}$. The two states are eigenstates of the *flavor operator*, which indicates one of the quantum numbers of the particles (such as strangeness):
$$
	F \ket{M^{0}} = \ket{M^{0}} ,\quad F\ket{\bar{M}^{0}} = - \ket{\bar{M}^{0}}.
$$
The particle dynamics is governed by an *effective Hamiltonian* 
$$
	H_{\mathrm{eff}} = M - \frac{i}{2} \Gamma,
$$
with both $M, \Gamma$, both hermitian. Moreover, suppose we chose phases so that CP symmetry acts as 
$$
	CP\ket{M^{0}} = \ket{\bar{M}^{0}} . 
$$
**Note:** from now on we assume *CPT symmetry*. Because of this, the diagonal elements of the Hamiltonian are equal.
The **mass eigenstates** are the eigenstates of the Hamiltonian:
$$
	\ket{M_{L,H}} = p\ket{M^{0}}  \pm q\ket{\bar{M}^{0}} .
$$
Where the labels stand *heavy and light mesons*. 
We have that **the state is CP invariant $\iff \left| \frac{q}{p} \right| =1$**.

After a short calculation, we find
$$
	\left( \frac{q}{p} \right)^{2} = \frac{M_{12}^{*} - \frac{i}{2} \Gamma_{12}^{*} }{M_{12} - \frac{i}{2}\Gamma_{12}}.
$$
Taking, the modulus square, we find the relation 
$$
	\left\lvert  \frac{q}{p}  \right\rvert = 1 \iff \mathrm{Im}(M_{12} \Gamma_{12}^{*})=0
$$

### Example: kaon decay

Consider the case of the kaons $K^{0},\bar{K}^{0}$. For simplicity, let's first suppose that the interaction corresponding to kaon decay is CP invariant, which does not imply that that the complete effective Hamiltonian is also CP invariant.

Because of this, the only possible decays are 
$$
	K_{1} \to \pi + \pi,\quad K_{2} \to \pi + \pi + \pi,
$$
where we defined the CP eigenstates
$$
	\ket{K_{1}} = \frac{1}{\sqrt{ 2 }}(\ket{K^{0}} + \ket{\bar{K}^{0}} ),\quad \ket{K_{2}} = \frac{1}{\sqrt{ 2 }}(\ket{K^{0}} - \ket{\bar{K}^{0}} ).
$$
Now, the true physical particles which propagate through time are instead the Hamiltonian eigenstates 
$$
	\ket{ K_{S,L}} \equiv p \ket{K^{0}}+ q \ket{\bar{K}^{0}},
$$
where the pedices stand for "short" and "long", referring to their lifetimes. The second particle is long-lived because it decays in three pions, and since $m_{K}\approx 3 m_{\pi}$ its decay is greatly suppressed by the phase space.

If $p \simeq q$, the physical states are slightly different from the CP eigenstates, and we define $\epsilon_{K}$ by
$$
	\ket{K_{S}} \simeq \frac{\ket{K_{1}} + \epsilon_{K}\ket{K_{2}} }{\sqrt{ 1 + \lvert  \epsilon_{K}\rvert ^{2} }}, \quad \ket{K_{L}} \simeq \frac{\ket{K_{2}} + \epsilon_{K}\ket{K_{1}}}{\sqrt{ 1 + \lvert \epsilon_{K} \rvert ^{2} }}.
$$
Due to this mixing it is possible to have CP violating decays. In particular, the long-lived particle $K_{L}$ can decay in two pions, and the amplitude is given by 
$$
	A(K_{L}\to \pi \pi) \simeq \epsilon_{K} A(K_{1}\to \pi \pi).
$$
We define the experimental observables
$$
	\frac{\bra{\pi^{0} \pi^{0}} H \ket{K_{L}}}{\bra{\pi^{0} \pi^{0}} H \ket{K_{S}} } \equiv \eta_{00} = \epsilon_{K} - 2 \epsilon'_{K}, \quad \frac{\bra{\pi^{+}\pi^{-}} H \ket{K_{L}} }{\bra{\pi^{+}\pi^{-}} H \ket{K_{S}} } \equiv \eta_{+ -} = \epsilon_{K} + \epsilon_{K}',
$$
where the $\epsilon_{K}'$ has been added to take into account possible [[Direct CP Violation|direct CP violation]] effects. If these were zero, then $\eta_{00}$ and $\eta_{+-}$ would be equal.


## Example:  Kaon mixing
$$
K^{0} = d\bar{s}
$$
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

## Example: B meson mixing
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

# One-loop calculation: the GIM mechanism
The loop is made by a $q^{j}$ line and a $\bar{q}^{i}$ line joined by two $W$ propagators.
A *dimensional analysis* argument would give that the amplitude goes like $G_{F}^{2}m_{W}^{2}$, but this is **wrong**, and kaon processess were much more *suppressed* than originally estimated.
Let's do the calculation in detail.

The amplitude goes like 
$$
	A = \sum_{k,l} V_{ki}^{*}V_{kj} V_{li}^{*}V_{lj}  F(m_{k},m_{l}) \equiv \sum_{k,l} \xi_{k}\xi_{l} F_{kl}.
$$
Moreover, we know that $\sum_{k} \xi_{k} = 0$ from unitarity, which implies (consider $F_{ui} \approx F_{0i}$, the up mass is small)
$$
\begin{align}
	A  & = \sum_{l}\xi_{l}[\xi_{c}(F_{cl} - F_{0l}) + \xi_{t}(F_{tl} - F_{0l})]  \\
	 & = \xi_{t}^{2}(F_{tt} + F_{00} - 2F_{t 0}) + \xi_{c}^{2}(F_{cc} + F_{00} - 2 F_{c 0}) + 2 \xi_{t} \xi_{c}(F_{ct} + F_{00} - F_{c 0}- F_{t_{0}}) \\
	 & \equiv \xi_{t}^{2} A_{tt} + \xi_{c}^{2} A_{cc} + 2 \xi_{t} \xi_{c} A_{ct}.
\end{align}
$$
I can Taylor expand the $A_{ij}$: 
$$
	A(m) \approx A(0) + \frac{m^{2}}{m_{W}^{2}}A'(0),
$$
from which we see that **the naif power counting misses a factor of $\frac{m_q^2}{m_W^2}$**. Thus, we have an amplitude 
$$
	A \sim G_{F}^{2}m_{c}^{2}.
$$

**Fun fact:** the **charm quark** was predicted based on symmetry/aesthetic arguments, but the GIM mechanism, along with explanation of vanishing flavor-changing neutral currents made the prediction very appealing.

**The mechanism was used to estimate the charm mass**. Indeed, kaon mixing gives 
$$
	\Delta m_{K} \propto G_{F}^{2} m_{c}^{2},
$$
which gave a bound on $m_{c}$ of about $1 \ \mathrm{GeV}$.