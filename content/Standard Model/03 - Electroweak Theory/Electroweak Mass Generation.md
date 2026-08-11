## Historical Motivation
Glashow's mixing unified the weak and electromagnetic forces, but it required the $W$ and $Z$ bosons to be exactly massless to preserve gauge invariance. In 1967, Weinberg and Salam solved this by applying the mechanism discovered by Higgs, Englert, and Brout (1964) to the $SU(2) \times U(1)$ model, generating mass through the [[Higgs Mechanism]].

## Higgs Doublet
To break $SU(2)_L \times U(1)_Y \to U(1)_{\text{em}}$, we introduce a complex scalar $SU(2)$ doublet with Hypercharge $Y=1$:
$$
H = \begin{pmatrix} i\phi^{+} \\ \frac{v + h + i \phi^{0}}{\sqrt{2}} \end{pmatrix}, \quad \langle H \rangle = \frac{1}{\sqrt{2}}\begin{pmatrix} 0 \\ v \end{pmatrix}
$$

We specifically align the Vacuum Expectation Value (VEV), $v$, in the lower (neutral) component. This ensures the vacuum remains uncharged, meaning the photon remains strictly massless: $Q \langle H \rangle = 0$.

## Gauge Boson Masses
When the Higgs field acquires its VEV, the covariant derivative generates mass terms for the gauge bosons.

> [!math]- Derivation: Evaluating $\lvert D_\mu H \rvert^2$
> The kinetic term for the Higgs is $\lvert D_\mu H \rvert^2$. In the vacuum, we evaluate it acting on $\langle H \rangle$:
> $$
> \lvert DH \rvert ^{2} = \frac{1}{2} \left[\left( g T^{a}W^{a}_{\mu} + \frac{1}{2}g' B_{\mu} \right) \begin{pmatrix} 0 \\ v \end{pmatrix} \right]^{\mathrm{T}} \left[ \left( g T^{a} W^{a}_{\mu} + \frac{1}{2} g' B_{\mu}\right) \begin{pmatrix} 0 \\ v \end{pmatrix} \right]
> $$
> Expanding the Pauli matrices $T^a = \sigma^a/2$:
> $$
> \lvert DH \rvert ^{2} = \frac{g^{2} v^{2}}{4} W_{\mu}^{+} W_{\mu}^{-} + \frac{v^{2}}{8}(-g W^{3}_{\mu} + g' B_{\mu})^{2}
> $$
> Using the Weinberg rotation to substitute $(-g W^3_\mu + g' B_\mu) = \sqrt{g^2 + g'^2} Z_\mu$, we get:
> $$
> \lvert DH \rvert ^{2} = \frac{g^{2} v^{2}}{4}W_{\mu}^{+ } W_{\mu}^{-} + \frac{v^{2}}{8} (g^{2} + g'^{2})Z_{\mu}Z_{\mu}
> $$

From this expansion, we extract the physical masses:
$$
m_{W} = \frac{1}{2}vg, \quad m_{Z} = \frac{1}{2}v\sqrt{g^{2} + g'^{2}}.
$$
From this, we also have the relation 
$$
	G_{F} = \frac{1}{\sqrt{ 2 }v^{2}}
$$
### The $\rho$ Parameter
Because of the specific geometric structure of a single $SU(2)$ doublet, the masses are fundamentally linked. At tree level, this relationship is defined by the $\rho$ parameter:
$$
\rho \equiv \frac{m_{W}^{2}}{m_{Z}^{2} \cos ^{2} \theta_{W}} = 1
$$

## Fermion Mass Generation 
Because the Standard Model is chiral (left and right-handed fields have different $SU(2)$ quantum numbers), explicit fermion mass terms like $m \bar{\psi}_L \psi_R$ are forbidden by gauge invariance. 

Instead, fermions acquire mass by coupling to the Higgs doublet via **Yukawa interactions**. Using the Higgs field $H$ and its charge conjugate $H^c = -i \sigma_2 H^*$:
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
> \mathcal{L}_{\text{mass}} = \frac{Y_{e} v}{\sqrt{2}} \bar{e}_{L} e_{R} + \mathrm{h.c.}
> $$

This gives the general formula for all fermion masses in the Standard Model:
$$
m_{f} = \frac{1}{\sqrt{2}} Y_{f} v
$$