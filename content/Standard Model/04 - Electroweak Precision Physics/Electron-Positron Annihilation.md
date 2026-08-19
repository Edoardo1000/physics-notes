Consider the process
$$
	e + \bar{e} \to \gamma^{*} / Z^{*} \to f + \bar{f},
$$
and suppose that the fermions are all massless.
# Tree-level cross section
 The relevant tree-level Feynman diagrams are the s-channel photon and $Z$ boson production. Because of the two contributions, the differential cross section is the sum of three terms:
$$
	\frac{d\sigma}{d \cos\theta}= \frac{\pi \alpha_{\mathrm{em}}^{2}}{2s}[\sigma_{\gamma} + \sigma_{Z}+\sigma_{\gamma Z}],
$$
with 
$$
	\begin{align}
	\sigma_{\gamma}  & = 1+\cos ^{2}\theta, \\
	\sigma_{Z}  & = \lvert \chi(s) \rvert ^{2} [(g_{A}^{2} + g_{V}^{2})^{2}(1 + \cos ^{2}\theta) + 8 g_{V}^{2}g_{A}^{2} \cos\theta],\\
	\sigma_{\gamma Z}  & = 2 \mathrm{Re}\chi(s)[g_{V}^{2}(1+\cos ^{2}\theta) + 2 g_{A}^{2}\cos\theta].
	\end{align}
$$
Here, we defined $\chi(s)$ as  
$$
	\chi(s) = \frac{1}{4 \sin ^{2}\theta_{W} \cos ^{2}\theta_{W}} \frac{s}{s - m_{Z}^{2} + i\Gamma_{Z}m_{Z}}.
$$
From this, we see the usual [[Decay and Optical Theorem#Breit-Wigner distribution|Breit-Wigner distribution]].

>[!math]- Derivation:  the cross section
>the initial electron and positron have momenta $p,p'$ respectively, while the muon and antimuon have momenta $k,k'$. Our calculations are in the massless fermion limit.
>The photon channel amplitude is 
>$$
>A_{\gamma} = i \frac{e^{2}}{s} \bar{v}(p')\gamma^{\mu}u(p) \bar{u}(k) \gamma_{\mu} v^{k'},
>$$
>while the amplitude from the $Z$ exchange is a bit more complicated:
>$$
>A_{Z} = i \frac{e^{2}}{4D_{Z}\sin ^{2}\theta_{W}\cos ^{2}\theta_{W}}\bar{v}(p')\gamma^{\mu}(g_{V}-g_{A}\gamma_{5})u(p) \ \bar{u}(k)\gamma^{\mu}(g_{V} - g_{A}\gamma_{5})v(k'),
>$$
>with $D_{Z} = s - m_{Z}^{2} + i \Gamma_{Z}m_{Z}$.
>Now, it's just a matter of squaring the sum of the amplitudes and using some trace technology (see [[Gamma Matrices]]). 
>For example, in the calculation of $\lvert A_{Z} \rvert^{2}$, we find the factor 
>$$
>\begin{align} & \mathrm{Tr}[\gamma_{\mu}(g_{V}-g_{A}\gamma_{5})\not\!{p} \gamma_{\nu}(g_{V}-g_{A}\gamma_{5}) \not\!{p'}] \\ &= \mathrm{Tr}[\gamma_{\mu} \not\!{p}\gamma_{\nu} \not\!{p'}(g_{V}^{2} + g_{A}^{2} - 2 g_{V}g_{A}\gamma_{5})].\end{align}
>$$
>From this, we find that the amplitude can be written as
>$$
>\lvert A_{Z} \rvert ^{2} = \frac{e^{4}}{64 \lvert D_{Z} \rvert ^{2} \cos ^{4}\theta_{W} \sin ^{4}\theta_{W}}L^{(e)}_{\mu \nu}L_{(\mu)}^{\mu \nu},
>$$
>where $$ L_{\mu \nu} = 4(g_{V}^{2}+ g_{A}^{2})[p_{\mu} p'_{\nu} + p_{\nu} p'_{\mu} - pp' \eta_{\mu \nu }] + 8i g_{V} g_{A} \epsilon_{\mu \alpha \nu  \beta} p^{\alpha} p'^{\beta}. $$
>The cool thing is that symmetric and antisymmetric parts of these tensors do not mix.
>We then contract the tensors, and making use of the identities
>$$
>p \cdot k = p' \cdot k' = \frac{s}{4}(1 - \cos\theta), \quad p \cdot k' = p' \cdot k = \frac{s}{4}(1 + \cos \theta),
>$$
>we arrive at our desired result. 
>The case of the interference term is analogous.

For energies less than $m_{Z}$, the total cross section is obtained by integrating the differential one, and we get 
$$
	\sigma \approx \frac{4 \pi \alpha^{2}}{3s} \left[ 1 - \frac{4 G_{F} s}{\sqrt{ 2 }e^{2}} g_{V}^{2} + 2 \left( \frac{G_{F}s}{e^{2}} \right)^{2} (g_{V}^{2} + g_{A}^{2})^{2} \right].
$$
**Observation:** from the [[Standard Model Parameter Values]], we see that $g_{V}$ is very small. Thus, the weak contribution to the total cross section is very *difficult to measure*.

**Observation:** In the expression for the total cross section, the contribution from $g_{A}$ is at *second order*. We have to do something else to measure parity violation effects.
# One-loop level cross section
At one-loop level, the leading contribution to the cross section near the $Z$ pole is given by
$$
	\sigma(s)_{e e \to ff} \approx \frac{12\pi}{m_{Z}^{2}}\Gamma_{e} \Gamma_{f} \frac{s}{(s-m_{Z}^{2})^{2} + m_{Z}^{2}\Gamma_{Z}^{2}},
$$
where 
$$
	\Gamma_{f} = 4N_{c} \Gamma_{0} [(g^{eff}_{V,f})^{2} R_{V}+ (g^{eff}_{A,f})^{2}R_{A}], \quad \Gamma_{0} = \frac{G_{F}m_{Z}^{2}}{24\pi \sqrt{ 2 }},
$$
$N_{c}$ is the number of colors of the fermion, and $R_{V}$ and $R_{A}$ are functions encoding QCD and QED radiative corrections.

Here, $g_{V}^{eff}$ and $g_{A}^{eff}$ are the [[Effective EW parameters|effective couplings]] at one-loop level.