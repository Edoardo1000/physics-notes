---
tags:
  - topic/electroweak
  - topic/standard-model
---
>[!hint]- Prerequisites
>- [[Glashow-Weinberg-Salam Model]]: definition of the gauge group;
>- [[Gauge Boson Mixing and Currents]]: how the physical bosons are defined;
>- [[Higgs Mechanism]]: how the process works in a general QFT

We need to *give mass to the $W$ and $Z$ bosons*, while still maintaining a **massless photon**. This is achieved by introducing the **Higgs doublet**. 
## Higgs Doublet
 To break $SU(2)_L \times U(1)_Y \to U(1)_{\text{em}}$, we introduce a complex scalar $SU(2)$ doublet with Hypercharge $Y=1$:
$$
H = \begin{pmatrix} H^{+} \\ \frac{v + h + i \phi^{0}}{\sqrt{2}} \end{pmatrix}, \quad \langle H \rangle = \frac{1}{\sqrt{2}}\begin{pmatrix} 0 \\ v \end{pmatrix}.
$$
We aligned $\langle H \rangle$ in the second component because this ensures a massless photon: we have $Q\langle H \rangle = 0$, implying that the photon corresponds to the unbroken generator. 

The potential which causes the nonzero VEV is described in [[Higgs Boson Interactions]].
## Gauge Boson Masses
When the Higgs field acquires its VEV, the covariant derivative generates *mass terms for the gauge bosons*.

> [!math]- Derivation: Evaluating $\lvert D_\mu H \rvert^2$
> The kinetic term for the Higgs is $\lvert D_\mu H \rvert^2$. In the vacuum, we evaluate it acting on $\langle H \rangle$:
> $$
> \lvert DH \rvert ^{2} = \frac{1}{2} \left[\left( -ig T^{a}W^{a}_{\mu} + -i\frac{g'}{2} B_{\mu} \right) \begin{pmatrix} 0 \\ v \end{pmatrix} \right]^{\dagger} \left[ \left( -ig T^{a} W^{a}_{\mu} + -i \frac{g'}{2} B_{\mu}\right) \begin{pmatrix} 0 \\ v \end{pmatrix} \right]
> $$
> Expanding the Pauli matrices $T^a = \sigma^a/2$:
> $$
> \lvert DH \rvert ^{2} = \frac{g^{2} v^{2}}{4} W_{\mu}^{+} W_{\mu}^{-} + \frac{v^{2}}{8}(-g W^{3}_{\mu} + g' B_{\mu})^{2}
> $$
>The expression in parenthesis is exaclty equal to $Z_{\mu}\sqrt{g^2 + g'^2}$, so we get
> $$
> \lvert DH \rvert ^{2} = \frac{g^{2} v^{2}}{4}W_{\mu}^{+ } W_{\mu}^{-} + \frac{v^{2}}{8} (g^{2} + g'^{2})Z_{\mu}Z_{\mu}.
> $$

From the expansion, we extract the **physical masses**:
$$
m_{W} = \frac{1}{2}vg, \quad m_{Z} = \frac{1}{2}v\sqrt{g^{2} + g'^{2}}.
$$
From this, we also have the relation 
$$
	G_{F} = \frac{1}{\sqrt{ 2 }v^{2}}.
$$
## Fermion Mass Generation 
Because the Standard Model is **chiral** (left and right-handed fields have different $SU(2)$ quantum numbers), explicit fermion mass terms like $m \bar{\psi}_L \psi_R$ are forbidden by gauge invariance. 

Instead, fermions acquire mass by coupling to the Higgs doublet via **Yukawa interactions**. Using the Higgs field $H$ and its **conjugate** 
$$
H^c = i \sigma_2 H^*,
$$
the *Yukawa sector* is
$$
\mathcal{L}_{Y} = Y_{e} \bar{L}_{L} H e_{R} + Y_{d}\bar{Q}_{L} H d_{R} + Y_{u} \bar{Q}_{L} H^{c} u_{R} + \mathrm{h.c.}
$$

> [!math]- Derivation: Expanding the Electron Mass
> Taking the electron term and expanding $H$ around its VEV:
> $$
> Y_{e} \bar{L}_{L} H e_{R} = Y_{e} \left( \bar{\nu}_{L} i \phi^{+} e_{R} + \bar{e}_{L} \frac{v + h + i\phi^{0}}{\sqrt{2}} e_{R} \right) + \mathrm{h.c.}
> $$
> Looking only at the constant VEV piece $v$:
> $$
> \mathcal{L}_{\text{mass}} = \frac{Y_{e} v}{\sqrt{2}} \bar{e}_{L} e_{R} + \mathrm{h.c.}.
> $$

This gives the general formula for all fermion masses in the Standard Model:
$$
m_{f} = \frac{1}{\sqrt{2}} Y_{f} v.
$$