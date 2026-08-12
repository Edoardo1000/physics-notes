---
tags:
  - topic/electroweak
  - topic/standard-model
---
## Charged and Neutral Gauge States
From the [[Glashow-Weinberg-Salam Model#Unbroken Interaction Lagrangian|Unbroken Interaction Lagrangian]], we can reorganize the $SU(2)_L$ fields $W^1, W^2$ into physically observable **charged currents**:
$$
\mathcal{L}_{\mathrm{cc}} = \frac{g}{\sqrt{2}}(J_{\mu}^{-}W_{\mu}^{+}+ J_{\mu}^{+}W^{-}_{\mu}), \quad J^-_{\mu} = \bar{\nu}_{L} \gamma_{\mu}e_{L}+ \bar{u}_{L}\gamma_{\mu}d_{L},\quad J^{+}_{\mu}  = (J^{-}_{\mu})^{\dagger},
$$
with 
$$
	W_{\mu}^{\pm} = \frac{1}{\sqrt{ 2 }}(W^{1}_{\mu} \mp W_{\mu}^{2}).
$$
>[!warning]- A note on convention
>We use this convention because the signs reflect the *electric charges of the operators*. Indeed, with this convention we can write 
>$$
>W_{\mu} = W_{\mu}^{a}T^{a} = \frac{1}{\sqrt{ 2 }}T^{+}W_{\mu}^{+} + \frac{1}{\sqrt{ 2 }} T^{-}W_{\mu}^{-} + W_{\mu}^{3} T^{3},
>$$
>and the electric charge becomes apparent when looking at $Q = T^3 + Y/2$. For the bosons we have $Y=0$, and 
>$$
>[T^{3}, T^{\pm}] = \pm T^{\pm}.
>$$
>For the currents, the convention is the same: **we look at the electric charge**.

>[!math]- Derivation: Charged current Lagrangian
>Let's just look at the lepton part. We write the interaction Lagrangian as 
>$$
>\begin{align}
>\mathcal{L}  & = - i\frac{g}{2} (W_{\mu}^{1}\bar{L}_{L}\gamma^{\mu}T^{1}L_{L} + W_{\mu}^{2}\bar{L}_{L}\gamma^{\mu}T^{2}L_{L}) \\
> & = -i \frac{g}{\sqrt{ 2 }} (W_{\mu}^{+}\bar{L}_{L} \gamma^{\mu}\sigma^{+} L_{L} + W_{\mu}^{-}\bar{L}_{L} \gamma^{\mu}\sigma^{-} L_{L})
>\end{align},
>$$
>with $\sigma^{\pm} = \frac{1}{2}(\sigma^1 \pm \sigma^2)$, which is the result we were looking for (Pay attention to the sign convention above).

## Weinberg Rotation
The physical neutral bosons $A_\mu$ and $Z$ are linear combinations of $W^3_\mu$ and $B_\mu$. They are rotated by the **Weinberg angle** ($\theta_W$):
$$
\begin{align}
A_{\mu} & = \sin \theta_{W} W^{3}_{\mu} + \cos \theta_{W} B_{\mu} \\
Z_{\mu} & = \cos \theta_{W} W^{3}_{\mu} - \sin \theta_{W} B_{\mu}
\end{align}
$$
The angle is found by *requiring that $A_{\mu}$ is the physical photon*. The **neutral current Lagrangian** then becomes 
$$
	\mathcal{L}_{nc} = -ie A_{\mu}J_{\mu}^{\mathrm{em}} - i \frac{g}{\cos \theta_{W}}Z_{\mu}J^{nc}_{\mu},
$$
with 
$$
	J_{\mu}^{em} = \sum_{\psi} \bar{\psi}\gamma_{\mu}Q\psi,\quad J_{\mu}^{nc} = \sum_{\psi}\bar{\psi}(T^{3}-\sin ^{2}\theta_{W} Q)\psi,
$$
where the sum runs over both left and right fermions, and $T^{3}$ is zero for right fermions.

>[!note] Note on the angle convention
>Usually, $\sin\theta_W$ and $\cos\theta_W$ are denoted by $s_W,c_W$.

> [!math]- Derivation: Neutral current Lagrangian
> We start from the neutral piece of the interaction Lagrangian:
> $$
> \mathcal{L}_{nc} = -ig J^{3}_{\mu} W_{\mu}^{3} - ig' J_{\mu}^{Y}B_{\mu}
> $$
> By substituting $W^3$ and $B$ in terms of $A$ and $Z$, and forcing the coefficient of the photon field $A_\mu$ to match the electromagnetic current $e J^{\text{em}}_\mu = e(J^3_\mu + J^Y_\mu)$, we find:
> $$
> e = g \sin\theta_W = g' \cos\theta_W.
> $$
> With this relation, we can rearrange the $Z$ boson coupling into:
> $$
> \mathcal{L}_{nc} = - i e A_{\mu} J_{\mu}^{\mathrm{em}} - i \frac{g}{\cos \theta_{W}} Z_{\mu} (J^{3}_{\mu} - \sin ^{2} \theta_{W}J_{\mu}^{\mathrm{em}}).
> $$

## Experimental Discovery: Gargamelle (1973)
Because the $Z$ boson couples to the neutral current $J^3_\mu$, the model predicts weak interactions that do not exchange electric charge. Before 1973, these had never been seen.

Researchers at CERN used the *Gargamelle* bubble chamber to search for this. They fired a muon neutrino ($\nu_\mu$) beam (produced by decaying $\pi^\pm$) into a gas target:
* **Charged Current Background:** $\nu_{\mu} + e^{-} \to \mu^{-} + \nu_{e}$
* **Neutral Current Signal:** $\nu_{\mu} + e^{-} \to \nu_{\mu} + e^{-}$

To prove the neutral current existed, they had to detect isolated electrons being knocked forward without any muons being produced. They successfully found these tracks, proving Glashow's $Z$ boson mixing years before the $Z$ boson itself was directly synthesized.

# Symmetry breaking
What we did so far *did not require bosons to be massive*. All this, however, seems arbitrary if we do not take into account how [[Electroweak Mass Generation|the mass of the vector bosons]] gets implemented via the [[Higgs Mechanism|Higgs mechanism]]. After spontaneous symmetry breaking, **the photon is the only vector who remains massless**.