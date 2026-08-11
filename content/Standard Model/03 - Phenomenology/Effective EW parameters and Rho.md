---
tags:
  - type/derivation
  - topic/electroweak
---
# Effective EW Couplings and the Rho Parameter

To compare theoretical predictions with experimental data, we describe the effect of radiative corrections using an **effective vertex**. Due to one-loop contributions, the vertex for the process 
$$
	Z \to f + \bar{f}
$$
is not just the tree-level one. It is described by  
$$ \mathcal{V}^{\mu} = \frac{g}{2 \cos \theta_W} \bar{f} \gamma^\mu(g_{V,f}^{eff} - g_{A,f}^{eff}\gamma_5)f. $$
Our task is to find an expression for the effective couplings in terms of theory data, so that they can be compared with experiments.

# Theoretical calculation at 1-loop
In order to calculate them at 1-loop level, it is convenient to map them into an **effective radius ($\rho_f$) and angle ($\theta_f^e$)**:
$$ g^e_{V,f} = \sqrt{\rho_f}(T^3_f - 2 Q^2 \sin^2 \theta_f^{eff}), \quad g_{A,f}^e = \sqrt{\rho_f}T^3_f.$$

>[!note]- Physical interpretation of $\rho$
> The parameter $\rho_f$ measures how neutral and charged current interactions differ from each other ($G_F^{nc,f} = \rho_f G_F^{cc,f}$). At tree-level, $\rho_f = 1$. Any deviation ($\rho_f \neq 1$) is a direct indicator of **custodial symmetry breaking**.

Usually, the parameters are written as 
$$
	\rho_{f} \equiv 1 + \Delta \rho_{f}, \quad \sin ^{2}\theta^{eff} = \sin ^{2}\theta_{W}(1 + \Delta \kappa)
$$
After a tedious calculation, we arrive at the result that 
$$
\Delta \rho_{f} =  \frac{N_c y_t^2}{32\pi^2} = \frac{3m_t^2 G_F}{8\sqrt{2}\pi^2} 
$$
## Calculation
You can take a look at [[Calculation of the Rho parameter]].