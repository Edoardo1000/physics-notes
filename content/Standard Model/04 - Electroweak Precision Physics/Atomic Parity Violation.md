There is a way to measure $\sin \theta_{W}$, which uses *parity violation* in atomic physics.
Our setting is thus an electron orbiting a completely still nucleus.

Since we are at very low energies, the weak interaction can be treated as pointlike.

The key idea is to look at the observable $\vec{s} \cdot \vec{p} \ \delta^{3}(\vec{x})$.

# Effective Hamiltonian

The parity violating weak interaction Hamiltonian between the nucleus and the electron is given by 
$$
	H_{\mathrm{eff}} = - \frac{G_{F}}{\sqrt{ 2 }} \sum_{q}C_{1q} \ (\bar{e} \gamma_{\mu} \gamma_{5} e) \ (\bar{q}\gamma^{\mu}q) + C_{2q} \ (\bar{e} \gamma_{\mu} e) \ (\bar{q} \gamma_{\mu} \gamma_{5} q),
$$
where $C_{1q}$ and $C_{2q}$ are **effective coefficients**. Note that the Hamiltonian has the opposite sign with respect to the Lagrangian.

>[!math]- Derivation: Effective Coefficients
> From the interaction in [[Electron-Neutrino Scattering]], we see that the parity violating part comes from terms in the interaction Lagrangian which contain a $\gamma_{5}$ factor.
> For example, we have 
> $$
> C_{1q} = -2g_{A}^{e} g_{V}^{q} = g_{V}^{q}.
> $$
> Similarly, we get
> $$
> C_{2q} = -2g_{A}^{q} g_{V}^{e}.
> $$


Now, the $C_{1q}$ term is proportional to the size of the nucleus, while the $C_{2q}$ term is proportional to its spin (you can see that by looking at the [[Spinors and Chiral Theories#Nonrelativistic Limit|nonrelativistic limit]] of spinors).
Thus, for large nuclei, we can neglect the second term.

Next, we approximate the *nucleus* as *pointlike and completely still*. In this regime, the electron action becomes 
$$
	H_{\mathrm{e}} = \frac{G_{F}}{\sqrt{ 2 }}\left[   \frac{Q_{W}}{4}\delta(\vec{x}) \frac{\vec{\sigma} \cdot \vec{p}}{2m} + \mathrm{h.c.}\right ],
$$
where we defined the **Weak Nucleus Charge**
$$
	Q_{W} \equiv -2 (N_{u} C_{1u} + N_{d} C_{1d}) = A - 2Z + 4Z \sin ^{2}\theta_{W},
$$
with $N_{u}, N_{d}$ the number of up and down quarks respectively.

>[!math]- Derivation: Effective Electron Action
> If $\ket{N}$ is the ground state of the nucleon, we have 
> $$
> H_{\mathrm{eff}} \approx -\frac{G_{F}}{\sqrt{ 2 }} \sum_{q} C_{1q} \bra{N} \bar{q} \gamma^{\mu} q \ket{N} \ (\bar{e} \gamma_{\mu} \gamma_{5}e).
> $$
>In our approximation, the nucleus is perfectly still,  so only the temporal component of the expectation value is nonzero. We also suppose that the quarks are completely localized at the origin, so that we have $\bra{N} q^{\dagger}q \ket{N} \approx \delta(\vec{x})$.
>The electron factor then needs to be hermitian, so that the corresponding quantum operator becomes 
>$$
>\frac{\vec{\sigma} \cdot \vec{p}}{m} \to \frac{\vec{\sigma} \cdot\vec{p}}{2m} + \mathrm{h.c.}.
>$$
>Summing over all quarks of the nucleus gives the result immediately.


# Experimental observation

*You can take a look at https://arxiv.org/abs/1904.00281.*
