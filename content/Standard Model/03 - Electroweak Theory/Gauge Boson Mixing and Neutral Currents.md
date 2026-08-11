## Charged and Neutral Gauge States
From the [[Glashow-Weinberg-Salam Model#Unbroken Interaction Lagrangian|Unbroken Interaction Lagrangian]], we can reorganize the $SU(2)_L$ fields $W^1, W^2$ into physically observable **charged currents**:
$$
\mathcal{L}_{\mathrm{cc}} = \frac{g}{\sqrt{2}}(J_{\mu}^{+}W_{\mu}^{-}+ J_{\mu}^{-}W^{+}_{\mu}), \quad J^{\pm}_{\mu} = \bar{Q}_{L} \gamma_{\mu} \sigma^{\pm}Q_{L} + \bar{L}_{L} \gamma_{\mu} \sigma^{\pm}L_{L}
$$

This leaves two electrically neutral gauge bosons: $W^3_\mu$ (from $SU(2)_L$) and $B_\mu$ (from $U(1)_Y$). However, neither of these is the photon. In order to recover standard electromagnetism, these two fields must mix.

##  Fermi's interaction
By expanding the interaction vertex for a [[Massive Vector Bosons|massive vector]], we find the old Fermi theory.

## Weinberg Rotation
The physical neutral bosons—the massless photon ($A_\mu$) and the massive $Z$ boson ($Z_\mu$)—are orthogonal linear combinations of $W^3_\mu$ and $B_\mu$. They are rotated by the **Weinberg angle** ($\theta_W$):
$$
\begin{align}
A_{\mu} & = \sin \theta_{W} W^{3}_{\mu} + \cos \theta_{W} B_{\mu} \\
Z_{\mu} & = \cos \theta_{W} W^{3}_{\mu} - \sin \theta_{W} B_{\mu}
\end{align}
$$

> [!math]- Derivation: Expanding the Neutral Current
> Starting from the neutral piece of the interaction Lagrangian:
> $$
> \mathcal{L}_{\mathrm{neutral}} = -ig J^{3}_{\mu} W_{\mu}^{3} - ig' J_{\mu}^{Y}B_{\mu}
> $$
> By substituting $W^3$ and $B$ in terms of $A$ and $Z$, and forcing the coefficient of the photon field $A_\mu$ to match the electromagnetic current $e J^{\text{em}}_\mu = e(J^3_\mu + J^Y_\mu)$, we find:
> $$
> e = g \sin\theta_W = g' \cos\theta_W
> $$
> We can rearrange the $Z$ boson coupling into:
> $$
> \mathcal{L}_{\mathrm{neutral}} = - i e A_{\mu} J_{\mu}^{\mathrm{em}} - i \frac{g}{\cos \theta_{W}} Z_{\mu} (J^{3}_{\mu} - \sin ^{2} \theta_{W}J_{\mu}^{\mathrm{em}})
> $$

Thus, **electromagnetism and the weak force are unified** under the same coupling constants. The Lagrangian for the neutral current is thus 
$$
	\mathcal{L}_{nc} = -ie A_{\mu}J_{\mu}^{\mathrm{em}} - i \frac{g}{\cos \theta_{W}}Z_{\mu}J^{nc}_{\mu}.
$$
*More about the interaction can be found in [[Electron - Neutrino Scattering]]*.

## Experimental Discovery: Gargamelle (1973)
Because the $Z$ boson couples to the neutral current $J^3_\mu$, the model predicts weak interactions that do not exchange electric charge. Before 1973, these had never been seen.

Researchers at CERN used the *Gargamelle* bubble chamber to search for this. They fired a muon neutrino ($\nu_\mu$) beam (produced by decaying $\pi^\pm$) into a gas target:
* **Charged Current Background:** $\nu_{\mu} + e^{-} \to \mu^{-} + \nu_{e}$
* **Neutral Current Signal:** $\nu_{\mu} + e^{-} \to \nu_{\mu} + e^{-}$

To prove the neutral current existed, they had to detect isolated electrons being knocked forward without any muons being produced. They successfully found these tracks, proving Glashow's $Z$ boson mixing years before the $Z$ boson itself was directly synthesized.