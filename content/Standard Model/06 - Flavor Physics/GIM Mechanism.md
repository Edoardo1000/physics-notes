
The mechanism is the suppression of flavor-changing neutral current (FCNC) interactions due to the unitarity of the [[Quark Mass Mixing and CKM Matrix|CKM matrix]].

# Example: penguin diagrams

Consider the $\Delta S=1$ process 
$$
	s\to d+\gamma,
$$
which is governed by a penguin diagram. The amplitude goes like 
$$
	A(s\to d\gamma) \sim \sum_{k=u,c,t} V_{ks}^{*}V_{kd} F(m_{k}),
$$
with $F$ some function. Writing 
$$
	\xi_{k}\equiv V_{ks}^{*}V_{kd},
$$
unitarity of the CKM matrix implies
$$
	\sum_{k} \xi_{k} = 0.
$$
Substituting this expression for one of the quarks (for example $u$, label it 0), we have 
$$
	A \sim \sum_{k=c,t} \xi_{k}[F(m_{k})-F(m_{0})].
$$
Taylor-expanding $F$ in powers of $\frac{m_{k}^{2}}{m_{W}^{2}}$ (which comes from expanding the proapagators in the loop), we see that the mass-independent part does not contribute to the amplitude, and the leading order has a **$\frac{m_q^2}{m_W^2}$ suppression**.

# Example: meson mixing

Consider the meson-mixing process
$$
	q^{j} \bar{q}^{i} \to \bar{q}^{j}q^{i}.
$$
The amplitude of this process comes from a box diagram
The loop is made by a $q^{j}$ line and a $\bar{q}^{i}$ line joined by two $W$ propagators.

A dimensional analysis argument would tell us that the amplitude goes like $G_{F}^{2}m_{W}^{2}$, but again we need to take into account the suppression factor.

In this case, the amplitude goes like
$$
	A = \sum_{k,l} V_{ki}^{*}V_{kj} V_{li}^{*}V_{lj}  F(m_{k},m_{l}) \equiv \sum_{k,l} \xi_{k}\xi_{l} F_{kl}.
$$
Using again the relation $\sum_{k} \xi_{k} = 0$, which implies 
$$
\begin{align}
	A  & = \sum_{l}\xi_{l}[\xi_{c}(F_{cl} - F_{0l}) + \xi_{t}(F_{tl} - F_{0l})]  \\
	 & = \xi_{t}^{2}(F_{tt} + F_{00} - 2F_{t 0}) + \xi_{c}^{2}(F_{cc} + F_{00} - 2 F_{c 0}) + 2 \xi_{t} \xi_{c}(F_{ct} + F_{00} - F_{c 0}- F_{t{0}}) \\
\end{align}
$$
From this, we see again that the flavor-independent contribution gets canceled, and the final amplitude goes like
$$
	A \sim G_{F}^{2}m_{c}^{2}.
$$

**Fun fact:** the **charm quark** was predicted based on symmetry/aesthetic arguments, but the GIM mechanism, along with explanation of vanishing flavor-changing neutral currents made the prediction very appealing.
