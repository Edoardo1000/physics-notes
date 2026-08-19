The Standard Model is probably the effective low-energy description of some UV theory which we do not know yet. We can try to look at operators with dimension greater than $4$:
- there is **exactly one dimension-5 operator**;
- there are **2499 dimension-6 operators**, 59 if we consider only one flavor.

This is nice, since it means there are many possible observables that I can measure. For example, there are the operators 
$$
	\begin{align}
	\mathcal{O}_{W}  & = D_{\mu}W_{\mu \nu}^{a}(H^{\dagger}D_{\nu}T^{a}H); \\
	\mathcal{O}_{B}  & = \partial_{\mu}B_{\mu \nu}(H^{\dagger} D_{\nu}H); \\
	\mathcal{O}_{WW}  & = (D_{\mu}W_{\mu \nu})^{2}; \\
	\mathcal{O}_{BB}  & = (\partial_{\mu}B_{\mu \nu})^{2}; \\
	\mathcal{O}_{T}  & = \lvert H^{\dagger}D_{\mu}H \rvert ^{2}; \\
	\mathcal{O}_{H} &  = \frac{1}{2} [\partial_{\mu}(H^{\dagger}H)]^{2}
	\end{align}
$$
All of these give corrections to the [[Extensions of the Standard Model|new physics parameters]]: 
$$
	\begin{align}
	S &  = (c_{W} + c_{B})v^{2}; \\
	T & = c_{T}v^{2};  \\
	W & = c_{WW}v^{2};  \\
	Y & = c_{BB}v^{2}.
	\end{align}
$$
### Contributions to $S$

For example, for $S$, there is a contribution from $\mathcal{O}_{W},\mathcal{O}_{B}$, which take the form 
$$
	\delta S = (c_{B}+c_{W}) \frac{v^{2}}{\Lambda^{2}}.
$$
However, operators such as $\mathcal{O}_{H}$ contribute to the parameter indirectly. This is because $\mathcal{O}_{H}$ modifies the Higgs boson kinetic term. If we canonically normalize, we get 
$$
	h\to h\left( 1 - \frac{v^{2}}{\Lambda^{2}}c_{H} \right)^{1/2} \approx h\left( 1 - \frac{v^{2}}{\Lambda^{2}} \frac{c_{H}}{2} \right).
$$
This in turn changes the interactions: 
$$
	Y \bar{\psi}_{L}\psi _{R}H \to Y \left( 1-\frac{c_{H}}{2} \frac{v^{2}}{c_{H}^{2}} \right)\bar{\psi}_{L} \psi_{R}h,\quad W_{\mu}^{+}W_{\mu}^{-}hg^{2}v\to g^{2}v\left( 1-\frac{c_{H}}{2} \frac{v^{2}}{\Lambda^{2}} \right)W_{\mu }^{+}W_{\mu}^{-}h.
$$
In particular, loops in the $B-W^{3}$ two-point function containing a Higgs get modified. The divergent part of $S$ becomes
$$
	S_{\mathrm{div}} = \frac{v^{2}}{\Lambda^{2}}\left[ \delta c_{B} + \delta c_{W} + \frac{g^{2}}{16\pi^{2}}c_{H} \frac{A}{\epsilon} \right],
$$
with $A$ some constant. Note that this result is valid in the convention $\mathcal{L} = -\frac{1}{4g^{2}}W_{\mu \nu}W^{\mu \nu}$. Thus, finiteness of $S$ gives an equation for $\delta c_{B} + \delta c_{W}$. 

Thus, we find 
$$
	S = \frac{v^{2}}{\Lambda^{2}}\left[ c_{B}(\mu) + c_{W}(\mu) + \frac{g^{2}}{16\pi^{2}}\log \frac{\mu^{2}}{m_{h}^{2}} + \dots\right].
$$
### Contributions to $T$

Let's look at how $T$ changes. We have a contribution at tree-level coming from $\mathcal{O}_{T}$: 
$$
	T_{\mathrm{tre e}} \sim c_{T} \frac{v^{2}}{\Lambda^{2}}.
$$
Notice that $\mathcal{O}_{T}$ changes only the neutral propagator, not the charged one.
Moreover, loops involving $hBW$ get modified again due to $\mathcal{O}_{H}$. If the Standard Model loops canceled, they do not anymore, and we have a divergence, 
$$
	\delta T_{\mathrm{loop}} \sim \frac{g'^{2}}{16\pi^{2}}c_{H} \frac{v^{2}}{\Lambda^{2}}\left[ \frac{1}{\epsilon} + \log \frac{\mu^{2}}{m_{h}^{2}} + \dots  \right].
$$
Note that $g'$ appears since $T$ is related to custodial symmetry breaking, and $g'$ explicitly breaks custodial symmetry. We then use $\delta c_{T}$ to cancel the divergence, and we find 
$$
	T = c_{T}(\mu) \frac{v^{2}}{\Lambda^{2}} + A_{T} \frac{g'^{2}}{16\pi^{2}}c_{H}(\mu) \frac{v^{2}}{\Lambda^{2}} \log \frac{m_{h}^{2}}{\mu^{2}} + \dots.
$$