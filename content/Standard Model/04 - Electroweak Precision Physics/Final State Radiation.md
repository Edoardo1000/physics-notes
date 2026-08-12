In a collider experiment, consider for example the following process 
$$
	e + \bar{e} \to \gamma^{*} \to q + \bar{q} + g,
$$
with a *soft final photon, in the limit of massless fermions*.
Recalling [[Electron-Positron Annihilation|electron-positron annihilation]],  the cross section of the process without the gluon is given by 
$$
	\sigma_{0} = \frac{4\pi\alpha^{2}}{3s} \sum_{q}Q_{q}^{2}N_{c},
$$
with $Q_{q},N_{c}$ the charge and number of colors of the outgoing fermions, respectively.

The peculiarity of this process is that there is an **infrared divergence** coming from the gluon. Let's see it in detail.

**Note:** If the fermions were massive, there would be no collinear divergence (see the following), but the divergence due to the *soft gluon* remains,
# Real emission
The amplitude of the full process is given by summing two Feynman diagrams: the gluon is emitted by either the quark or the anti-quark.
Let's call the Mandelstam variables 
$$
	s_{12} = (p_{q} + p_{g})^{2},\quad s_{23} = (p_{\bar{q}} + p_{g})^{2},\quad s_{13} = (p_{q} + p_{\bar{q}})^{2},
$$
while the photon momentum is 
$$
	q^{2} = s_{12} + s_{13} + s_{23}.
$$
Calculating the cross section, we arrive at the expression 
$$
	\sigma_{q\bar{q}g} = \frac{1}{2\pi} \int_{0}^{1}dy_{12} \int_{0}^{1-y_{12}}dy_{23}\left[ \frac{y_{12}}{y_{23}} + \frac{y_{23}}{y_{12}} + 2\left( \frac{1}{y_{12}y_{23}}-\frac{1}{y_{12}}-\frac{1}{y_{23}} \right)\right].
$$
The integration is a triangle (*the Dalitz plot*), and the edges of the triangle $y_{12}\to_{0}$ and $y_{23}\to_{0}$ correspond to infrared **log divergences**.

# Loop divergence
In the massless fermion limit, the loop acquires the same divergence as the real emission part, plus some finite terms.
The integral we have to consider is 
$$
   -\frac{\alpha}{4\pi} \int dx dy dz \ \frac{q^{2}(1-x)(1-y)}{q^{2}xy-z\mu_{IR}^{2}},
$$
which also has a log divergence.

# Physical interpretation
The two divergences perfectly cancel, thereby giving a finite total cross section.
Now, all experiments have **finite resolution in energy**; for example, a detector might be sensible only to photons/gluons with an energy greater than $E_{\mathrm{min}}$, and the total cross section can be divided as 
$$
	\sigma_{\mathrm{tot}} = \sigma_{2\to 2} + \sigma_{2\to 3},
$$
where 
$$
	\sigma_{2\to 3} = \sigma_{q\bar{q}g}\bigl|_{E>E_{\mathrm{min}},\theta>\delta},
$$
takes into account all the process in which the emitted gluon is **energetic enough and not collinear** with the quark. Thanks to this condition, this cross section is *IR finite*, even though it might behave like $\log \frac{q^{2}}{E_{\mathrm{min}}^{2}}$. The first term is *also IR finite*: 
$$
	\sigma_{2\to 2} = \sigma_{q\bar{q}}\bigl|_{\mathrm{1-loop}} + \sigma_{q\bar{q}g}\bigr|_{E<E_{\mathrm{min} }\ \mathrm{ or}\ \theta<\delta},
$$
which can be interpreted as the cross section of producing a **jet**. A jet can be defined as generic two-body final state. The key idea is that **it's impossible to distinguish between a final quark and its cloud of surrounding gluons**, so the cross section cannot distinguish between them with *infinite precision*.
