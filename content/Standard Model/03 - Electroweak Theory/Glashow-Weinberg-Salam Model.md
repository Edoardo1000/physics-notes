## Historical Motivation
Before this model, physicists knew that weak interactions required a massive mediator to explain their short range. However, as shown in [[Massive Vector Bosons]], massive spin-1 particles have longitudinal polarization states that cause high-energy scattering amplitudes to grow as $E^2$. 

To tame these divergences, Sheldon Glashow (1961) realized the interactions had to be governed by a local gauge symmetry. He proposed unifying the weak force with electromagnetism under a combined gauge group, which Weinberg and Salam later perfected by adding the Higgs mechanism.

## $SU(2)_L \times U(1)_Y$ Gauge Group
The Standard Model is a **chiral theory** (see [[Spinors and Chiral Theories]]). Left-handed and right-handed fermions transform differently under the weak interaction.

The full gauge group for the electroweak sector is $SU(2)_L \times U(1)_Y$:
* **$SU(2)_L$ (Weak Isospin):** Couples *only* to left-handed fermions. Its gauge bosons are $W^1_\mu, W^2_\mu, W^3_\mu$, and the coupling constant is $g$.
* **$U(1)_Y$ (Weak Hypercharge):** Couples to both left and right-handed fermions. Its gauge boson is $B_\mu$, and the coupling constant is $g'$.

Weak hypercharge $Y$ is defined to bridge the gap between electric charge $Q$ and the third component of weak isospin $T^3_L$ via the **Gell-Mann-Nishijima formula**:
$$
Q = T^{3}_{L} + \frac{Y}{2}
$$

## Field Representations and Quantum Numbers
Using the conjugate basis to write all right-handed fields as left-handed anti-fields, the particle representations under $SU(3)_c \times SU(2)_L \times U(1)_Y$ are:

| Field | $SU(3)_c$ | $SU(2)_L$ | $U(1)_Y$ |
| :--- | :---: | :---: | :---: |
| $Q = (u_L, d_L)^T$ | 3 | 2 | 1/3 |
| $L = (\nu_L, e_L)^T$ | 1 | 2 | -1 |
| $u^c$ (RH Up Quark) | $\bar{3}$ | 1 | -4/3 |
| $d^c$ (RH Down Quark)| $\bar{3}$ | 1 | 2/3 |
| $e^c$ (RH Electron) | 1 | 1 | 2 |

## Unbroken Interaction Lagrangian

Before any mass is generated, the interaction between the fermions and the gauge bosons is dictated strictly by the covariant derivative $D_\mu = \partial_\mu - ig W^a_\mu T^a - ig' B_\mu \frac{Y}{2}$.

The interaction Lagrangian is:
$$
\mathcal{L}_{\mathrm{int}} = g W_{\mu}^{a} J_{\mu}^{a} + g' B_{\mu} J_{\mu}^{Y}
$$
Where the $SU(2)$ currents $J^a_\mu$ act only on the left-handed doublets ($Q_L, L_L$), and the hypercharge current $J^Y_\mu$ acts on everything according to their $Y$ quantum number.

*More on the currents can be found in [[Gauge Boson Mixing and Neutral Currents]].*