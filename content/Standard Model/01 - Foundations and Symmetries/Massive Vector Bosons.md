## Historical Motivation
[[Fermi interaction| Fermi's theory]] was highly successful at low energies, but its point-like nature caused probabilities to exceed 100% at high energies. Physicists tried to "UV-complete" the theory by introducing a heavy mediator (the $W$ boson) by hand. This note explains mathematically why simply adding a mass term to a vector field is doomed to fail.

## Proca Lagrangian
If we try to UV-complete Fermi theory by simply introducing a massive charged vector boson ($W^\mu$) by hand, the Lagrangian reads:
$$\mathcal{L}_{W} = \frac{1}{2} W_{\mu \nu}^{+}W_{\mu \nu}^{-} - \frac{1}{2} m_{W}^{2} W_{\mu}^{+}W_{\mu}^{-} + \frac{g}{\sqrt{2}} J_{\mu}^{+}W_{\mu}^{-} + \mathrm{h.c.}$$

> [!math]- Derivation: Propagator Matrix Inversion
> Writing the Lagrangian as $\mathcal{L} = W_{\mu}^{+}K^{\mu \nu}W_{\mu}^{-}$, where $K_{\mu \nu} = -g_{\mu \nu} \Box + \partial_{\mu} \partial_{\nu} - m_{W}^{2} g_{\mu \nu}$, the propagator is its inverse: 
> $$
> D_{\mu \nu}(q) = \frac{-i}{q^{2}-m_{W}^{2}+i\epsilon}\left( g_{\mu \nu} - \frac{q_{\mu}q_{\nu}}{m_{W}^{2}} \right)
> $$

> [!math]- Derivation: Effective Action 
> Integrating out the heavy $W$ field via the path integral:
> 
> $$
> Z = \int \mathcal{D}W\mathcal{D}\bar{\psi}\psi e^{iS} \equiv \int \mathcal{D}\bar{\psi}\psi e^{iS_{\mathrm{eff}}}
> $$
> 
> At leading order ($q^2 \ll m_W^2$), the propagator reduces to $g_{\mu\nu}/m_W^2$, yielding:
> $$
> i S_{\mathrm{eff}} \approx -i \frac{g^{2}}{2 m_{W}^{2}} \int d^{4}x \, J^{+}(x)J^{-}(x)
> $$
> Matching back to Fermi Theory gives the mass scale relation:
> $$
> M_{W}^{2} = \frac{\sqrt{2}}{8} \frac{g^{2}}{G_{F}} \approx (g \times 123 \mathrm{GeV})^{2}
> $$

### High-Energy Scattering
Longitudinal polarization vectors scale like $\epsilon_{\mu}(p) \approx \frac{p_{\mu}}{m_{W}}$ at high energies. If we look at the diagrams
![[feynman_SM_WInteractionQuartic.png|108]] ![[feynman_SM_WInteractionSChannel.png|179]]
then scattering goes like:

$$A \sim \frac{E^4}{m_W^4}$$
From this, we see that the theory loses predictivity and breaks unitarity at energy scales $E > \frac{m_{W}}{\sqrt{g}}$.
