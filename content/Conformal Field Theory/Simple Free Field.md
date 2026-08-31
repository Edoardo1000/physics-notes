
The space built from this theory is the Fock space. 
 Its dimension is fixed by the one of the ambient space: 
$$
	\Delta_{\phi} = \frac{d}{2}-1,
$$
and it obeys the equation of motion 
$$
	\Box \phi = 0
$$
## Thermal partition function

- Consider a state $\ket{\Delta,m}$. States constructed from him contribute $(1-q^{\Delta y^{m}})^{-1}$ to the partition function, so we have the *thermal partition function*:
$$
	Z^{\mathrm{free}} = \prod_{\Delta,m} \frac{1}{1- q^{\Delta}y^{m}} = \prod_{\ell=0^{\infty}}\prod_{m=-\ell}^{\ell} \frac{1}{1-q^{\ell+1/2}y^{m}}.
$$
^partition-function

There is, however, a better representation, which is 
$$
	\log Z^{\mathrm{free}} = - \sum_{\Delta,m}\log(1-q^{\Delta}y^{m}) = \sum_{\Delta,m}\sum_{n=1}^{\infty} \frac{(q^{\Delta}y^{m})^{n}}{n} = \sum_{n=1}^{\infty} \frac{1}{n} \sum_{\Delta,m} q^{n\Delta}y^{nm},
$$
and in the last sum we recognize the character of the one-particle space, evaluated at $q^{n}, y^{n}$. Using the expansion 
$$
	\chi^{\mathrm{free}}(q,y) = \chi_{\frac{1}{2},0}(q,y) - \chi_{\frac{5}{2},0}(q,y) = \frac{q^{1/2}(1+q)}{(1-qy)\left( 1-\frac{q}{y} \right)},
$$
we finally find 
$$
	\log Z^{\mathrm{free}} \sum_{n=1}^{\infty} \frac{1}{n} \frac{q^{n/2}(1+q^{n})}{(1-q^{n}y^{n})(1-q^{n}y^{-n})} = \sum_{n=1}^{\infty} \frac{1}{n} \frac{q^{n/2}(1+q^{n})}{1+q^{2n}-2q^{n}T\left( 1+\frac{u}{2} \right)}.
$$
Here, $T_{n}$ denotes the Chebyshev polynomial of the first kind. We can expand in characters 
$$
	Z^{\mathrm{free}}(q,y) = \sum_{\Delta,\ell}m_{\Delta,\ell} \chi_{\Delta,\ell}(q,y).
$$
If we expand in powers of $q$, we get 
$$
	Z^{\mathrm{free}} = 1 + \chi^{\mathrm{free}} + \chi_{1,0} + \chi_{\frac{3}{2},0} + \chi_{2}^{\mathrm{short}} + \chi_{2,0} + \dots, \quad \chi_{\ell}^{\mathrm{short}} = \chi_{\ell+1,\ell} - \chi_{\ell+2, \ell-1}.
$$

# "Short" Verma module

In this case 
$$
	P^{2}\ket{\phi} = 0.
$$
Thus, we have null states, which need to be subtracted from the Verma module. This means that to find the character we must subtract the character of the null state from the one of the full Verma module, that is 
$$
	X_{SFF}(q) = \frac{q^{d/2-1} - q^{d/2+1}}{(1-q)^{d}}.
$$