There is a subtle point concerning symmetries, which is very often overlooked. Not all symmetries are equal, and only some of them are physical.

Consider a field theory on a manifold $\mathcal{M}$ described by an action 
$$
S[\varphi,g] = \int d^{d}x \sqrt{ -g }\mathcal{L}(\varphi, \partial_{\mu}\varphi).
$$

# General covariance

General covariance is not really a physical symmetry, but a requirement for the equations that appear in physics.
Consider a diffeomorphism $f:\mathcal{M}\to\mathcal{M}$. General covariance requires that 
$$
S[\varphi,g] = S[f^{*}\varphi,f^{*}g],
$$
where $f^{*}$ is the pullback of the map.
# Physical symmetries

For a symmetry to be physical, the condition is 
$$
S[\varphi,g] = S[f^{*}\varphi,g],
$$
which under general covariance is equivlent to 
$$
S[\varphi,g] = S[\varphi,(f^{-1})^{*}g].
$$
This implies that the transformation is an isometry.

# Weyl invariance

A theory must be invariant under local rescalings of the metric and the fields: 
$$
S[\varphi,g] = S[e^{ -\Delta \sigma }\varphi,g],
$$
with $\sigma(x)$ a funcion of the coordinates, and $\Delta$ a real number.

# Conformal invariance

Suppose that $f$ is conformal, which means $f*g = e^{ 2\sigma }g$, with $\sigma(x)$ a function of the coordinates. Conformal invariance states that for any such transformation we have 
$$
S[\varphi,g] = S[e^{ \Delta\sigma }\varphi,g].
$$

We have that **Weyl invariance and general covariance imply conformal invariance**.