Hydrodynamics is the long-wavelength Effective Field Theory of a many body system near local thermal equilibrium.

Degrees of freedom: 
- **local temperature:** $T(x)$;
- **chemical potentials:** $\mu(x)$, one for each conserved charge;
- **fluid velocity:** $u^{\mu}(x)$.

The fieds obey the equations of motion 
$$
\nabla_{\mu} T^{\mu \nu} = 0,\quad \nabla_{\mu}J^{\mu} = 0,
$$
where $T,J$ are called *constitutive relation*: expressions for the stress tensor and current in terms of the fields and their derivatives.

Suppose the background metric is stationary, with Killing vector $\xi$.
The temperature field obeys the [[Tolman-Ehrenfest Effect|Tolman-Ehrenferst relation]].

>[!warning]- Tolman temperature and local temperature
>When doing the derivative expansion, the local temperature i just a field we named $T(x)$, which is a priori independent from the Tolman temperature $\frac{T_{0}}{\lvert \xi \rvert}$. 
>Normally, $T(x)$ is written as a derivative expansion, so that at leading order the usual flat space relation $\epsilon = \epsilon(T)$ is still true, i.e. you declare that $\langle T^{00} \rangle\equiv\epsilon(T(x))$, with $T^{00}$ the stress-energy tensor in the flat-space case .
>It turns out that at equilibrium and zeroth order in the derivative expansion the two temperatures are equal.

# Derivative expansion

Hydrodynamics is valid when the fields vary slowly compared to the microscopic mean free path of the particles.
### Zeroth order
We can write the constitutive relations as 
$$
T^{\mu \nu} = (\epsilon + \mathcal{P})u^{\mu}u^{\nu} + \mathcal{P} g^{\mu \nu},\quad J^{\mu} = n u^{\mu}. 
$$
Here, $\epsilon,\mathcal{P},n$ are related by an equation of state.
### Higher orders
This time we write the expansion as 
$$
T^{\mu \nu} = \epsilon u^{\mu} u^{\nu} + p \: \Delta^{\mu \nu} + q^{\mu} u^{\nu} + q^{\nu} u^{\mu} + \pi^{\mu \nu},\quad J^{\mu} = n u^{\mu} + \nu^{\mu}.
$$
Here, $\Delta^{\mu \nu}=g^{\mu \nu}+u^{\mu}u^{\nu}$, the charge-diffusion term satisfies $\nu^{\mu}u_{\mu}=0$, and $\pi^{\mu \nu}$ is the shear stress 
$$
\pi^{\mu \nu} = -\eta \sigma^{\mu \nu},\quad \sigma^{\mu \nu} = \Delta^{\mu\alpha} \Delta^{\nu\beta} (\partial_{\alpha}u_{\beta} + \partial_{\beta} u_{\alpha}) - \frac{2}{d-1}\theta,\quad \theta=\partial_{\mu} u^{\mu},
$$
with $\eta(T,\mu)$ the shear viscosity.

Note that we defined $q^{\mu},\pi^{\mu \nu},\nu^{\mu}$ as the terms in the constitutive equations which are not the zeroth order ones. We can then do a derivative expansion 
$$
\pi_{\mu \nu} = \pi^{(1)}_{\mu \nu}+ \pi^{(2)}_{\mu \nu}+ \dots,\quad \nu_{\mu} = \nu^{(1)}_{\mu}+\nu^{(2)}_{\mu}+\dots,
$$
where the superscript determines the number of derivatives.

There is some freedom to redefine the fields, more on [[Hydrodynamic Frames]].


#### Partition Function
The coefficients appearing in the constitutive relations obey some constraints, which are obtained using the [[Equilibrium Partition Function Method]].
