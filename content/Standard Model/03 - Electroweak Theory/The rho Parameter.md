Since the various components of $H$ are linked by $SU(2)$ symmetry, the [[Electroweak Mass Generation|masses of the vector bosons]] are not independent of each other. This relationship is defined by the **$\rho$ parameter**:
$$
\rho \equiv \frac{m_{W}^{2}}{m_{Z}^{2} \cos ^{2} \theta_{W}},
$$
which is equal to $1$ at tree level.

Loop corrections to $\rho$ are found in [[Effective EW parameters]].

# BSM contributions
The [[Sigma Model for Higgs|sigma model for Higgs]] lets us parametrize possible variations of $\rho$ due to BSM physics.

Since $T^{3}_{R}$ is the only gauge generator, $g'$ explicitly breaks the symmetry.
If $g'$ were zero, the $W$ bosons would form a triplet with identical masses, and $B$ would be a singlet. *However*, because of $g'$ they mix and the masses are different.

The parameter $\rho$ signals how much custodial symmetry is broken. In the Standard Model, its value is one, but Beyond Standard Model particles might cause the parameter to deviate from it.

For example, in the effective Lagrangian, I can add the term
$$
	\mathcal{L} = \frac{v^{2}}{4}\mathrm{Tr}[D_{\mu}U^{\dagger} D^{\mu}U] + \epsilon \frac{v^{2}}{4} \mathrm{Tr}[D_{\mu}U^{\dagger} U \sigma_{3}]^{2}.
$$
Observe that $\mathrm{Tr}[D_{\mu}U^{\dagger}U]=0$ (just put $U=1)$.
This shifts the $Z$ mass by 
$$
	\delta m_{Z}^{2} = \frac{v^{2}}{4}(g^{2}+g'^{2})\epsilon,
$$
which thereby implies
$$
	\rho = \frac{1}{1+\epsilon}.
$$
Thus, this term in the effective action is what parametrizes the breaking of custodial symmetry.
We can get bounds on BSM physics energy by restoring the original dimensionful $\mathcal{H}$, thus obtaining the term
$$
	\frac{1}{\Lambda^{2}}\mathrm{Tr}[D_{\mu}\mathcal{H}^{\dagger} \mathcal{H} \sigma_{3}],
$$
from which we deduce $\epsilon \sim \frac{v^{2}}{\Lambda^{2}}$. 
From experiments we know $\epsilon \leq 0.1 \%$, so that $\Lambda$ is $O(\mathrm{TeV})$.