*Conventions in [[Glossary hub]].*

People are usually interested in CFTs on $S^{1} \times S^{2}$, which is equivalent on a theory on $\mathbb{R}^{3}$ at finite temperature.

# Partition function

The simplest one is the **partition function**: 
$$
	Z(\beta,\mu) = \mathrm{Tr}_{\mathcal{H}}(e^{ -\beta D }e^{ i \mu M }) = \mathrm{Tr}_{\mathcal{H}}(q^{D}y^{M}).
$$
It contains the information about the **spectrum of primaries**: 
$$
	Z(q,y) = \sum_{\Delta,l} n_{\Delta,l} \chi_{\Delta,l}(q,y) = \int_{0}^{\infty} d\Delta \sum_{l} \rho(\Delta,l) \chi_{\Delta,l}(q,y).
$$
- Using orthogonality of characters, we can write the *inversion formula*: 
	$$
	\rho(\Delta,l) = \frac{1}{2\pi i} \int_{\gamma-i\infty}^{\gamma+i\infty} d\beta \int_{-\pi}^{\pi} d\mu \omega(\beta,\mu) \chi_{3-\Delta,l}(\beta,\mu)Z(\beta,\mu).
    $$
    ^density-inversion

For orthogonality of characters, see [[Conformal Characters]].

### Explicit examples
[[Generalized Free Field]]

# One-point functions

The next simplest correlator is the **one-point function**: 
$$
	\langle \phi(x) \rangle_{q,y} = \frac{1}{Z(q,y)} \mathrm{Tr}_{\mathcal{H}}[\phi(x)q^{D}y^{M}].
$$
Here, $\phi(x)$ is a local primary field.

![[Conformal Blocks#^thermal-1pt-block]]

We define the **averaged OPE coefficient**: 
$$
	\overline{\lambda^{a}_{\phi \mathcal{O}\mathcal{O}}} = \frac{1}{n_{\Delta,l}} \sum_{i=1}^{n_{\Delta,l}}\lambda^{a}_{\phi \mathcal{O}\mathcal{O}}.
$$

The relation between 1-point function and OPE coefficients is given by 
$$
	Z(\beta,\mu)\langle \phi(x) \rangle _{\beta,\mu} = r^{-\Delta_{\phi}} \int_{0}^{\infty}d\Delta \sum_{l} \rho(\Delta,l) \sum_{a=0}^{l}\overline{\lambda^{a}_{\phi \mathcal{O}\mathcal{O}}}g^{\Delta_{\phi},a}_{\Delta,l}(\beta,\mu,\theta).
$$

- *Inversion formula*:
$$
	\rho(\Delta,\ell)\overline{{{\lambda_{\phi O O}^{a}}}}(\Delta,\ell)={\frac{r^{\Delta_{\phi}}}{2\pi i}}\int\mathcal{W}\ g_{3-\Delta,\ell}^{3-\Delta_{\phi},a}(\beta,\mu,\theta)\,Z(\beta,\mu)\langle\phi(x)\rangle_{\beta,\mu}\,,
$$ 
^inversion-formula

with the measure $\mathcal{W}$ given by  ^2538d1
$$
	\mathcal{W}(\beta,\mu,\theta) = \frac{1}{2} \omega (\beta,\mu) \sin\theta.
$$
For the proof, [Buric et al. 2025] (https://arxiv.org/abs/2506.21671).
#### Free fields

In this case, we can use Wick's theoorem.

*Taking the OPE limit:* if the points get close together, only the $n=1$ term contributes.

Now, the OPE is 
$$
	\phi(x_{1}) \times \phi(x_{2}) \approx \frac{I}{\lvert x_{12} \rvert ^{2\Delta_{\phi}}} + \lambda_{\phi \phi \phi^{2}}\phi^{2}(x).
$$
Consider the two-point function given in the section below. If we take the expectation value of the OPE, subtract the $n=0$ contribution, which corresponds to the identity, and finally set $r=1, \theta_{1} = \theta_{2} \equiv \theta, \phi=0$, we learn that 
$$
    \begin{align}
	 \lambda_{\phi\phi\phi^{2}}\langle\phi^{2}(x)\rangle_{q,y} & =\sum_{n\ne0}\frac{q^{n\Delta_{\phi}}}{\left(1+q^{2n}-2q^{n}(\cos^{2}\theta+\sin^{2}\theta\cos(n\mu)\right)^{\Delta_{\phi}}} \\
	  & = \sum_{n=1}^{\infty} \frac{2}{\left( q^{n} + q^{-n} - 2\left( \cos ^{2}\theta + \sin ^{2}\theta T_{n}\left( 1+\frac{u}{2} \right) \right) \right)^{\Delta_{\phi}}},
	\end{align}
$$
where $T_{n}$ are the Chebyshev polynomials of the first kind.

# Two-point function

 - *Two point function at finite temperature:* at zero temperature it is simply 
$$
	\langle \phi(x_{1})\phi(x_{2}) \rangle = \frac{1}{\lvert x_{12} \rvert^{2\Delta_{\phi}} },
$$
while for finite temperature we have to find a Green's function which is periodic in imaginary time. This can be obtained by summing over the zero-temperature ones but translated, and with a twist, thereby giving 
$$
	a\langle \phi(x_{1})\phi(x_{2}) \rangle _{q,y} = \sum_{n=-\infty}^{\infty} \frac{q^{n \Delta_{\phi}}}{\lvert x_{12}^{(n)} \rvert ^{2\Delta_{\phi}}}, \quad x_{1}^{(n)}=x_{1},\ x_{2}^{(n)}=(r_{2}q^{n},\theta_{2},\phi_{2}+n\mu),
$$
(remember that we are on the plane, the translations in time are on the cylinder) ^thermal-2pt-function