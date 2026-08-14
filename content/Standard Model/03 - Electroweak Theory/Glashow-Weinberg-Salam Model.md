---
tags:
  - topic/electroweak
  - topic/standard-model
---
>[!hint]- Prerequisites
>- [[Spinors and Chiral Theories]]

>[!info]- Historical note
>In the origin, there was [[Fermi interaction|Fermi theory]], which had a nonrenormalizable contact interaction. 
>Introducing a *massive vector boson* as a mediator explained the contact interaction, but interacting massive vectors behave badly in the UV.
>Glashow later identified the $SU(2) \times U(1)$ Yang-Mills structure, which fixes the interactions and gave important cancellations in the UV, but masses still had to be added by hand and breaking gauge symmetry.
>Weinberg and Salam used the [[Higgs Mechanism]] to furnish mass to those particles without breaking gauge invariance, rendering the theory well-behaved in the UV.
## $SU(2)_L \times U(1)_Y$ Gauge Group
The Standard Model is a [[Spinors and Chiral Theories|chiral theory]]: left-handed and right-handed fermions transform differently under the weak interaction.

The full gauge group for the electroweak sector is $SU(2)_L \times U(1)_Y$:
* **$SU(2)_L$ (Weak Isospin):** Couples *only* to left-handed fermions. Its gauge bosons are $W^1_\mu, W^2_\mu, W^3_\mu$, and the coupling constant is $g$.
* **$U(1)_Y$ (Weak Hypercharge):** Couples to both left and right-handed fermions. Its gauge boson is $B_\mu$, and the coupling constant is $g'$.

Weak hypercharge $Y$ is defined to bridge the gap between electric charge $Q$ and the third component of weak isospin $T^3_L$ via the **Gell-Mann-Nishijima formula**:
$$
Q = T^{3}_{L} + Y
$$

## Field Representations and Quantum Numbers
Considering also the *color part* coming from QCD, and using the conjugate basis to write all right-handed fields as left-handed anti-fields, the particle representations under $SU(3)_c \times SU(2)_L \times U(1)_Y$ are:

| Field                | $SU(3)_c$ | $SU(2)_L$ | $U(1)_Y$ |
| :------------------- | :-------: | :-------: | :------: |
| $Q = (u_L, d_L)^T$   |     3     |     2     |   1/6    |
| $L = (\nu_L, e_L)^T$ |     1     |     2     |   -1/2   |
| $u^c$                | $\bar{3}$ |     1     |   -2/3   |
| $d^c$                | $\bar{3}$ |     1     |   1/3    |
| $e^c$                |     1     |     1     |    1     |

## Unbroken Interaction Lagrangian
*Before any mass is generated*, the interaction between the fermions and the gauge bosons is dictated strictly by the covariant derivative 
$$
D_\mu = \partial_\mu - ig W^a_\mu T^a - ig' B_\mu \frac{Y}{2},
$$
The **interaction Lagrangian** is:
$$
\mathcal{L}_{\mathrm{int}} = g W_{\mu}^{a} J_{\mu}^{a} + g' B_{\mu} J_{\mu}^{Y},
$$
where the $SU(2)$ currents $J^a_\mu$ involve only the left-handed doublets ($Q_L, L_L$).

After symmetry breaking $W_{\mu}^{3}$ and $B_{\mu}$ mix to produce the photon and the $Z$ boson, as discussed in [[Gauge Boson Mixing and Currents]].