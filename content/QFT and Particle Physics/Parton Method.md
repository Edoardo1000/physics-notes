---
tags:
  - status/to-do
---
Suppose you want to calculate the process 
$$
	f + \bar{f} \to f + X,
$$
where $X$ is a possible final product of the reaction, and also suppose that the process originates from $f$ **emitting a vector boson** $V$.

The trick is to treat $V$ as a **parton**.
Now, the idea is that we can write the amplitude as 
$$
\begin{align}
 A  & = J_{\mu} A_{\nu} \frac{g_{\mu \nu}}{q^{2}-m_{V}^{2}}  \\
  & = \frac{J_{\mu}}{q^{2}-m_{V}^{2}} \sum_{\lambda} \epsilon^{\mu}_{\lambda}\epsilon_{\lambda}^{\nu}A_{\nu}  \\
  & = \sum_{\lambda}\frac{J_{\mu}\epsilon^{\mu}_{\lambda}}{q^{2}-m_{V}^{2}}A(V_{\lambda}+\bar{f}\to X),
\end{align}
$$
where $\lambda$  runs over the possible vector polarizations, and $V_{\lambda}$ is the vector boson with fixed polarization.
From this, the cross section for fixed polarization emission is
$$
	\sigma_{\lambda} = \int E\frac{dE}{8\pi^{2}} \frac{q^{0}}{E_{f}} \frac{\lvert J_{\mu}\epsilon^{\mu}\rvert^{2}}{[-2E_{f}E'_{f}(1-\cos\theta)-m_{V}^{2}]}\hat{\sigma} d\cos\theta,
$$
where 
$$
	\hat{\sigma} \equiv  \lvert A(V_{\lambda}+\bar{f}\to X) \rvert^{2}.
$$
The main idea is then to use the **effective vector approximation**: In the expression of $\hat{\sigma}$, the vector $V$ possesses momentum $q^{\mu} = (q^{0},\vec{q}_{T},q_{L})$, and is off-shell. We ignore the transverse momentum and pretend that $V$ is in fact an on-shell physical particle.
*The approximation is valid as long as the main contribution to the cross section comes from collinear vectors, which is the case for very energetic fermions.*
### Longitudinal case
In this case, if the vector was massless, there would be an infrared divergence.
Expanding in $m_{V}^{2}$, and integrating in $d \cos\theta$, we find
$$
	\sigma_{L} \approx \int dx f_{L}(x)\hat{\sigma},\quad f_{L}(x) = \frac{g^{2}}{16\pi^{2}} \frac{1-x}{x},
$$
$f_{L}(x)$ is called the **splitting function**. Physically, it tells us how probable it is to spit out a vector boson with energy $x \cdot E$.


**Something in the derivation is wrong, please correct**

>[!math]- Derivation: Longitudinal splitting function
>Take the expression for $\sigma_\lambda$. Using changing coordinates to
>$$
>Q^{2} = -q^{2} = 2E E_{f} \cos\theta, \quad q^{0} = x E_{f}, \quad E = E_{f}(1-x),
>$$
>the expression for $\sigma_\lambda$ becomes
>$$
>\sigma_{\lambda} = \frac{m_{V}^{2}}{4\pi^{2}}\int_{0}^{1}dx \frac{1-x}{x} \hat{\sigma} \int_{0}^{\mu_{F}} \frac{1}{Q^{2}-m_{V}^{2}} dQ^{2}.
>$$
>In the second integral, we introduced the **factorization scale** $\mu_F$ (see the following sections for its significance).
>Evaluating the integral 
>$$
>\int dQ^{2} \frac{1}{Q^{2} + m_{V}^{2}} \sim \frac{1}{m_{V}^{2}},
>$$
>and restoring a $g^2$ factor (depending on the convention), we find our formula.
### Transverse case
In this case, the splitting function has a **physical infrared divergence**: 
$$
	f_{T}(x) = \frac{g^{2}}{4\pi^{2}} \log\left( \frac{\mu_{F}^{2}}{m_{V}^{2}}\right) \frac{x^{2}+2x(1-x)}{x},
$$
where $\mu_{F}$ is a scale which was introduced to cut off the contributions of the amplitude coming from the region of high transverse momentum.

## The factorization scale
In the derivation of the longitudinal splitting function, a **factorization scale was introduced**. This is because we made the *collinear approximation*, in which the transverse momentum of the vector boson is considered negligible.
However, the full calculation of the cross section involves integrating on a region of high transverse momentum, which breaks down the collinear approximation.

Because of this, we *cut* *off the integral* at a certain scale. In a typical experiment, this scale is some characteristic scale of the system. Refining our analysis, we could also try to study the dependence of $\hat{\sigma}$ on the factorization scale. The dependence should cancel the one of the splitting function, since the physics cannot depend on this scale. Staying at lowest order, we accept a dependence on the cutoff scale, meaning that the calculation is just a *coarse approximation* of the true process
# Infrared divergences
Depending on the theory we are studying, there are different regulators which prevent the logarithm from blowing up:
- **EW:** the vector bosons' masses;
- **QCD:** we have $\Lambda_{QCD}$, below that threshold the theory is nonperturbative;
- **QED with massive fermions**:  we have  $m_{e}$, in this case $t=-\frac{s}{2}(1-\cos\theta) + 2m_{e}^{2}$ does not diverge;
- **QED with massless fermions:** in this case the theory does not make any sense. If we look at the spectral density, the pole at the origin an the multiparticle state branch cut touch each other.