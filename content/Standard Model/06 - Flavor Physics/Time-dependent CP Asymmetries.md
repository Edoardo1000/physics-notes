This phenonemon occurs when there is [[Meson Mixing|meson mixing]], combined with a decay channel common to both mesons and its antimatter partner.

Thus, suppose the mesons $M^{0}, \bar{M}^{0}$ both decay into $f$. Since there is also meson mixing, there can be interference between different decay paths.
If we start from the meson $M^{0}$, and look at its decay after some time $t$, there are two possible processes:
$$
	M^{0}\to f, \quad \bar{M}^{0} \to M^{0} \to f.
$$
We can take a look at the observable
$$
	A_{CP}(t) \equiv \frac{\Gamma(\bar{M}^{0}(t)\to f) - \Gamma(M^{0}(t)\to f)}{\Gamma(\bar{M}^{0}(t)\to f)+\Gamma(M^{0}(t)\to f)},
$$
since now the particle evolves in time. After some calculations we find
$$
\begin{align}
 A_{CP}(t)  &  = \frac{(1-\lvert \lambda_{f} \rvert ^{2})\cos \Delta\omega t - 2 \mathrm{Im}\lambda_{f} \sin \Delta\omega t}{1 + \lvert \lambda_{f} \rvert ^{2}} \equiv  \\
  & \equiv C_{f} \cos \Delta\omega t - S_{f} \sin \Delta\omega t
\end{align},
$$
with 
$$
\lambda_{f} \equiv \frac{\bar{A}_{f}}{A_{f}} \frac{q}{p},\quad A_{f} = \bra{f} H\ket{M^{0}} ,\quad \bar{A}_{f} = \bra{f} H \ket{\bar{M}^{0}}  .
$$
We see that this observable may not be zero even if both $\frac{\bar{A}_{f}}{A_{f}}, \frac{q}{p}$ have unit norm. Note that even though the single ratios change under rephasing of the states, their product remains constant, and is thus a legitimate physical observable.

To do the calculation, take 
$$
	\ket{M^{0}(t)} = g_{+}(t)\ket{M^{0}} + \frac{q}{p}g_{-}(t)\ket{\bar{M}^{0}}
$$
just like in [[Meson Mixing]]. The final expression requires 
$$
	\left\lvert  \frac{q}{p}  \right\rvert = 1
$$
