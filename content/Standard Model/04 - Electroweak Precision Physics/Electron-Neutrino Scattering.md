---
tags:
  - topic/electroweak
  - topic/standard-model
---
>[!hint]- Prerequisites
>- [[Particle Scattering]]
# Weak couplings
We can write the neutral current from [[Gauge Boson Mixing and Currents]] using the **axial and vector couplings**:
$$
	J_{\mu}^{nc} = \frac{1}{2} \sum_{f} \bar{f} \gamma_{\mu} (g_{V} - g_{A} \gamma_{5})f,\quad g_{V} = T^{3} - 2 \sin ^{2}\theta_{W} Q,\quad g_{A}=T^{3}.
$$
>[!math]- Derivation: left-right and axial-vector couplings
> To derive the above expression, write the current as 
>$$
>J^{nc}_{\mu} = \sum_{f}[ g_{L}^{(f)}\bar{f}_{L}\gamma_{\mu}f_{L}+g_{R}^{(f)}\bar{f}_{R}\gamma_{\mu}f_{R}],
>$$
> where we defined 
>$$
>g_{L} = T^{3}-\sin ^{2} \theta_{W}Q, \quad g_{R} = -\sin ^{2}\theta_{W}Q.
>$$
> If we define 
> $$
> g_{V} = g_{L} + g_{R} = T^{3} - 2 \sin ^{2}\theta_{W} Q,\quad g_{A} = g_{L}-g_{R} = T^{3},
> $$
> we get the desired relation.

# $Z$ Boson exchange
## Fermi constant for the neutral current
Consider a $Z$ exchange process, such as ${\nu}_{\mu} + e \to\nu_{\mu}+e$.
 By looking at the tree-level diagrams for the neutral current Lagrangian, we have the overall factor 
$$
	\frac{g^{2}}{\cos ^{2}\theta_{W}} \cdot \frac{1}{m_{Z}^{2}} = \frac{g^{2}}{m_{W}^{2}}.
$$
From this, we deduce that **at tree level the neutral and charged Fermi constants are equal**.

## Cross Section $(\nu_{\mu}+e\to \nu_{\mu}+e)$
- **Note:** the cross section results are in the limit of **massless electrons**.

For the neutrino, we have $g_{A} = g_{V} = \frac{1}{2}$. Thus, the *effective interaction* Lagrangian is 
$$
	\mathcal{L} = \frac{G_{F}}{\sqrt{ 2 }}[\bar{\nu}\gamma_{\mu}(1-\gamma_{5})\nu][\bar{e}\gamma^{\mu}(g_{V}-g_{A}\gamma_{5})e],
$$
from which we get the *scattering cross section*:
$$
	\sigma(\nu_{\mu}+e\to \nu_{\mu}+e) = \frac{G_{F}^{2} s}{\pi}\left( g_{L}^{2} + \frac{1}{3}g_{R}^{2} \right).
$$
>[!math]- Derivation of the cross section
> The tree-level Feynman diagram is only the t-channel one, and the amplitude is 
> $$
> A =\frac{4G_{F}}{\sqrt{ 2 }}[\bar{u}(k)\gamma_{\mu}P_{L} u(k')][\bar{u}(p)\gamma^{\mu}(g_{L}P_{L}+g_{R}P_{R})u(p')],
> $$
> where $P_{L}$ and $P_{R}$ are the left and right projectors respectively.
> We need to square it, sum over the final polarizations and average over the initial ones (in this case the neutrino is only left handed), getting traces of gamma matrices.
> The left and right projectors help here because we can move them around, and we get 
> $$
> \lvert \bar{A} \rvert ^{2} = \mathrm{Tr}[\not\!{k}\gamma_{\mu}\not\!{k'}\gamma_{n}P_{L}] (\mathrm{Tr}[\not\!{p}\gamma^{\mu}\not\!{p'}\gamma^{\nu}(g_{L}^{2}P_{L}+g_{R}^{2}P_{R})] + 4 m^{2}g_{L}g_{R}\eta^{\mu \nu}).
> $$
> Evaluating the traces, we get 
> $$
> 64G_{F}^{2} [g_{L}^{2}(k \cdot p)^{2} + g_{R}^{2}(k \cdot p')^{2} - g_{L}g_{R}m^{2} k \cdot k'].
> $$
> Now, going to the massless electron limit and writing everything in terms of Mandelstam variables and the scattering angle $\theta$, the amplitude reads
> $$
> \lvert \bar{A} \rvert ^{2} = 4G_{F}^{2} s^{2}[4 g_{L}^{2} + g_{R}^{2}(1+\cos\theta)^{2}],
> $$
> from which the differential cross section and the total one can be found.

## Cross Section $(\bar{\nu}_{\mu} + e \to \bar{\nu}_{\mu} + e)$
 Now the cross section can be inferred from the previous one we found. The key idea is that **the weak force couples to left-chiral fields**. The fundamental field is $\nu_{L}$, which has left chirality, meaning that **the neutrino has negative [[Spinors and Chiral Theories#Helicity and Chirality|helicity]]**, while **the antineutrino has positive helicity**.

From the point of view of the electron, this means that the left and right components of the interaction swap. Thus, the cross section is given by 
$$
	\sigma = \frac{G_{F}^{2} s}{\pi} \left( g_{R}^{2} + \frac{1}{3}g_{L}^{2} \right).
$$

## Cross Section $(\nu_{e} + e \to \nu_{e} + e)$ and antineutrino analogue
Let's look at the scattering $\nu_{e}+e \to \nu_{e}+e$.
 In this case, we have the *t-channel $Z$ exchange* plus another term: the *u-channel W exchange*.

The cross section can again be computed with some tricks, and the result is 
$$
	\sigma(\nu_{e}+e\to \nu_{e}+e) = \frac{G_{F}^{2} s}{\pi}\left( (g_{L}+1)^{2} + \frac{1}{3}g_{R}^{2} \right).
$$

>[!math]- Derivation of the cross section
>We calculated the $Z$-exchange diagram in the previous sections. The amplitude for the $W$-exchange is
>$$
>\begin{align}  A_{W} &= \frac{G_{F}}{\sqrt{ 2 }}\bar{\nu}\gamma_{\mu}(1-\gamma_{5})e \ \bar{e}\gamma^{\mu}(1-\gamma_{5})\nu  \\ &= \frac{G_{F}}{\sqrt{ 2 }}\bar{\nu}\gamma_{\mu}(1-\gamma_{5})\nu \bar{e}\gamma^{\mu}(1-\gamma_{5})e\end{align},
>$$
>where going to the second line we used the [[Spinors and Chiral Theories#Fierz Identity|Fierz Identity]]. We observe that adding this amplitude to the $Z$ exchange one is equivalent to the change $g_{L}\to g_{L}+1$, from which the result immediately follows.


Now, it's quite easy to guess what the cross section of the process $\bar{\nu}_{e}+e \to \bar{\nu}_{e} + e$ would be: just exchange $g_{L}$ and $g_{R}$ from the previous result. Thus, we have 
$$
	\sigma(\bar{\nu}_{e}+e\to \bar{\nu}_{e}+e) = \frac{G_{F}^{2} s}{\pi}\left( (g_{R}+1)^{2} + \frac{1}{3}g_{L}^{2} \right).
$$

# Experimental measurements

*More on the measurement of the couplings can be found in [[Electron-Positron Annihilation]].*

All the cross sections we found produce **ellipses** in the $g_{V}-g_{A}$ plane. We then can find the values of $g_{v},g_{A},\sin \theta_{W}$.
- We look at the intersections of the cylinders
- One of them is very small
- We know $g_{A} = T^{3}$, which cannot be small, so it must be $g_{V}$
- To find theta, we have the relation 
  $$
  	-\frac{1}{2} + 2\sin ^{2}\theta = g_{V} \approx 0.04.
  $$

