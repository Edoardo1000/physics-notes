Particle colliders such as LEP can produce particles with high enough energy to create $Z$ bosons.

The process used in the accelerators is 
$$
	e + \bar{e} \to \mu + \bar{\mu},
$$
which has both an *electromagnetic* and a **weak** channel.
The ratio of the cross sections of the two processes is 
$$
	\frac{\sigma_{\mathrm{weak}}}{\sigma_{\mathrm{QED}}} \sim \frac{G_{F}^{2} s^{2}}{(4\pi\alpha)^{2}}\sim \left( \frac{\sqrt{ s }}{30 \ \mathrm{GeV}} \right)^{4},
$$
from which we know how energetic are the collisions we have to produce in order to see effects of the weak interaction.

# Cross section
 The relevant tree-level Feynman diagrams are the *s-channel photon and $Z$ boson production*. Because of the two contributions, the **differential cross section** is the sum of three terms:
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
From this, we see the usual **Breit-Wigner distribution**.

>[!math]- Derivation of the cross section
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
>Now, it's just a matter of squaring the sum of the amplitudes and using some trace technology (*see [[Gamma Matrices]]*). 
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

For energies less than $m_{Z}$, the **total cross section** is obtained by integrating the differential one, and we get 
$$
	\sigma \approx \frac{4 \pi \alpha^{2}}{3s} \left[ 1 - \frac{4 G_{F} s}{\sqrt{ 2 }e^{2}} g_{V}^{2} + 2 \left( \frac{G_{F}s}{e^{2}} \right)^{2} (g_{V}^{2} + g_{A}^{2})^{2} \right].
$$
**Observation:** from the [[Standard Model Parameter Values]], we see that $g_{V}$ is very small. Thus, the weak contribution to the total cross section is very *difficult to measure*.

**Observation:** In the expression for the total cross section, the contribution from $g_{A}$ is at *second order*. We have to do something else to measure parity violation effects.
 
# Asymmetries 
The total cross section is not enough to determine the single values of $g_{V,f},g_{A,f}$, so we need other observables. Let's define the amplitude 
$$
	A_{f} \equiv \frac{g_{L,f}^{2} - g_{R,f}^{2}}{g_{L,f}^{2}+g_{R,f}^{2}} = \frac{2g_{V,f}g_{A,f}}{(g_{V,f})^{2} + (g_{A,f})^{2}},
$$

We can measure the **moments** of the distribution. For example, I can define the **forward cross section:** 
$$
	\sigma_{F} \equiv \int_{0}^{1} d\cos\theta \ \frac{d\sigma}{d\cos\theta},
$$
and an analogous quantity for the backward cross section.
We can then define:
- **forward-backward asymmetry:**  $$
		A_{\mathrm{FB}} = \frac{\sigma_{F} - \sigma_{B}}{\sigma_{F} + \sigma_{B}}.
	$$
- **left-right asymmetry:**  $$
	  	A_{LR} \equiv \frac{\sigma_{L} - \sigma_{R}}{\sigma_{L} + \sigma_{R}} = A_{e},
	  $$
  where $\sigma_{L,R}$ is the total cross section for a beam with fixed polarization
- **forward-backward-left-right asymmetry:**  $$
  	A_{LR,FB} = \frac{[\sigma_{L} - \sigma_{R}]_{F}-[\sigma_{L}-\sigma_{R}]_{B}}{[\sigma_{L}+\sigma_{R}]_{F}+[\sigma_{L}+\sigma_{R}]_{B}} = \frac{3}{4} A_{f}.
  $$
 Using the cross section we found, we have 
$$
	A_{\mathrm{FB}} \approx - \frac{3G_{F}}{\sqrt{ 2 }e^{2}} g_{A}^{2}.
$$

