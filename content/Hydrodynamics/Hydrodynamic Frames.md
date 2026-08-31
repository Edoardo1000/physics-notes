In hydrodynamics, the only physical observables are the stress-energy tensor and conserved currents. The field we use to parametrize them can be redefined at will. Because of this, various conventions (frames) can be used. Here we list some examples.

Consider the [[Relativistic Hydrodynamics]] at first order in the derivative expansion.

# Eckart frame

Define $u^\mu$ so that it points along the particle/charge flow, so that 
$$
J^{\mu} = n u^{\mu},
$$
exactly. This forces the charge dissipation to appear in the heat flux in $T^{\mu \nu}$: 
$$
q^{\mu}_{\mathrm{Eckart}} = -\kappa \Delta^{\mu \nu}(\partial_{\nu}T + T a_{\nu}),\quad a^{\mu} = u^{\nu}\partial_{\nu}u^{\mu}.
$$

# Landau frame

Define $u^{\mu}$ to be the timelike eigenvector of the stress tensor: 
$$
T^{\mu \nu}u_{\nu} = - \epsilon u^{\mu}.
$$
This forces 
$$
q^{\mu} = 0,\quad \pi^{\mu \nu}u_{\nu}=0.
$$
The dissipation shows up in the current part:
$$
\nu^{\mu}_{\mathrm{La ndau}} = -\sigma_{Q} T \Delta^{\mu \nu}\partial_{\nu} \left( \frac{\mu}{T} \right).
$$
