# Particle decay
In nature, there appear to be many particles which do not live forever, but eventually decay **lighter particles**.
Consider a particle of mass $M$ which decays in $n$ products: 
$$
	\phi \to X,
$$
its **decay width** is defined as 
$$
	\Gamma_{X} = \frac{1}{2M}\int \lvert A(\phi \to X) \rvert ^{2} d\Phi_{n},
$$
where $d\Phi_{n}$ is the *phase space element (see [[Particle Scattering]] for the definition)*.
The **total decay with** $\Gamma$ is defined as the sum over all possible final products.

### Decay in two particles with the same mass
In this case, the phase space element becomes 
$$
	d\Phi_{2} = \frac{d\Omega}{32\pi^{2}}\sqrt{ 1-\frac{4m^{2}}{M} }
$$


# Breit-Wigner distribution
In collider experiments, *virtual intermediate particles* are often created. An intermediate particles appear as propagators in scattering amplitudes. If the particles were stable, the propagator, and thus cross sections, would diverge. However, due to the particles being unstable, the divergence gets smeared out due to an additional **imaginary mass term**. The propagator becomes 
$$
	D(s) = \frac{1}{s-M^2 + i\sqrt{ s }\Gamma(s)},
$$
where $\Gamma(s)$ is the total decay width, but with the mass of the particles substituted with $\sqrt{ s }$, and $M$ is the *physical mass* of the particle.

>[!math]- Derivation: propagator of an unstable particle
>
>In general, the propagator of a particle can be written as 
>$$ D(s) = \frac{1}{s - M^2 - i \mathrm{Im}\Sigma(s)}, $$
>where $M$ is the *physical mass* of the particle, and $\Sigma(s)$ is the sum of all the IPI diagrams. The real part of $\Sigma$ has been reabsorbed in the definition of the physical mass.
> Now, the **Optical theorem** states that 
>$$ \mathrm{Im}\Sigma(s) = -\sqrt{ s } \Gamma(s), $$
>where $\Gamma(s)$ is the decay rate of a **virtual decaying particle**, which appears when colliding particles at high energies.
>From this relation, the result immediately follows.

