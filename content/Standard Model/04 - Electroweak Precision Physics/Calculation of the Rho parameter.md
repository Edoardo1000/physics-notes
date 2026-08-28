---
tags:
  - type/derivation
---
We work in the scheme $\{ G_{F}, m_{Z}, \alpha \}$. Moreover, we will use the *on-shell renormalization scheme*. In our context, the physical values 
$$
	v^{2} = \frac{1}{\sqrt{ 2 }G_{F}},\quad g_{Z} \equiv \frac{g}{2c_{W}} = (\sqrt{ 2 } G_{F}m_{Z}^{2})^{1/2}
$$
are considered fixed.

For the calculation of $\Delta \rho_{f}$, it is sufficient to look at the axial part of the [[Effective EW parameters|effective vertex]]. Given $g_{A}^{eff} = g_{A}\left( 1 + \frac{1}{2} \Delta \rho_{f} \right)$, this has the form
$$
	\mathcal{V}_{A} = g_{Z} g_{A} \left( 1 + \frac{1}{2} \Delta \rho_{f}  \right).
$$
## One-loop amplitude
To find with the 1-loop amplitude, we are going to use renormalized perturbation theory. We start from the bare Lagrangian 
$$
	\mathcal{L}_{B} = g_{Z 0} Z_{0 \mu} \psi_{0} \gamma^{\mu} (g_{V 0} - g_{A}\gamma_{5})\psi_{0},
$$
(notice that $g_{A}$ is just an integer, so it does not renormalize) and do the substitution 
$$
	Z_{0 \mu} = \sqrt{ Z_{Z} }Z_{\mu},\quad \psi_{0} = \sqrt{ Z_{f} }\psi, \quad g_{Z,V,A 0} = g_{Z,V} + \delta g_{Z,V}.
$$
We thus have the physical tree vertex 
$$
	\mathcal{L}_{\mathrm{tree}} = g_{Z} Z_{\mu} \psi \gamma^{\mu}(g_{V}-g_{A}\gamma_{5})\psi,
$$
where the couplings and the fields are now the physical ones, plus some counterterms 
$$
	\mathcal{L}_{CT} = \mathcal{L}_{tree} \left[ \frac{\delta g_{Z}}{g_{Z}} + \frac{1}{2} \delta Z_{Z} + \delta Z_{f} \right] + g_{Z} Z_{\mu}\bar{\psi}\gamma^{\mu}\delta g_{V}\psi.  
$$
Now, let's look at the interaction vertex at 1-loop level, more specifically the axial part: 
$$
	A_{A} = g_{Z}\left[   g_{A} + g_{A}\left( \frac{\delta g_{Z}}{g_{Z}} + \frac{1}{2} \delta Z_{Z} \right) + A_{\mathrm{loop}} + g_{A}\delta Z_{f}\right].
$$
Comparing with the effective vertex, we find 
$$
	\Delta \rho_{f} = 2 \frac{\delta g_{Z}}{g_{Z}} + \delta Z_{Z} + 2 \frac{\Delta g_{A}}{g_{A}},\quad \Delta g_{A} \equiv A_{\mathrm{loop}} + g_{A}\delta Z_{f}.
$$
For a charged lepton, $g_{A} = -\frac{1}{2}$, thus we have
$$
	\Delta \rho = 2 \frac{\delta g_{Z}}{g_{Z}} + \delta Z_{Z} - 4 \Delta g_{A}.
$$
We now have to write explicitly the counterterms, which are determined by our on-shell renormalization condition.
## Renormalization conditions
 While $v, m_{Z}, g_{Z}$ are fixed, their bare counterparts possess the counterterms $\delta v, \delta m_{Z}^{2},\delta g_{Z}$. They are linked by the relation
$$
	m_{Z,0}^{2} = g_{Z,0}^{2} v_{0}^{2} \implies 2 \frac{\delta g_{Z}}{g_{Z}} =  \frac{\delta m_{Z}^{2}}{m_{Z}^{2}} - 2 \frac{\delta v}{v}.
$$
Muon decay also fixes $\delta v$: at one-loop level, the decay amplitude is 
$$
	A_{\mu} = \frac{1}{2v^{2}}\left[ 1 - 2 \frac{\delta v}{v} - \frac{\Pi_{WW}(0)}{m_{W}^{2}} + \frac{\delta G_{F}^{V+B}}{G_{F}} \right],
$$
where $\delta G_{F}^{V+B}$ represents corrections such as 1PI vertex diagrams, box diagrams and so on. Since it should correspond to the physical value $\frac{G_{F}}{\sqrt{ 2 }} = \frac{1}{2v^{2}}$, we must have 
$$
	2 \frac{\delta v}{v} = - \frac{\Pi_{WW}(0)}{m_{W}^{2}} + \frac{\delta G_{F}^{V+B}}{G_{F}}.
$$
Now, the other renormalization conditions also impose
- $\delta m_{Z}^{2} + \Pi_{Z Z}(m_{Z}^{2}) = 0$;
- $\delta Z_{Z} = \Pi_{Z Z}'(m_{Z}^{2})$.
Putting all together, we find 
$$
	\Delta \rho_{f} = - \frac{\delta G_{F}^{V+B}}{G_{F}} + \frac{\Pi_{WW}(0)}{m_{W}^{2}} - \frac{\Pi_{Z Z}(m_{Z}^{2})}{m_{W}^{2}} + \Pi_{Z Z}'(m_{Z}^{2}) - 4 \Delta g_{A}.
$$
Writing  
$$
\Pi_{Z Z}(q^{2}) = \Pi_{ZZ}(0) + q^{2} F_{ZZ}(q^{2}),\quad\Pi_{ZZ}'(q^{2}) = F_{Z Z}(q^{2}) +q^{2} F'_{Z Z}(q^{2}),
$$
we find our final result 
$$
	\Delta \rho_{f} = -\frac{\Delta G_{F}^{V + B}}{G_{F}} + \left( \frac{\Pi_{WW}(0)}{m_{W}^{2}} - \frac{\Pi_{Z Z}(0)}{m_{Z}^{2}}\right) + m_{Z}^{2} F_{Z Z}'(m_{Z}^{2}) - 4 \Delta g_{A}.
$$
Now, the relevant part is the one in parentheses. Using that $c_{W}^{2} \Pi_{Z Z}(0) = \Pi_{33}(0)$ (the photon cannot mix at $q^{2}=0$), we have 
$$
	\Delta \rho_{f} \approx \frac{1}{m_{W}^{2}}(\Pi_{33}(0)-\Pi_{WW}(0))
$$
# Goldstone modes trick

![[../assets/goldstone_equivalence.svg|540]]

To find $\Pi_{AA}(0)$, consider the low-energy effective Lagrangian obtained from expanding the Higgs sector and using 
$$
	H \approx \begin{pmatrix}
	i\pi^{+} \\ \frac{v + h + i\pi^{0}}{\sqrt{ 2 }}.
	\end{pmatrix}
$$
Retaining only second-order interactions in the fields, the *bare* Lagrangian reads (suppose the field renormalizations factors are $1$)
$$
	\mathcal{L} = -\frac{1}{4}Z_{\mu \nu}Z^{\mu \nu} - \frac{1}{2}W_{\mu \nu}^{+}W^{-}_{\mu \nu}+Z_{+}\lvert \partial_{\mu}\pi^{+} - m_{W}W^{+} \rvert ^{2} + \frac{1}{2}Z_{0}(\partial_{\mu}\pi^{0} + m_{Z} Z_{\mu})^{2}.
$$
Computing the quantum effective action for $\pi^{0}$, we find 
$$
	\Gamma_{\pi^{0}\pi^{0}} = p^{2} + \delta Z_{0}p^{2} + \Sigma_{0}(p^{2}),\quad \delta Z_{0} = Z_{0}-1,
$$
with $\Sigma_{0}(p^{2})$ the sum of 1PI diagrams appearing in the $\pi^{0}$ propagator. Note that $\Sigma_{0}(0)=0$ since Goldstone modes are massless. Taylor expanding $\Sigma_{0}$, we obtain that the quantum effective action contains the term 
$$
	\Gamma_{\mathrm{eff}} \supset \frac{K_{0}}{2}(\partial_{\mu}\pi^{0})^{2},\quad K_{0} \equiv 1 + \delta Z_{0} + \Sigma_{0}'(0).
$$
Now, gauge invariance implies that the quantum effective action must take the form 
$$
	\Gamma_{\mathrm{eff}} \supset \frac{K_{0}}{2}(\partial_{\mu}\pi^{0}+m_{Z}Z_{\mu})^{2} + K_{+}\lvert \partial_{\mu}\pi^{+} - m_{W}W_{\mu} \rvert ^{2},
$$
where the definition of $K_{+}$ is analogous to the one of $K_{0}$.
Looking now at the vector part of the quantum effective action, we have 
$$
	\Gamma_{Z Z} = F_{Z}(p^{2})p^{2} - K_{0} m_{Z}^{2},
$$
with $F_{Z}(p^{2})$ a function containing loops and counterterms. It is not relevant since $F_{Z}(p^{2})p^{2}\bigr|_{p^{2}=0} =0$. From this we find 
$$
	\frac{\Pi_{Z Z}(0)}{m_{Z}^{2}}=K_{0}-1,\quad \frac{\Pi_{WW}(0)}{m_{W}^{2}} = K_{+}-1.
$$
From which we find 
$$
	\Delta \rho_{f} \approx K_{+} - K_{0} = \Sigma_{+}'(0) - \Sigma_{0}'(0).
$$
Note that $Z_{0}=Z_{+}$, since the two couplings come from the same interaction in the Standard Model, so they cancel in the final expression.
# Goldstone-fermion loops

![[../assets/pizero_t_loop.svg|267]]

The Yukawa interaction from the Standard Model is written as 
$$
	\mathcal{L}_{Y} \supset -\frac{i}{v} \pi^{0} (m_{t} \bar{t}\gamma^{5}t - m_{b}\bar{b}\gamma^{5}b) + \frac{\sqrt{ 2 }}{v}\pi^{+}\bar{t}(m_{t}P_{L}-m_{b}P_{R})b + \mathrm{h.c.},
$$
with $P_{L,R}$ the left and right projectors.
Now, compute the loops 
$$
	\pi^{0} \to t\bar{t}, \bar{b} \to \pi^{0},\qquad \pi^{+}\to t\bar{b}\to \pi^{+},
$$
differentiate and take the difference.
In the limit $m_{t}\gg m_{b}$, we find our final expression 
$$
	\Delta \rho_{f} = \frac{3G_{F}m_{t}^{2}}{8\sqrt{ 2 }\pi^{2}}.
$$
# Goldstone-boson loops

In this case, the relevant terms come from $g'$. We need to calculate the loop diagrams 
$$
	\pi^{3} \to B_{\mu},h\to \pi^{3},\qquad \pi^{1,2}\to \pi^{1,2},B_{\mu}\to \pi^{1,2},
$$
and subtract them. The result goes like 
$$
	\log\left( \frac{m_{h}}{m_{W}} \right) \frac{g'^{2}}{16\pi^{2}}.
$$
Since the term is ~1/1000, LEP was needed for such precise measurements. Moreover, since the logarithm is a slow function, predictions about $m_{h}$ were hard to do using this process.