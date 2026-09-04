Due to the [[Higgs Boson Interactions|interactions of the Higgs boson]], several [[Decay and Optical Theorem|decay]] channels are possible. Here we list some with their widths
# Summary of branching ratios

The various branching ratios of the Higgs boson are summarized in the following picture.

![[../assets/higgs_branching_ratios.svg|593]]

**Observation:** Contrary to what one could expect, $h$ can decay in $W,Z$ even at $m_{h}<2m_{W}$. In this case, one of the particles can be virtual, so instead of a hard cutoff we have a suppression due to the $\frac{1}{m_{W}^{2}}$ in the propagator.
**Observation:** At large $m_{h}$, the decay is dominated by $W$ and $Z$ bosons. Precisely, their longitudinal modes. Moreover, they are in the ratio $2:1$. This can be understood using the equivalence at high energy between the Goldstone modes and the longitudinal vectors: two of them are eaten by the $W^{\pm}$, while just one by the $Z$. 
# Decay into fermions
The width for the decay $h\to f + \bar{f}$ is given by 
$$
	\Gamma(h\to \bar{f}f)=\frac{m_{f}^{2}}{v^{2}}m_{h}\left( 1-\frac{4m_{f}^{2}}{m_{h}^{2}} \right)^{3/2} \frac{N_{c}}{8\pi}.
$$
>[!math]- Derivation: decay width for fermions
>Looking at the interactions with fermions, the amplitude is given by (after averaging over polarizations)
>$$
>\lvert A \rvert ^{2} = \frac{m_{f}^{2}}{v^{2}}\mathrm{Tr}[(\not\!{p_{f}}-m_{f})(\not\!{p}_{\bar{f}}+m_{f})] = \frac{2m_{f}^{2}}{v^{2}}(m_{h}^{2}-4m_{f}^{2}).
>$$
>Multiply by the phase space element of two particles with the same mass, and the result is obtained
# Decay into bosons
In this case, for a vector boson $V$, let $x_{V} \equiv \frac{m_{V}^{2}}{m_{h}^{2}}$. Then, we have 
$$
	\begin{align}
	\Gamma(h\to W^{+}W^{-})  & = \frac{m_{h}^{3}}{16\pi v^{2}}\sqrt{ 1 - 4x_{W} }(1 - 4x_{W} + 12x_{W}^{2})  \\
	\Gamma(h\to Z Z)  & = \frac{m_{h}^{3}}{32\pi v^{2}}\sqrt{ 1 - 4x_{Z} }(1 - 4x_{Z} + 12x_{Z}^{2})  \\
	
	\end{align}
$$

>[!math]- Derivation: decay width for vector bosons
>The relevant interaction is the cubic one. The vertex $hVV$ for a vector $V$ gives an amplitude 
>$$
>2i\frac{m_{V}^{2}}{v}g_{\mu \nu}
>$$
>The tree-level amplitude of the decay is thus 
>$$
>iA = i \frac{2m_{V}^{2}}{v}\epsilon_{\lambda_{1}}^{*}(p_{1}) \epsilon_{\lambda_{2}}^{*}(p_{2}),
>$$
>with $\lambda_1, \lambda_2$ the polarizations of the outgoing vectors.
>Averaging over polarizations, and using the polarization sum, we find 
>$$
>\lvert \bar{A} \rvert^{2} = \frac{4m_{V}^{4}}{v^{2}}\left[ 2 + \frac{(p_{1} \cdot p_{2})^{2}}{m_{V}^{4}} \right] = \frac{m_{h}^{4}}{v^{2}}(1 - 4x_{V} + 12x_{V}^{2})
>$$
>From this, the result is pretty straightforward. Pay attention that *the phase space of the $Z$ bosons has a factor of $1 / 2$ since the particles are identical*.

>[!math]- Derivation: alternative method using equivalence principle
>In this case, I can just write 
>$$
>H^{\dagger} H = \frac{(v+h)^{2}}{2} + \frac{\phi^{0}}{2} + \phi^{+}\phi^{-},
>$$
>so that the potential contains the term 
>$$
>(v+h)^{2}\left( \phi^{+}\phi^{-} + \frac{(\phi^{0})^{2}}{2} \right),
>$$
>which implies a cubic vertex with factor
>$$
>- 2i \lambda v = - i \frac{m_{h}^{2}}{v}.
>$$
>From this, we see immediately that the amplitude goes like 
>$$
>\Gamma(h\to W^{+}W^{-}) \approx \Gamma(h\to \phi^{+}\phi^{-}) = \frac{\frac{1}{2m_{h}}m_{h}^{4}}{v^{2}} \frac{1}{8\pi} = \frac{m_{h}^{3}}{16 \pi v^{2}}.
>$$

---
**Observation:** we see that 
	- decay in fermions goes like $\frac{m_{f}^{2}}{v^{2}}m_{h}$
	- decay in bosons goes like $\frac{m_{h}^{2}}{v^{2}}m_{h}$
	this is related to the fact that the longitudinal polarization is proportional to $p$.
From this we observe that **the decay in two vector bosons is much more sensible on the mass of the Higgs boson**.

# One-loop decay channel

![[../assets/h_photon_loop_diagram.svg|181]]

While Higgs boson does not couple directly to gluons and photons, it can still couple to them through vector and boson loops.
The leading contributions to gluon decay comes from a top quark loop, and the decay width can be computed: 
$$
	\Gamma(h\to g g) = \frac{\alpha^{2}m_{t}^{3}}{256 \pi^{3} v^{2}} \left\lvert  f\left( \frac{m_{t}^{2}}{m_{h}^{2}} \right)  \right\rvert^{2},
$$
where $f$ is the function coming from the loop calculation.

The key idea is that $h$ generates a left and a right fermion line, which have to be connected to close the loop. Since gluons do not change chirality, an operator $m_{t}\bar{t}_{L} t_{R}$ must appear inside the loop. Because of this, the amplitude must go like 
$$
A \sim \frac{\alpha}{4\pi} Y_{t} m_{t} f\left( \frac{m_{t}^{2}}{m_{h}^{2}} \right).
$$

## Decay at low energy
The decay into photons in the limit $m_{t}\gg m_{h}$ can be studied using a trick: the **low-energy theorem**.
### Low-energy theorem
The theorem states the following identity between scattering amplitudes:
$$
	\lim_{ p_{h} \to 0 } A(X\to Y + h) = \sum_{i} \frac{m_{i}}{v} \frac{\partial}{\partial m_{i}} A(X\to Y).
$$
This theorem is related to the fact that *the mass of all the particles is proportional to $\langle H \rangle$*.

Using this theorem, it is now easy to show that the amplitude of the process is given by 
$$
	A(h\to\gamma+\gamma) \approx \frac{\beta_{\mathrm{em}}}{\alpha} \frac{1}{v}, \quad \beta_{\mathrm{em}}= \frac{2\alpha^{2}}{3\pi}Q_{t}^{2}.
$$
>[!math]- Derivation: Higgs decay amplitude
>We use the low-energy theorem applied to the amplitude $\gamma \to \gamma$. The amplitude at one-loop level is given by
>$$
>\hat{\Pi}_{\gamma\gamma}(0) = -\frac{\alpha Q^{2}}{3\pi}\log\left( \frac{\mu^{2}}{m^{2}} \right).
>$$
>Applying the theorem, we have
>$$
>A(h\to\gamma+\gamma) \approx \frac{m_{t}}{v} \frac{\partial}{\partial m_{t}}\hat{\Pi}_{\gamma\gamma}(0),
>$$
>from which the result follows.

### EFT for the $h$-photon interaction
In general, the decay of the Higgs boson in photons can be described using an effective Lagrangian. The term is given by 
$$
	\mathcal{L}_{\mathrm{eff}} = \frac{1}{4}\frac{\beta(\alpha)}{\alpha} \frac{h}{v} F_{\mu \nu}F^{\mu \nu}.
$$
*Note*: this operator is not gauge-invariant, one should look at the full invariant dimension-6 operator. Examples of such operators are 
$$
	H^{\dagger}H \ B_{\mu \nu}B^{\mu \nu},\quad H^{\dagger}H \ W_{\mu \nu}^{a}W^{\mu \nu}_{a},\quad H^{\dagger} \sigma^{a} H \ W_{\mu \nu}^{a}B^{\mu \nu}.
$$

>[!math]- Derivation: Effective Lagrangian
>The effective Lagrangian is obtained by integrating out the fermions and the exact expression will be nonlocal in general, we can write its quadratic term as 
>$$
>\mathcal{L}^{(2)}_{\mathrm{eff}} = \frac{1}{2} \int \frac{d^{4}q}{(2\pi)^{4}}A_{\mu}(-q)[q^{2}g^{\mu \nu}-q^{\mu \nu }](1+\hat{\Pi}_{\gamma\gamma}(q^{2}))A_{\nu}(q),
>$$
>the first piece corresponds to the kinetic term:
>$$
>-\frac{1}{4} \int d^{4}x F_{\mu \nu}F^{\mu \nu} = \frac{1}{2} \int \frac{d^{4}q}{(2\pi)^{4}} A_{\mu}(-q)[q^{2}g^{\mu \nu}-q^{\mu}q^{\nu}]A_{\nu}(q).
>$$
>Thus, $\Pi_{\gamma\gamma}(0)$ corresponds to a correction to the kinetic term. Now, if the propagator depends on the mass of a fermion $m(h) = m(1 + \frac{h}{v})$, we can expand and get 
>$$
>\begin{align} \mathcal{L}_{\mathrm{eff}}^{(2)}  & = -\frac{1}{4}[1 + \Pi_{\gamma\gamma}(0,m(h))] F_{\mu \nu}F^{\mu \nu} \\  & \supset -\frac{1}{4} \left[ \frac{m}{v} \frac{\partial}{\partial m} \hat{\Pi}_{\gamma\gamma}(0,m) \right]h F_{\mu \nu}F^{\mu \nu}\end{align},
>$$
>from which the result follows.


