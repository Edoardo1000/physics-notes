> Prerequisite: [[Anomalies]]
# Gauge anomalies
For a theory to *make sense*, it must not possess gauge [[Anomalies|anomalies]].
Let's look at the groups of the Standard Model:
- $SU(3)^3$ does not have anomalies;
- $SU(2)_L^3$ does not have anomalies;
- $SU(N)$  is in general anomaly-less;
- $U(1)_Y$ is risky.

Let's look at 
$$
	\mathrm{Tr}[Y\{ T^{a},T^{b} \}].
$$
The various combinations give:
- $SU(3)^2 \times U(1)_{Y} \implies$ no anomaly
- $SU(2)^2 \times U(1)_Y \implies$ no anomaly
- $\mathrm{Tr}(Y^3) = 0 \implies$ no anomaly
Thus, **there are no gauge anomalies in the Standard Model**.
# Global anomalies
Regarding the [[Global Symmetries of the Standard Model|global symmetries]] of the Standard model, we have:
- **Baryon number:** $SU(3)_c$ is okay, while we have 
  $$
  	\mathrm{Tr}[B\{ T^{a},T^{b} \}] = \frac{\delta^{ab}}{2}N_{f},\quad \mathrm{Tr}[B Y^{2}] = - \frac{N_{f}}{2}
  $$
  which are not zero. Thus, *baryon number is anomalous*. In particular, we have 
  $$
	\langle \partial_{\mu} J^{\mu}_{B} \rangle = - \frac{1}{32\pi^{2}} \epsilon^{\mu \nu \rho \sigma} N_{f}(W_{\mu \nu}^{a}W_{\rho \sigma}^{a}-B_{\mu \nu}B_{\rho \sigma}).
  $$
- **Lepton number:** by doing an analogous calculation, we find 
  $$
  	\langle \partial_{\mu}J^{\mu}_{L} \rangle = \langle \partial_{\mu}J^{\mu}_{B} \rangle .
  $$

From this, we observe that *$B-L$ is a symmetry also at the quantum level*.

Thus, the question wether or not $B-L$ can be a *gauge symmetry* arises. We just have to look at $\mathrm{Tr}[(B-L)^{3}]$.

# Charge quantization
It might be suprising that the charges of the particles are all a **multiple of some fundamental charge**. This charge quantization maybe is due to the need for *anomaly cancellation*.

Let's try to calculate the anomaly coefficients for *generic hypercharge*.
We have:
- $\mathrm{Tr}[t^{a}t^{b}Y] = \frac{\delta^{ab}}{2}(Y_{q}N_{c}+Y_{\ell})=0$
- $\mathrm{Tr}[T^{a}T^{b}Y]=\frac{\delta^{ab}}{2}(2Y_{q}+ Y_{u} + Y_{d})=0$
- $\mathrm{Tr}[Y^{3}]=2N_{c}Y_{q}^{3} + N_{c}Y_{d}^{3}+2Y_{\ell}^{3}+Y_{e}^{3}=0$
- $\mathrm{Tr}[Y] =0$
The last condition comes from **gravity**, you can see it as $\mathrm{Tr}[Y R_{\mu \nu}R^{\mu \nu}]=0$.

There are two solutions. One of them is the *Standard model*: 
$$
	Y_{u} = -4Y_{q},\quad Y_{d}=2Y_{u},\quad Y_{\ell} = -3Y_{q},\quad Y_{e} = 6Y_{q} = -2Y_{\ell};
$$
the Standard Model correponds to the choice $Y_{q} = \frac{1}{6}$. There is also a simpler solution:
$$
	Y_{q} = Y_{\ell} = Y_{e} = 0,\quad Y_{u} = -Y_{d}.
$$

**Observation:** The particles were known *a priori*. If we for example add another particle, such as a right neutrino, the system becomes *underdetermined*.

#### Adding a right neutrino
If we add a $\nu_{R}$ particle, the conditions become 
$$
	\frac{\delta^{ab}}{2} (Y_{q}N_{c}+ Y_{\ell})=0,\quad \frac{\delta^{ab}}{2} (2 Y_{q} + Y_{y} +Y_{d})=0.
$$
I have two free parameters. However, the solution becomes unique again if we add $\frac{B-L}{2}$:
$$
	\mathrm{Tr}\left[ \frac{t^{a}t^{b}(B-L)}{2} \right]= \sum_{\mathrm{doublet}} \frac{\delta_{ab}}{2}\left[ N_{c}\cdot \frac{1}{6}-\frac{1}{2} \right]=0,
$$
and we have 
$$
	Y = T_{3R} + \frac{B-L}{2}.
$$
If we wanted to *extend $B-L$ to a gauge symmetry*, we indeed needed $\nu_{R}$.  Without it, we would have 
$$
	\mathrm{Tr}\left[ \left( \frac{B-L}{2} \right)^{3} \right] = 2N_{c} \left( \frac{1}{6} \right)^{3} + 2 \left( -\frac{1}{2} \right)^{3} + 2 N_{c}\left( -\frac{1}{6} \right)^{3} + \left( \frac{1}{2} \right)^{3} = -\frac{1}{8}.
$$
The $\nu_{R}$ adds a $\left( \frac{1}{2} \right)^{3}$ which cancels the anomaly. 

We observe that the second solution becomes $Y_{e} = -Y_{\nu}$.

