We know that, since the electromagnetic coupling $\alpha_{\mathrm{em}}$ runs under a **renormalization** group flow, its value differs between experiments at high and low, energies. In particular, we have 
$$
	\alpha_{\mathrm{em}}(q^{2} = 0) \approx \frac{1}{137},\quad \alpha_{\mathrm{em}}(q^{2} =  m_{Z}^{2}) \approx \frac{1}{127}.
$$
We must know its value in order to compare theory with weak experiments. We already know its **running**: 
$$
	\alpha_{\mathrm{em}}(q^{2}) = \frac{\alpha_{\mathrm{em}}(0)}{1 - \Delta \alpha_{\mathrm{em}}(q^{2})},
$$
where $\Delta \alpha_{\mathrm{em}}$ is found from the loop contributions to the photon propagator.
The problem is that QCD contributions are too difficult to calculate, so we must use some other methods other than perturbative ones.

# Photon propagator
The leptonic contributions are known perturbatively with a very high precision. The problem comes from **hadronic contributions**, which are nonperturbative. We write the propagator as 
$$
	D_{\mu \nu}(q^{2}) = \left( \eta^{\mu \nu}q^{2} - \frac{q^{\mu}q^{\nu}}{q^{2}} \right) \Pi(q^{2}), \quad \Pi(q^{2}) = \Pi^{\mathrm{lep}}(q^{2}) + \Pi^{\mathrm{had}}(q^{2}),
$$
where we separated the leptonic and hadronic contributions. We are interested in finding the hadronic part.

The key idea is the hypothesis that the propagator is an **analytic function** of the variable $q^{2}$. This, along with the **optical theorem**, permits us to find an expression for the propagator.
Our final result for the running of the fine structure constant is 
$$
	\Delta \alpha_{\mathrm{em}}(q^{2}) = \frac{\alpha}{3\pi} q^{2} \mathcal{P}\int_{4m_{\pi}^{2}}^{\infty} \frac{R_{h}(s)}{s(s-q^{2})}ds,
$$
with 
$$
	R_{h}(s) \equiv \frac{3}{\alpha} \mathrm{Im}\Pi(s) = \frac{3s}{4\pi\alpha^{2}}\sigma(e \bar{e}\to \mathrm{had.}).
$$
>[!math]- Derivation of the running of $\alpha$
>From the optical theorem we know that
>$$ \mathrm{Im}\Pi(s) = \sum_{\mathrm{state}} \lvert A(\gamma \to \mathrm{state}) \rvert ^{2}. $$
>The pion is the lightest hadron which can be produced from a photon. From this, we deduce that for $s > 4m_{\pi}^{2}$ (corresponding to $\gamma \to \pi^{+}\pi^{-}$), the propagator has a nonzero imaginary part. This, with the fact that $f(\bar{z}) = \bar{f}(z)$ for a generic analytic function, implies that the propagator has a branch cut on the real line starting from $4m_{\pi}^{2}$, and $f(x+i\epsilon) - f(x-i\epsilon) = 2i \mathrm{Im}f(x)$.
>Now, we use the *residue theorem*: integrate along a counter-clockwise curve which goes at infinity and around  the branch cut, we get 
>$$ \oint \frac{\Pi(s)}{s(s-q^2)}ds = 2\pi i \left( \frac{\Pi(0)}{-q^{2}} + \frac{\Pi (q^{2})}{q^{2}} \right) \equiv \frac{2\pi i}{q^{2}} \Delta \Pi(q^{2}).$$
>The quantity $\Delta \Pi^{2}$ is exactly what we are looking for.  The integral along the contour line is given by 
>$$ \int_{4m_{\pi}^{2}+i\epsilon}^{\infty+i\epsilon} \frac{\Pi(s)}{s(s-q^{2})} - \int_{4m_{\pi}^{2}-i\epsilon}^{\infty-i\epsilon} \frac{\Pi(s)}{s(s-q^{2})} = \int_{4m_{\pi}^{2}}^{\infty } \frac{2i\mathrm{Im}\Pi(s)}{s(s-q^{2})}ds,$$
>and we know the imaginary part of the propagator from the optical theorem: 
>$$ \mathrm{Im}\Pi(s) = \frac{s}{4\pi \alpha}\sigma(e \bar{e}\to \mathrm{had.}) \equiv \frac{\alpha}{3}R_{h}(s).$$
>We are almost done, the only problem is that the integral presents a pole at $s = q^{2}$. In order to cure that, we take the principal part, and the main result is obtained.

The cause of the lower precision in the value of the coupling at high energy is thus $R_{h}(s)$, which is known with much less accuracy.